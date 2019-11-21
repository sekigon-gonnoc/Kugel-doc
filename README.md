# Kugel-1 ビルドガイド

自作キーボードキットKugel-1のビルドガイドです  
組立前に必ず一回以上確認してください

## 準備
### キット内容の確認
- メインPCB x1
- トップPCB x1
- ボトムPCB x1
- アクリルミドルプレート x1
- 電池ボックス x1
- 電源スイッチ x1
- リセットスイッチ x1
- M2x5ねじ x25
- M2x3ねじ x3
- M2x8スペーサー x11
- M2x3スペーサー x3
- トラックボール用セラミックボール x1

<details><summary>パーツ画像一覧</summary>
<p>

|<br>![part](./img/part012.jpg)|
|-|
|メインPCB 1個|
|<br>![part](./img/part009.jpg)|
|ボトムPCB 1個|
|<br>![part](./img/part011.jpg)|
|トップPCB 1個|
|<br>![part](./img/part014.jpg)|
|ミドルプレート 1個|
|<br>![part](./img/part010.jpg)|
|BLE Micro Proカバー 1個|
|<br>![part](./img/part015.jpg)|
|トラックボール用プレート 1個|
|<br>![part](./img/part013.jpg)|
|トラックボール用IC, レンズ 1セット|
|<br>![part](./img/part018.jpg)|
|セラミックボール 1個|
|<br>![test](./img/part001.jpg)|
|リセットスイッチ 1個|
|<br>![part](./img/part019.jpg)|
|電源スイッチ 1個|
|<br>![part](./img/part016.jpg)|
|単三電池ケース 1個|
|<br>![part](./img/part002.jpg)|
|ネジ M2x5 25個|
|<br>![part](./img/part003.jpg)|
|ネジ M2x3 3個|
|<br>![part](./img/part005.jpg)|
|スペーサ M2x8 11個|
|<br>![part](./img/part004.jpg)|
|スペーサ M2x5 3個|

</p>
</details>

### 別途必要な部品
- BLE Micro Pro x1
- コンスルーまたはピンヘッダ x2
- タミヤ 楽しい工作シリーズ No.144　ボールキャスター 
  - 家電量販店や通販で購入できます
- 塩化チオニルリチウム電池 x1
  - 無線動作させる場合は3.6Vの電池が必要です。秋月電子などで購入できます
- MXソケット x43
- MX互換スイッチ x43
- MX用キーキャップ(1U) x43

<details><summary>パーツ画像一覧</summary>
<p>

|<br>![part](./img/part006.jpg)|
|-|
|BLE Micro Pro 1個|
|<br>![part](./img/part007.jpg)|
|コンスルー 2個|
|<br>![part](./img/part008.jpg)|
|タミヤ ボールキャスター 1個|

</p>
</details>

### 工具の確認
- ハンダコテ、はんだ
- ニッパー
- ドライバー
- マスキングテープ

## 組み立て手順
1. スイッチソケットをはんだ付けする
2. トラックボール用ICをはんだ付けする
3. レンズ、リセットスイッチ、電源スイッチを差し込む
4. トッププレート、スイッチを取り付ける
5. トラックボールを取り付ける
6. リセットスイッチ、電源スイッチ、電池ボックスをはんだ付けする
7. スペーサーを取り付ける
8. BLE Micro Proを取り付けて動作確認する
9.  ミドルプレート、ボトムプレートを取り付ける
10. トラックボールの位置を調整する

### スイッチソケットのはんだ付け
![build](./img/build003.jpg)
- スイッチ用ソケットをはんだ付けしていきます  
  - ソケットが浮き上がらないように注意してください  
  - 端子の左右にフィレットができるようにしっかりハンダを盛ってください

### トラックボールICのはんだ付け
![build](./img/build004.jpg)
![build](./img/build006.jpg)
- PCBから浮かないようにトラックボールICをはんだ付けします  
  - 机の上に置いてはんだ付けするとICが浮いてしまうので、マスキングテープで固定したり指で裏側からICを押さえつけながらはんだ付けしてください
  - 写真をよく見て取り付ける向きを間違えないようにしてください

