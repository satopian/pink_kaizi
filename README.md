# POTI-board用テーマPINK 改二

**[POTI-board改二](https://github.com/satopian/poti-kaini)用のテンプレートです。**

**「POTI-board改」と「POTI-board改二」のテンプレートは互換性がありません。**

間違えると掲示板が動作しなくなりますのでご注意ください。

POTI-board改はサポートを終了し改二に移行しました。
新規設置を検討されている方は、より高速に動作する[POTI-board改二](https://github.com/satopian/poti-kaini)の利用をご検討ください。

## サポート

[POTI改設置サポート掲示板](https://pbbs.sakura.ne.jp/cgi/neosample/support/)で対応します。
GitHubの[Issues](https://github.com/satopian/pink_for_pot-kaini/issues)でも対応できると思います。

### 設置サンプル

[POTI-board用テーマ PINK 設置サンプル](https://pbbs.sakura.ne.jp/cgi/neosample/poti/)

### 特徴

[お絵かき掲示板](https://pbbs.sakura.ne.jp/)交流サイトで使っているテンプレートを一般配布用にカスタマイズしたものです。

[POTI-board用テーマ PINK を配布します。: STP^3](http://stp.sblo.jp/article/182310034.html)

BBSNoteのようなレイアウト。

スマートフォン・タブレットに対応したレスポンシブデザイン。

お絵かき掲示板に特化したアップロード機能が無いテーマとして配布してきましたが  
POTI-board改二v2.8.0以後のバージョンでは「画像アップロード機能を 使う 使わない」を選択できるため画像アップロード機能にも対応しました。

従来と同じように「お絵かき掲示板」としてのみ使いたい時は  
config.phpで以下のように設定します。  

>//画像アップロード機能を 使わない:0 使う:1   
>define('USE_IMG_UPLOAD','0');  

>//画像のないコメントのみの新規投稿を拒否 しない:0 する:1   
>define('DENY_COMMENTS_ONLY', '1');  

なぜコメントのみの投稿も拒否するのかというと画像がないテキスト掲示板になるかもしれないからです。  
またこの設定ならお絵かきの無いテキストのみの投稿を行うスパムbotを弾く事ができるかもしれません。(新規投稿の場合）    

### このテーマを使うために必要なもの

お絵かき掲示板のスクリプト本体、[POTI-board改二](https://github.com/sakots/poti-kaini)をダウンロードします。

### このテーマのダウンロード 

**緑色の「Code」ボタンを押下してpink_for_pot-kaini-master.zipを入手します。**

### テーマを入れ替える前に ##

テーマを入れ替える前に、掲示板が問題なく動作することを確認します。

### サーバへの転送

> //テーマ(テンプレート)のディレクトリ。'/'まで  
> //themeディレクトリに使いたいtemplateをいれて使ってください。(推奨)  
> //別のディレクトリにしたい場合は設定してください。  
> //例えばおまけのnee2を使いたい場合はtheme_nee2/とすることができます。初期値は theme/ です。  

config.phpを編集します。

例えば

> define('SKIN_DIR', 'pink/');

の場合。

![Screen-2020-05-27_15-35-53](https://user-images.githubusercontent.com/44894014/83000244-0ed13280-a045-11ea-92f1-37c6d6238a72.png)

↑
ダウンロードしたpotiboard2フォルダに、ダウンロードしたpinkフォルダを追加します。


![Screen-2020-05-27_18-09-37](https://user-images.githubusercontent.com/44894014/83000458-5c4d9f80-a045-11ea-8a31-94ce1f2df273.png)

↑
その中に入っているファイル。


> define('SKIN_DIR', 'pink/');

と設定したので、 pink/ ディレクトリのテーマが適用されます。

**pinkディレクトリを転送します。**

掲示板が表示されたら設置完了です。

テーマを変更しても表示が変わらない時は、管理画面からログ更新するかなんでもいいので書き込みます。

### 履歴
#### [2020/10/08] lot.201008
POTI-board改二 v2.18.3に対応しました。  
`//画像なしのチェックボックスを使用する する:1 しない:0`    
` define('USE_CHECK_NO_FILE', '0');`  
で、画像なしのチェックボックスの表示非表示を切り替える事ができます。  

#### [2020/10/06] lot.201006

カタログモードの画像のaltとtitleがおかしかったのを修正しました。  
添付画像をエクスプローラーから選ぶ時にjpeg/gif/pngだけ表示するようにしました。  
これまではPSDファイルも表示されていました。

#### [2020/09/22] lot.200922

投稿ボタン2度押しによるトラブルの回避のためjQueryを使ったスクリプトを追加しました。

#### [2020/09/17] lot.200917

レスでお絵かきするときもパレットデータファイル切り替えができるようになりました。  
search.htmlの反復処理が入れ子になっていたのを修正しました。  

#### [2020/09/02] lot.200902

パレットデータファイル切り替え機能に対応しました。

#### [2020/08/30] lot.200830

iPadなどのタブレット端末、例えばviewportの解像度横幅768pxの時に横幅750px以上の画像を表示すると横スクロールがでるのを修正しました。

#### [2020/07/28] lot.200728

画像アップロード機能を使う使わないを選択できるようになった改二v2.8.0に対応しました。  
画像アップロード機能が使えるようになりました。アップロード機能なしにする事もできます。    

#### [2020/07/16] lot.200716

POTI-board改二 v2.7.6に対応。名前からのリンクは作者のイラスト一覧になりました。
