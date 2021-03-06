# Build Guide
こちらはHalfcliffのビルドガイドです。
基本セット(左右ProMicro基板＋左右キースイッチ基板＋左右JIS拡張基板）の組立方法を記載しています。

大まかな流れは以下の通りです。
*   同梱品の確認
*   別途必要な部品の準備、確認
*   左右ProMicro基板の組立
*   左右キースイッチ基板の組立
*   左右JIS拡張基板の組立
*   各基板の接続、ボトムプレートの取付け
*   動作確認

組立時点でオプションのトラックボールモジュール、ロータリーエンコーダ、OLEDの取付を想定している場合は、[オプション用の資料](https://github.com/N2-Sumikko/HalfCliff/blob/master/doc/option_jp.md)を作業前にご一読いただくと良いかと思います。(取付時にははんだ付けしないキースイッチ等があるため)

(遊舎工房様のレンタルボックス販売品(β版)をご購入いただいた方へ)
β版と正式版の大きな違いは以下の通りです。
*   右キースイッチ基板のアンダーグロー用LED取付済み(β版の基板は配線修正が必要なため)
*   左右キースイッチ基板の部品面(キースイッチを取付ける面)にもレジストあり(本来ははんだ付けする面のみ)
*   右キースイッチ基板にトラックボールモジュールを取付ける際の、変換基板へピンヘッダをはんだ付けする面が逆
*   価格(β版の方が上記の分正式版より安くなっています。）

# 同梱品の確認
各基板用の部品が揃っていることを確認します。

ねじやピンヘッダ、ピンソケット等は、各基板用のものをそれぞれ別の袋に梱包しています。

部品数は合計を記載しています。(例えば、左右の基板で1つずつ使用するなら2と記載)

文字だけではどの部品か分かりにくい場合は、組立の各手順の写真も参考にしてみてください。

M2x2mm中空スペーサー等、予備の部品が付属しているものもあります。

*   左右ProMicro基板用

|名前|部品数|概要|
|:-|:-|:-|
ProMicro基板|2|表にControl Boardと書かれた基板です。他基板と繋がっている事もあります。
1x9L字ピンソケット|4|黒色の、ピンがL字型をした９ピンのピンソケットです。樹脂部分の長さは8.5㎜です。
1x12ピンソケット|4|黒色の、12ピンのピンソケットです。樹脂部分の長さは5.7㎜です。
リセットスイッチ|2|ボタンがある四角い部品です。
2x4細ピンヘッダ(2mmピッチ)|2|2x4ピンの2mmピッチのピンヘッダです。
ジャンパピン(2mmピッチ）|4|内部に金属端子がある、黒色の四角い樹脂製の部品です。
TRRSジャック|2|TRRSケーブルを接続する穴がある四角い部品です。
1x4ロープロファイルピンソケット|2|4ピンの背が低いピンソケットです。
M2x2mm中空スペーサー|8|厚さ2mmのワッシャのような部品です。4つは予備です。
M2x8mmなべ小ねじ|4|銀色の長さ8㎜のねじです。
M2ナット|4|銀色の六角形の部品です。

*   左右キースイッチ基板用

|名前|合計数|備考|
|:-|:-|:-|
左キースイッチ基板|1|表にLeft Switch Boardと書いてある基板です。
右キースイッチ基板|1|表にRight Switch Boardと書いてある基板です。
トッププレート|2|四角い穴の開いた白色の基板のうち、一番大きいものです。
左ボトムプレート|1|アクリル製の透明な板のうち、二番目に大きいものです。
右ボトムプレート|1|アクリル製の透明な板のうち、一番大きいものです。
1x9L字ピンヘッダ|4|ピンがL字型をした9ピンのピンヘッダです。
ダイオード|50|リードタイプのダイオードです。
1x9ロープロファイルピンヘッダ|1|9ピンの背が低いピンヘッダです。
1x8ロープロファイルピンヘッダ|1|8ピンの背が低いピンヘッダです。
1x4ロープロファイルピンソケット|2|4ピンの背が低いピンソケットです。(オプション用)
M2x7mmスペーサー|12|円柱の形をした長さ７mmの部品です。
M2x4mmねじ|20|銀色の長さ4㎜のねじです。
M2x6mmなべ小ねじ|4|銀色の長さ6㎜のねじです。
ProMicroカバー|2|アクリル製の透明な板のうち、一番小さいものです。
ゴム足|8|透明なゴム足です。シートに貼り付けてあります。
LEDテープ|2|1枚当たり5つのLEDが付いたテープ状の部品です。

*   左右JIS拡張基板用

|名前|部品数|概要|
|:-|:-|:-|
左JIS拡張基板|1|表にLeft Extension Boardと書かれた基板です。他基板と繋がっている事もあります。
右JIS拡張基板|1|表にRight Extension Boardと書かれた基板です。
左JIS拡張基板用トッププレート|1|四角形の穴が開いた白色の基板のうち、一番小さいものです。
右JIS拡張基板用トッププレート|1|四角形の穴が開いた白色の基板のうち、二番目に大きいものです。
ダイオード|25|リードタイプのダイオードです。
1x8ロープロファイルピンヘッダ|1|8ピンの背が低いピンヘッダです。
1x9ロープロファイルピンヘッダ|1|9ピンの背が低いピンヘッダです。
ジャンパピン(2.54mmピッチ）|17|内部に金属端子がある、四角い樹脂製の部品です。（黒色ではないジャンパピンです。）
M2x7mmスペーサー|8|円柱の形をした長さ７mmの部品です。
M2x4mmなべ小ねじ|16|銀色の長さ4㎜のねじです。

# 別途必要な部品の準備、確認
以下の部品を用意します。

|名前|部品数|概要|
|:-|:-|:-|
pro micro|2|ProMicro、または互換品です。
ピンヘッダ1x12|4|12ピンのピンヘッダです。ProMicroの袋に同梱のものが使用可能です。
スタビライザー(2u用)|2|キースイッチのような部品2つが金属製のシャフトでつながった部品です。
キーキャップ|75|CherryMX互換品のキーキャップが必要です。例えば[これ](https://www.diatec.co.jp/shop/det.php?prod_c=4130)
キースイッチ|75|Cherry MX互換品が必要です。(余談)自分は[Kailh BOX Brown](https://shop.yushakobo.jp/collections/all-switches/products/kailh-box?variant=37665170456737)をよく使います。
microUSBケーブル|1|USBのType-A端子とmicroUSBのType-B端子を接続して通信可能なケーブルが必要です。
TRRSケーブル|1|TRRSジャックに接続するケーブルです。

# 組立に必要な工具の用意
Halfcliff組立て時に自分が使用したものを以下に記載します。
* はんだごて
* はんだこて台
* はんだ
* 簡易はんだ吸い取り機(ハッコースッポン 20Gを使用しました。)
* フラックス
* ピンセット
* マスキングテープ(キースイッチ等をはんだ付け時に固定する際に使用しました。)
* 精密ドライバー
* 大き目のクリップ(キースイッチのはんだ付け時に、キースイッチを基板に固定するために使用しました。)
* ニッパー
* 鉄やすり
* 瞬間接着剤(ピンソケットやピンヘッダの取付け時に任意で使用します。部品の樹脂部分にのみ少量だけ塗布して基板に接着します。金属部分にはつかないよう注意です。)
* ハックルー(ProMicroのモゲ対策として、エポキシ接着剤の代わりに使いました。)

他にも、こちらのサリチル酸様のWebページも非常に参考になるかと思います。(この場を借りて感謝申し上げます。)

[自作キーボードを作るために必要な工具 - 自作キーボード温泉街の歩き方](https://salicylic-acid3.hatenablog.com/entry/tool-lubrication)


# 組立時の主な注意点
* ProMicro基板の組立時、1x9L字ピンソケットの向きに注意してください。(後の手順で詳細を記載しています。)
* ダイオードをはんだ付けする際の向きに注意してください。
* はんだ付け時にキースイッチやピンソケット、ピンヘッダ等の部品が基板から浮かないように注意してください。
* ジャンパピンの取付位置に注意してください。
* LEDテープ等、はんだが乗りにくい部分には、フラックスを薄く塗布してからはんだ付けしてください。
* 部品の取外しのためにはんだの吸取りを行う場合、吸取りが不十分な状態で無理に部品を取外そうとすると、基板の銅箔がはがれることがあるので注意してください。

# 左右ProMicro基板の組立
左右ProMicro基板を組立てます。(つまり、各作業を2回行うことになります。)

おおまかな流れは以下の通りです。
* (ProMicro基板が他の基板と繋がっている場合)コントロール基板の切り離し
* (気になる場合)切り離したPromicro基板の整形
* 1x9L字ピンソケット2つのはんだ付け
* 1x4ロープロファイルピンソケットのはんだ付け
* 2x4ピンヘッダのはんだ付け
* 1x12ピンソケット2つのはんだ付け
* リセットスイッチのはんだ付け
* 2x4ピンヘッダへのジャンパピンの取付け
* TRRSジャックのはんだ付け
* ProMicroへの1x12ピンヘッダ2つのはんだ付け
* 1x12ピンソケットへのProMicroの取付け

画像は主に左基板のものですが、右の組立方法も殆ど同じです。

左右で組立手順が明らかに異なるものには、なるべく両方の画像を用意しています。
# (ProMicro基板が他の基板と繋がっている場合)コントロール基板の切り離し
ProMicro基板が他の基板と繋がっている場合、画像の様にニッパー等で切り離します。(以下、「画像の様に～」は基本的に省略します。)

あとで触ってケガしないよう、鋭い部分が残らないよう切り離してください。切り残しが基板の凹みより内側にあれば、組立て時に干渉はしません。
![IMG_20210613_101842](https://user-images.githubusercontent.com/54104281/122664449-6c9a6480-d1dc-11eb-82b1-c0d392597671.jpg)
切り離した後の基板
![ProMicro基板整形前](https://user-images.githubusercontent.com/54104281/122668801-d3c41300-d1f4-11eb-903c-23730a14e727.jpg)
# (気になる場合)切り離したPromicro基板の整形
切り残しが気になる場合は鉄ヤスリ等で削ります。
![ProMicro基板整形後](https://user-images.githubusercontent.com/54104281/122664522-f77b5f00-d1dc-11eb-895f-f90aabdbdf0d.jpg)
# 1x9L字ピンソケット2つのはんだ付け
基板に1x9L字ピンソケット2つを取付け、はんだ付けします。左右の基板で向きが異なるので注意してください。
![1x9L字ピンソケットはんだ付け後](https://user-images.githubusercontent.com/54104281/122664620-7a9cb500-d1dd-11eb-8fc7-6cf1ecd44526.jpg)
はんだ付けの流れとしては、まずはピンソケットの端子1つをはんだ付けします。

(画像では下のピンソケットの一番上のピンをはんだ付けしています。)
![1x9L字ピンソケット_1端子はんだ付け後](https://user-images.githubusercontent.com/54104281/122664693-eed75880-d1dd-11eb-94e4-877204e0cb77.jpg)
ピンソケットが基板から浮いていないことを確認します。画像の状態であればOKです。浮いている場合は、はんだを溶かしながら位置を調整します。
![1x9L字ピンソケット浮き確認](https://user-images.githubusercontent.com/54104281/122664713-10d0db00-d1de-11eb-8f03-969f75833915.jpg)

問題が無ければ残りの端子をはんだ付けします。

以下、はんだ付けする部品は同じように、浮いていないことを確認しながら取付けていきます。
# 1x4ロープロファイルピンソケットのはんだ付け
基板に1x4ロープロファイルピンソケットを取付け、はんだ付けします。
![1x4LPピンソケットはんだ付け後](https://user-images.githubusercontent.com/54104281/122664810-8dfc5000-d1de-11eb-8514-edcf17207d45.jpg)
# 2x4細ピンヘッダ(2mmピッチ)のはんだ付け
ピンの短い方が基板側となるように2x4細ピンヘッダ(2mmピッチ)を取付け、はんだ付けします。ピン同士がはんだでくっつかないように注意してください。

1x12ピンソケットの後のはんだ付けは大変なので、それより前にはんだ付けします。

(画像は1x12ピンソケットを先にはんだ付けしてしまった時のものです。出来なくはないですが、やっぱり大変でした。)
![2x4細ピンヘッダはんだ付け後_文字追加](https://user-images.githubusercontent.com/54104281/122665026-d405e380-d1df-11eb-85bc-78656980ddec.jpg)
#  1x12ピンソケット2つのはんだ付け
基板へ1x12ピンソケット2つを取付け、はんだ付けします。
![1x12ピンソケットはんだ付け後](https://user-images.githubusercontent.com/54104281/122665055-09123600-d1e0-11eb-9c8d-e9247a03453f.jpg)
# リセットスイッチのはんだ付け
基板へリセットスイッチを取付け、はんだ付けします。リセットスイッチに向きはありません。

![リセットスイッチはんだ付け後](https://user-images.githubusercontent.com/54104281/122665076-29da8b80-d1e0-11eb-984f-df885c01b4f1.jpg)
# ジャンパピンの取付け
はんだ付けしたピンヘッダへジャンパピンを取り付けます。画像の赤枠の位置に取付けてください。
![ジャンパピン取付後_赤枠追加後](https://user-images.githubusercontent.com/54104281/122859792-86ac8200-d357-11eb-854a-9757c55c339a.jpg)

(余談)ジャンパピンの位置を変更し、マスタ側の抵抗用のランドに4.7kΩ抵抗2つをはんだ付けすることで、左右のキーボード間の通信をI2Cで行うこともできます。

ただし、通信をI2Cで行う場合、ファームウェアの変更が必要となります。方法を知っている方向けです。(需要があれば詳細を追記するかもです。)
# TRRSジャックのはんだ付け
基板へTRRSジャックを取付け、はんだ付けします。左右の基板で取付場所が異なるので注意してください。

…といっても、順番通り組立てれば、使用しない取付場所は1x9L字ピンヘッダで塞がれるので問題無いはずです。
![TRRSジャックはんだ付け後](https://user-images.githubusercontent.com/54104281/122665426-16c8bb00-d1e2-11eb-80a4-07c40dc649c5.jpg)
# ProMicroへの1x12ピンヘッダ2つのはんだ付け
ProMicroへ1x12ピンヘッダ2つをはんだ付けします。画像を見ながら、ProMicroの表裏、ピンヘッダの向きに注意してはんだ付けしてください。

言葉で説明すると、ProMicroの部品が無い面を上にした状態で、ピンヘッダの長い方がProMicro側、かつピンヘッダの樹脂部分がProMicroの部品がある面に来るようにはんだ付けします。

また、HalfCliffではコンスルーは使用しませんので注意してください。
![1x12ピンヘッダはんだ付け後](https://user-images.githubusercontent.com/54104281/122665461-4d063a80-d1e2-11eb-9f31-617e12d4df32.jpg)
できればここでProMicroのUSB端子のモゲ対策をしておくとよいです。(「ProMicro もげ」等で検索するとサイトが色々出てきます。)

はんだ付け後、はんだ付けした側のピンが短くなるように、ニッパー等で切り落とします。切り落とさないと、後で取付けるProMicroカバーにピンが干渉します。
![ピンヘッダ切り落とし後](https://user-images.githubusercontent.com/54104281/122665708-c18da900-d1e3-11eb-8b37-7e2d22927f1b.jpg)
# 1x12ピンソケットへのProMicroの取付け
　ProMicroをピンソケットへ取付けます。
 ![ProMicro取付後](https://user-images.githubusercontent.com/54104281/122665744-044f8100-d1e4-11eb-8690-c6bfbd4ea3f8.jpg)
以上でProMicro基板の組立は完了です。
# 左右キースイッチ基板の組立
左右のキースイッチ基板を組立てます。(つまり、各作業を2回(ry)

おおまかな流れは以下の通りです。
* ダイオードのはんだ付け
* 1x9L字ピンヘッダ2つのはんだ付け
* 1x4ロープロファイルピンソケットのはんだ付け
* 1x8(右は1x9)ロープロファイルピンヘッダのはんだ付け
* ProMicro基板とキースイッチ基板の接続
* 左右キースイッチの入力動作テスト
* 四隅のキースイッチの取付け、はんだ付け
* 残りのキースイッチの取付け、はんだ付け
* 左キースイッチ基板のLEDテープの貼付け、はんだ付け
* 右キースイッチ基板のLEDテープの貼付け、はんだ付け
* M2x7mmスペーサー4つの取付け
* スペーサーのトッププレートへのねじ止め

# ダイオードのはんだ付け
左右のキースイッチ基板にリードタイプのダイオードを取付け、はんだ付けします。

ダイオードは左右で各25個、合計50個使用します。

まずは50個のダイオードのリードを曲げます。リードを根本付近で曲げれば、基板へ取付可能な状態になります。
![曲げたダイオード](https://user-images.githubusercontent.com/54104281/122665890-1120a480-d1e5-11eb-8f0e-424067bb2186.jpg)
リードを曲げたらダイオードの黒色の部分と、基板のシルクの横線の向きを合わせて取付けます。5個ずつくらい行っていくとよいです。

(余談)Halfcliffではんだ付けを行う基板はすべて一層(片面)基板なので、本来レジスト(はんだ付けを行う面に塗られる色がついた保護膜)は片面のみです。
ですが、初回注文時の左右キースイッチ基板は何らかの理由でレジストが両面にある状態になってしまいました。
ビルドガイドでは初回注文時の基板を撮影しているので、ちょっと赤色がきつくてシルクが見づらいです。ごめんなさい。
![ダイオードの向き判別用](https://user-images.githubusercontent.com/54104281/122665942-4fb65f00-d1e5-11eb-9e8f-7c27b0076c27.jpg)
右キースイッチ基板のダイオード2つのみ、ほかのダイオードと異なる場所にあるので注意してください。(画像の黄枠の部分です。)
![右キースイッチ基板のダイオード位置注意用](https://user-images.githubusercontent.com/54104281/122666097-4c6fa300-d1e6-11eb-96e7-b451fe21232e.jpg)
取付けが完了したらはんだ付けをします。はんだ付け後、不要なリードをニッパーなどで切り落とします。

画像は参考として、左キースイッチ基板の右端の5個だけダイオードをはんだ付けし、リードをカットした時の裏面です。
![左キースイッチ基板_ダイオードリードのカット後](https://user-images.githubusercontent.com/54104281/122666192-d3bd1680-d1e6-11eb-848c-17bd2453e605.jpg)
この作業を50個のダイオードに対して行います。完了後の状態は下の画像を参考にしてください。
![左キースイッチ基板_ダイオード取付後](https://user-images.githubusercontent.com/54104281/122666217-07983c00-d1e7-11eb-9ccc-00763ef166b7.jpg)
![右キースイッチ基板_ダイオード取付け後](https://user-images.githubusercontent.com/54104281/122666220-0cf58680-d1e7-11eb-9e3e-0df18b089623.jpg)

# 1x9L字ピンヘッダ2つのはんだ付け
基板に1x9L字ピンヘッダ2つを取付け、はんだ付けします。L字ピンヘッダの取付け向きに注意してください。

言葉で説明すると、基板の表(HalfCliffと書いてある面)を上から見た時にL字ピンヘッダの樹脂部分の細長い方の面が見えるように、かつピンヘッダの端子が基板の外に向くように取付けます。
![左キースイッチ基板_1x9L字ピンヘッダ取付後](https://user-images.githubusercontent.com/54104281/122666300-665db580-d1e7-11eb-85ee-4ef8de620992.jpg)
# 1x4ロープロファイルピンソケットのはんだ付け
左右キースイッチ基板に1x4ロープロファイルピンソケットを取付け、はんだ付けします。
![左キースイッチ基板_1x4LPピンソケットはんだ付け後](https://user-images.githubusercontent.com/54104281/122666492-817cf500-d1e8-11eb-8057-4a6e75d1c5dc.jpg)
# 1x8(右は1x9)ロープロファイルピンヘッダのはんだ付け
左キースイッチ基板に1x8ロープロファイルピンヘッダ、右キースイッチ基板に1x9ロープロファイルピンヘッダを取付け、はんだ付けします。

ピンヘッダの短い方が基板側になるように取付けてください。

はんだ付け後の左キースイッチ基板
![左キースイッチ基板_1x8LPピンヘッダはんだ付け後](https://user-images.githubusercontent.com/54104281/122860321-78ab3100-d358-11eb-9330-e156e74a1034.jpg)
右キースイッチ基板
![右キースイッチ基板_1x9LPピンヘッダはんだ付け後](https://user-images.githubusercontent.com/54104281/122860354-8660b680-d358-11eb-9e56-faba18cbf504.jpg)
# ProMicro基板とキースイッチ基板の接続
動作テストのために、左右のProMicro基板のピンソケットと、キースイッチ基板のピンヘッダを接続します。
![左キースイッチ基板_ProMicro基板接続後](https://user-images.githubusercontent.com/54104281/122666556-e6384f80-d1e8-11eb-8efd-85b6aff607dc.jpg)
# 左右キースイッチ基板の動作テスト
左右キースイッチ基板の動作テストはこのタイミングか、キースイッチのはんだ付け後に行うのがおすすめです。
(キースイッチはんだ付け後に行う時は、問題発生時の原因がキースイッチにある可能性も考慮します。）

動作テストの手順は以下のリンクに記載しています。
[入力動作テスト](https://github.com/N2-Sumikko/HalfCliff/blob/master/doc/Oparation_test_jp.md)
# ProMicro基板とキースイッチ基板の分離
動作確認完了後、組立進行のためにProMicro基板とキースイッチ基板を分離します。
# トッププレートへのM2x7mmスペーサーの取付け
左右のトッププレートへM2x7mmスペーサーを、M2x6mmねじで取付けます。

左右のトッププレートで取付け向きが異なるので注意して下さい。
数は左右で各2つ、合計4つです。後から取付けるのは大変なので、なるべく忘れずに取付けてください。
![トッププレート_スペーサー取付後](https://user-images.githubusercontent.com/54104281/122666597-3b746100-d1e9-11eb-8eaa-d85c7327f6b3.jpg)
# 四隅のキースイッチの取付け、はんだ付け
まずはトッププレートの四隅へキースイッチを取付けます。

その後、トッププレートを取付けたキースイッチを、キースイッチ基板に取付けます。
![左キースイッチ基板_四隅キースイッチ取付後](https://user-images.githubusercontent.com/54104281/122666664-aa51ba00-d1e9-11eb-9100-20fd72f15f99.jpg)
取付け時に、キースイッチのピンが基板の穴に正しく入っていることを確認してください。入っていない場合は、ピンが曲がっていないか等を確認します。

正しく取付けたら、いずれか1つのキースイッチの片方のピンを、キースイッチ基板から浮かないようにはんだ付けします。

例えば画像の左下のキー等、正方形以外の穴に取付けるキースイッチは、比較的浮きやすいので注意してください。
![左キースイッチ基板_四隅キースイッチ取付後_注意書き](https://user-images.githubusercontent.com/54104281/122666805-762ac900-d1ea-11eb-9193-975f6243e704.jpg)

キースイッチを固定する際は、マスキングテープで固定したり、大き目のクリップで基板とキースイッチを挟むといった方法がおすすめです。

端子とパッド間は十分な量のはんだではんだ付けしてください。(画像くらいの量なら大丈夫です。)
![はんだの量目安](https://user-images.githubusercontent.com/54104281/122666946-2e587180-d1eb-11eb-9957-650596c44d5b.jpg)

はんだ付け後、キースイッチが浮いていないことを確認します。浮いている場合は修正します。

確認後、もう片方のピンをはんだ付けします。

同様の作業を、残り3つのキースイッチに対しても行います。
![左キースイッチ基板_四隅キースイッチはんだ付け後](https://user-images.githubusercontent.com/54104281/122666971-5516a800-d1eb-11eb-9bc0-4b2498c21a3b.jpg)
# 残りのキースイッチの取付け、はんだ付け
残りのキースイッチを取付け、はんだ付けします。
![左キースイッチ基板_キースイッチはんだ付け後](https://user-images.githubusercontent.com/54104281/122667004-7f686580-d1eb-11eb-8ee0-b2c35930f6dc.jpg)
# 左キースイッチ基板のLEDテープの貼付け、はんだ付け
まずはLEDテープ裏面のシールをはがします。

その後、画像を参考にLEDテープの向きを合わせます。
![IMG_20210619_123149](https://user-images.githubusercontent.com/54104281/122667045-bf2f4d00-d1eb-11eb-9260-d18a7040e9b3.jpg)

言葉で説明すると、

・基板のGNDとLEDテープの-

・基板のTXとLEDテープのDI

・基板のVCCとLEDテープの+5V

を合わせます。

LEDテープの向きを合わせたら、左キースイッチ基板へLEDテープを貼付けます。

貼付け後、LEDテープの端子にフラックスを塗布し、はんだ付けします。

![左キースイッチ基板_LEDテープはんだ付け後](https://user-images.githubusercontent.com/54104281/122667255-dc185000-d1ec-11eb-9a48-c0d95a3f5e27.jpg)

# (基板のバージョンで組立内容が変わります。)右キースイッチ基板のLEDテープの貼付け、はんだ付け
右キースイッチ基板のLEDテープの貼付けは、基板のバージョンによって作業内容が変わります。基板のバージョンは基板の表面にシルクで「Ver～～」と印刷されています。

バージョンが1.01以降の場合は、左キースイッチ基板と同じ手順(基板のシルクとLEDテープの文字を対応させる)で貼付け、はんだ付けをします。

バージョンが1.0(β版)の場合は、右キースイッチ基板のパターンミスのせいで、左キースイッチ基板と同じ手順ではLEDテープは動作しません。
対応として、LEDテープが動作するように配線を追加した右キースイッチ基板に、LEDテープをはんだ付け済みのものを販売しています。そのため作業は不要です。

# M2x7mmスペーサー4つの取付け
キースイッチ基板へM2x7㎜スペーサー4つを取付けます。
取付位置は画像を参考にしてください。

(画像は右キースイッチ基板のものですが、左キースイッチ基板も位置は同じです。)
![右キースイッチ基板_M2x7mmスペーサー取付後](https://user-images.githubusercontent.com/54104281/122667441-df600b80-d1ed-11eb-8324-d8cb590e8f6a.jpg)
# スペーサーのトッププレートへのねじ止め
M2x7mmスペーサーをトッププレートにM2x4mmねじでねじ止めします。スペーサーを落とさないように注意してください。
![左キースイッチ基板_M2x7mmスペーサーねじ止め後](https://user-images.githubusercontent.com/54104281/122667384-a162e780-d1ed-11eb-804c-efc212a28768.jpg)
以上でキースイッチ基板の組立は完了です。
![左右キースイッチ基板組立完了後](https://user-images.githubusercontent.com/54104281/122667463-f56dcc00-d1ed-11eb-9410-6f2ac8a1a307.jpg)

次は左右のJIS拡張基板を組立てます。

# 左右のJIS拡張基板の組立
左右のJIS拡張基板を組立てます。(つまり、各(ry)

おおまかな流れは以下の通りです。
* (左JIS拡張基板が他の基板と繋がっている場合)他の基板と繋がっていた部分の整形、やすりがけ
* ダイオードのはんだ付け
* 1x8(右は1x9)ロープロファイルピンヘッダのはんだ付け
* (右のみ)スタビライザーの取付け
* トッププレートへのキースイッチ(四隅）の取付け、はんだ付け
* 残りのキースイッチの取付け、はんだ付け
* M2x7mmスペーサー4つの取付け
* スペーサーのトッププレートへのねじ止め
* ボトムプレートへのゴム足の取付け
* キーキャップの取付け
* 組立後の動作確認

# (左JIS拡張基板と他の基板が繋がっている場合)他の基板と繋がっていた部分の整形、やすりがけ
他の基板と繋がっていた部分を、ProMicro基板の時と同じように、鋭い部分が残らないように切り離します。
![左JIS拡張基板整形後](https://user-images.githubusercontent.com/54104281/122667563-60b79e00-d1ee-11eb-80e5-b2a6e6a389c6.jpg)
# ダイオードのはんだ付け
リードタイプのダイオードをキースイッチ基板に取付け、はんだ付けします。

ダイオードは左基板10個、右基板15個、合計25個使用します。

手順はキースイッチ基板の時と同様ですが、向きがキースイッチ基板とは逆なので注意してください。

ダイオードの黒色の部分と、基板のシルクの横線との向きを揃えればOKです。
# 1x8(右は1x9)ロープロファイルピンヘッダのはんだ付け
左基板に1x8ロープロファイルピンヘッダ、右基板に1x9ロープロファイルピンヘッダを取付け、はんだ付けします。

ピンヘッダの短い方が基板側になるように取付けてください。
![右JIS拡張基板_1x8LPピンヘッダはんだ付け後](https://user-images.githubusercontent.com/54104281/122667643-d28fe780-d1ee-11eb-9c14-fdfad900ffd1.jpg)
![左JIS拡張基板_1x9LPピンヘッダはんだ付け後](https://user-images.githubusercontent.com/54104281/122667668-f05d4c80-d1ee-11eb-9af2-c4cf0f3c59e2.jpg)
#  (右のみ)スタビライザーの取付け
右JIS拡張基板にスタビライザー2つを取付けます。

ルブの用意がある場合は、スタビライザーへのルブを塗布してから取付けます。

ルブの塗布に関しては、こちらのサリチル酸様のWebページが非常に参考になるかと思います。(この場を借りて重ねて感謝申し上げます。)

[スタビライザーのルブの話](https://salicylic-acid3.hatenablog.com/entry/stabilizer-lubrication)

![右JIS拡張基板_スタビライザー取付後](https://user-images.githubusercontent.com/54104281/122667691-0e2ab180-d1ef-11eb-9d07-a17d9102224d.jpg)
# トッププレートへのキースイッチ(四隅）の取付け、はんだ付け
キースイッチ基板の時と同様、トッププレートの四隅へキースイッチを取付け、はんだ付けします。
![左JIS拡張基板_四隅キースイッチはんだ付け後](https://user-images.githubusercontent.com/54104281/122667737-5ea20f00-d1ef-11eb-8600-5f0569463756.jpg)
# 残りのキースイッチの取付け、はんだ付け
キースイッチ基板の時と同様、残りのキースイッチを取付け、はんだ付けします。
![左JIS拡張基板_キースイッチはんだ付け後](https://user-images.githubusercontent.com/54104281/122667734-5a75f180-d1ef-11eb-9225-98945e0fc8ce.jpg)
# JIS拡張基板へのM2x7mm スペーサー4つの取付け
JIS拡張基板へM2x7mmスペーサー4つ(左右で合計8個)を取付けます。
![左JIS拡張基板_M2x7mmスペーサー取付後](https://user-images.githubusercontent.com/54104281/122667793-a32daa80-d1ef-11eb-85b4-dff0ac5ba902.jpg)
![右JIS拡張基板_M2x7mmスペーサー取付後](https://user-images.githubusercontent.com/54104281/122936934-87233800-d3ac-11eb-8756-ca180a3ee67e.jpg)

この時点ではスペーサーは固定されていないので、落とさないよう注意してください。
# スペーサーのトッププレートへのねじ止め
スペーサーをトッププレートへM2x4mmねじでねじ止めします。

以上で左右の拡張基板の組立は完了です。
![左JIS拡張基板_完成後](https://user-images.githubusercontent.com/54104281/122667847-028bba80-d1f0-11eb-8558-310b7c70d2b7.jpg)
![右JIS拡張基板_完了後](https://user-images.githubusercontent.com/54104281/122667843-fc95d980-d1ef-11eb-9c14-c0f38b1a9a60.jpg)
最後に、各基板を連結し、ボトムプレートを取付けます。
# 各基板の接続、ボトムプレート、ProMicroカバーの取付け
各基板を接続し、ボトムプレートを取付けます。(つまりry

おおまかな流れは以下の通りです。
* ボトムプレートへのProMicro基板の仮止め
* ProMicro基板とキースイッチ基板の接続
* ボトムプレートへのキースイッチ基板の仮止め
* ボトムプレートへのJIS拡張基板の仮止め
* キースイッチ基板とJIS拡張基板のピンヘッダへのジャンパピンの取付け
* ボトムプレートと各基板のねじ止め
* キースイッチ基板のトッププレートへのProMicroカバーのねじ止め
# ボトムプレートへのProMicro基板の仮止め
ボトムプレートの保護シートをはがします。

その後、ボトムプレートへProMicro基板をM2x8mmねじ2本とM2x2mm中空スペーサー2つ、M2ナット2つを使用して2箇所を仮止め(ガタがある程度にねじ止め)します。
![ボトムプレート_ProMicro基板仮止め後](https://user-images.githubusercontent.com/54104281/122667886-3ebf1b00-d1f0-11eb-802b-d4c8a5bb5e9c.jpg)
仮止めするのは、後の手順で基板の位置を微調整する可能性があるためです。

ねじ止め可能な個所は3箇所ありますが、基本的には画像と同じ場所を使用するとよいです。
![ProMicro基板ねじ止め位置説明用](https://user-images.githubusercontent.com/54104281/122667973-b8ef9f80-d1f0-11eb-9c57-cb0750f12cc7.jpg)
部品の順番を言葉で説明すると、下から上に、M2x8mmねじの頭、ボトムプレート、M2x2㎜中空スペーサー(真鍮色の部品)、ProMicro基板、M2ナットの順になります。

文章だとわかりにくいので、画像も参考にしてください。
![ProMicro基板ねじ止め時の部品順説明用](https://user-images.githubusercontent.com/54104281/122667940-847be380-d1f0-11eb-82ab-1e7180eaaf68.jpg)
ProMicroのUSB端子の下の穴にナットを止めにくい場合は、一度ProMicroを取り外すとよいです。

その際は、ProMicroの端子が曲がらないように注意します。ProMicroの中心付近をもってまっすぐ引き抜くとよいです。

# ProMicro基板とキースイッチ基板の接続
動作テストの時と同様、ProMicro基板とキースイッチ基板を接続します。

ProMicro基板にボトムプレートを仮止めしてあるので、キースイッチ基板がボトムプレートに乗る形になります。
![ボトムプレート_右キースイッチ基板接続後](https://user-images.githubusercontent.com/54104281/122668111-84c8ae80-d1f1-11eb-90a2-8bf89308637d.jpg)
# ボトムプレートへのキースイッチ基板の仮止め
ボトムプレートへキースイッチ基板をM2x4mmねじ4本で仮止めします。
# ボトムプレートへのJIS拡張基板の仮止め
JIS拡張基板をボトムプレートにM2x4mmねじ4本で仮止めします。
![IMG_20210619_180809](https://user-images.githubusercontent.com/54104281/122668139-a32eaa00-d1f1-11eb-8b78-229cd61218de.jpg)
# キースイッチ基板とJIS拡張基板のピンヘッダへのジャンパピンの取付け
キースイッチ基板とJIS拡張基板のピンヘッダが隣り合うようにそれぞれの基板の位置を微調整し、ピンヘッダの各ピンを橋渡しするように、ジャンパピンを取付けます。
一番下のピンから上に、一つずつ取付けていくとよいです。
![左基板_ジャンパピン取付後](https://user-images.githubusercontent.com/54104281/122668205-fe609c80-d1f1-11eb-9667-0582de9b5016.jpg)

この時、キースイッチの種類によってはキースイッチ(の羽のような部分)とジャンパピンが干渉する事があります。

その場合は、該当箇所をニッパー等で切断します。その際は、ピンヘッダのピンを切断しないよう注意します。

![ジャンパピン取付け時のキースイッチ干渉部分への対応](https://user-images.githubusercontent.com/54104281/122668414-edfcf180-d1f2-11eb-8a52-c4f2478d49c5.jpg)
# ボトムプレートと各基板のねじ止め
ボトムプレートへ仮止めした各ねじを本締めします。

ProMicro基板のねじは、M2のナットが空転しないようにピンセット等で押さえながら本締めすると良いです。

# キースイッチ基板のトッププレートへのProMicroカバーのねじ止め
キースイッチ基板へ取付けてあるM2x7mmスペーサーに、ProMicroカバーをM2x4mmねじ2本でねじ止めします。
![左基板_ProMicroカバーねじ止め後](https://user-images.githubusercontent.com/54104281/122668549-93b06080-d1f3-11eb-9298-bfc938806837.jpg)

(補足)もしM2x7mmスペーサーの取付けを忘れている場合は、M2x3㎜スリムヘッド小ねじを入手し、基板とトッププレートの間からそのねじを入れ、M2x7mmスペーサー2つをねじ止めした後、M2x6㎜ねじでProMicroカバーをねじ止めします。
# ボトムプレートへのゴム足4つの取付け
ボトムプレートの四隅へゴム足を取付けます。
![ゴム足取付後](https://user-images.githubusercontent.com/54104281/123529102-4c146200-d728-11eb-9bd5-fe993c060dcb.jpg)

# キーキャップの取付け
各キースイッチへお好みのキーキャップを取付けます。
Halfcliffの基本キットの場合、JIS配列のキーキャップが使用可能です。

一番下の行等に使用する1uのキーキャップが足りない場合、ファンクションキー等のキーキャップを逆向きにして代用するとよいです。

他には、無刻印キーキャップの使用もおすすめです。
![キーキャップ取付後(トリミング後)](https://user-images.githubusercontent.com/54104281/125184713-0b096b00-e25b-11eb-8237-5f4d2a286bc4.jpg)

# 組立後の動作確認
組立完了後、キースイッチ基板のみで行った時と同様の手順で動作確認を行います。

動作確認が完了したら、組立完了です。おつかれさまでした。

使用する[ファームウェアの書込み](https://github.com/N2-Sumikko/HalfCliff/blob/master/doc/modify_keymap.md)後、必要に応じてキーマップを変更し、楽しいキーボードライフをお過ごしください。