### レンズ、リセットスイッチ、電源スイッチを差し込む
![build](./img/build009.jpg)
![build](./img/build007.jpg)
- リセットスイッチ、電源スイッチを差し込みます。**はんだ付けはまだしないでください**
- 写真を参考にニッパーでレンズの両端の一部をカットします  
  - 光学部分に変色などの影響が出ないように少しずつカットしてください  
- トラックボールICの保護シールを剥がし、レンズを取り付けます

### トッププレート、スイッチを取り付ける
![build](./img/build010.jpg)
![build](./img/build011.jpg)
![build](./img/build012.jpg)
- トッププレートの上からスイッチをメインPCBに取り付けていきます  
  - ソケットが剥がれないようにメインPCBを机の上に載せて、真上からスイッチを押し込んでください
  - スイッチの足が机を傷つけないように上に作業用マットを敷いておきましよう  
- 4つくらいスイッチを取り付けるとトッププレートとメインPCBの位置関係が固定されます。リセットスイッチと電源スイッチがトッププレートの穴から操作できることを確認しておきましょう  
また、この時点でトラックボールの左上にスイッチを取り付けてもレンズと干渉しないことと、5mmのスペーサーとレンズが干渉しないことを確認してください
  - 干渉する場合は再度レンズをカットしてください
- 5mmのスペーサーをM2x3mmのなべネジで固定します
- スイッチの爪がトッププレートにはまっていることを確認しながら残りのスイッチを一個ずつ取り付けてください  

### トラックボールを取り付ける
![build](./img/build017.jpg)
![build](./img/build018.jpg)
![build](./img/build001.jpg)
![build](./img/build020.jpg)
- ボールホルダーにセラミックボール、コロ、PCBプレートを入れます  
- 中身がこぼれないようにボールホルダーをひっくり返し、キーボードにネジ止めします

### リセットスイッチ、電源スイッチ、電池ボックスをはんだ付けする
![build](./img/build014.jpg)
![build](./img/build013.jpg)
![build](./img/build015.jpg)
- リセットスイッチ、電源スイッチをはんだ付けします
- 電池ボックスを差し込み裏側からはんだ付けします。
  - なるべく電池ボックスの足が飛び出ないようにニッパーで切断してからはんだ付けしてください

### スペーサーを取り付ける
![build](./img/build021.jpg)
- 8mmのスペーサーをトッププレートの外周部にネジ止めします

### BLE Micro Proを取り付けて動作確認する
![build](./img/build016.jpg)
![build](./img/build019.jpg)
- BLE Micro ProにKugel用のファームウェアを書き込みます  
- BLE Micro ProのUSBコネクタ側に寄せてコンスルーを取り付けます。Pro Microと異なりはんだ付けは不要です  
- BLE Micro Proを裏向きでKugelに取り付けます  
- USBでパソコンに接続してキー入力ができることを確認してください

### ミドルプレート、ボトムプレートを取り付ける
![build](./img/build022.jpg)
![build](./img/build025.jpg)
![build](./img/build024.jpg)
- ミドルプレートをはめこみ、ボトムプレートをネジ止めします  
- ボトムプレートにゴム足を貼り付けます
- BLE Micro Proカバーを取り付けます
  - 構造上コンスルーと接触してカバーの端が浮く場合があります。気になる場合はコンスルーをはんだ付けした上でカットしてください 

### キーキャップを取り付ける
- スイッチにキーキャップを取り付けます

### トラックボールの位置を調整する
- トラックボールが反応するように取り付け位置を調整します  
  - ボールを回してもカーソルが動かなかったり特定の方向だけ効きが悪い場合は、ICの検出範囲とボールの位置が合うように位置調整が必要です
  - 固定ネジを少し緩めると取り付け位置を動かせます。操作したときの反応を見ながら位置を決めてネジをしっかり締め付けます
  - 調整しろが足りない場合にはトラックボールホルダー側の爪の端をカットして調整範囲を広げてください
