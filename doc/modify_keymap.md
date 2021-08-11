# modify keymap
こちらはHalfcliffのキーマップ変更用の資料です。(20210808時点で未完成)
キーマップの変更方法を記載しています。

キーマップの変更法は複数ありますが、本資料では、

* Remapを使用したキーマップ変更方法
* (準備中)keymap.cを直接編集してのキーマップ変更方法
* (準備中)VIAを使用したキーマップ変更方法

を記載します。

# Remapを使用したキーマップ変更方法
ここでは、Remapを使用したキーマップの変更方法を記載します。大まかな流れは以下の通りです。
* (行っていない場合)キーマップをviaに指定してファームウェア書込
* RemapのWebサイトへアクセス
* PCへのキーボードの接続
* Remapにてキーマップ変更用画面の表示
* キーマップの変更

# (行っていない場合)キーマップをviaに指定してファームウェア書込
Remapでのキーマップ変更には、 viaを指定したファームウェアがProMicroに書き込まれている必要があるため、行っていない場合はそれを行います。

具体的には、動作テスト時に行った
[入力動作テスト](https://github.com/N2-Sumikko/HalfCliff/blob/master/doc/Oparation_test_jp.md)
の内容に従い、
* (QMK MSYSを使用する場合）コマンド「qmk flash -kb halfcliff -km via」でのファームウェアの書込み
* (QMK Toolboxを使用する場合)ダウンロードした「HalfCliff-master」内の「hex/via/normal/halfcliff_via.hex」を使用してのキーマップ書込み
を行います。

# RemapのWebサイトへアクセス
[Remap](https://remap-keys.app/)へアクセスします。







