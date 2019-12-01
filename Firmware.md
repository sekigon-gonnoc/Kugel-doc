# Kugel用のファームウェアの作成

- BLE Micro Pro用のソースコードをgithubからcloneする
  ```
  git clone -b dev/ble_micro_pro https://github.com/sekigon-gonnoc/qmk_firmware.git qmk_firmware_bmp
  ```

- ビルドできることを確認
    ```
    make kugel:default:uf2
    ```

# トラックボールの設定
## 関係する変数、関数
- *tb_info
  - センサが読み取ったボールのx方向y方向の動き(速度)
- tb_div
  - センサの感度を決める変数。値が大きいほど感度が低くなる
- tb_scrl_flag
  - このフラグがオンの時、ボールの動きをスクロールとして送信する
  - 141行目あたり

## レイヤによる動作の切り替え
- レイヤによって感度、スクロールを切り替える
  - keymap.c:113
    ```c
    if (layer_state == 0) {
        tb_scrl_flag = 0;
        tb_div = 64;
    } else if (layer_state == 0b100) {
        tb_scrl_flag = 1;
        tb_div = 64;
    } else if (layer_state == 0b10) {
        tb_scrl_flag = 0;
        tb_div = 256;
    }
    ```

## 移動量に応じた感度の切り替え
- 一定速度以上で動いた場合に感度を倍にする
  - keymap.c:130
    ```c
    if (tb_info->x > 400 || tb_info->x < -400) {
        mouse_rep.x *= 2;
    }

    if (tb_info->y > 400 || tb_info->y < -400) {
        mouse_rep.y *= 2;
    }
    ```