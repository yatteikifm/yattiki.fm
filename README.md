# yatteikifm.github.io

https://yatteikifm.github.io のソースコード。

## 会話の収録方法

### Skype

https://www.skype.com/ja/

音声通話には音質を優先してSkypeを利用する。

### Soundflower

https://github.com/mattingalls/Soundflower/releases/

macOS用の仮想オーディオデバイス。LadioCastと組み合わせて利用する。

### LadioCast

https://itunes.apple.com/jp/app/ladiocast/id411213048?mt=12

macOS用のソフトウェアミキサー。Soundflowerと組み合わせて、マイクの入力とmacOSの出力をミックスするのに使う。

![image](https://pbs.twimg.com/media/Cv7fUPDUMAAyeYv.jpg:orig)

### QuickTime Player

録音用のアプリ。macOCに最初からインストールされている。

### Audacity

http://www.audacityteam.org/

QuickTime Playerで録音した .m4a 形式のファイルを読み込み、.mp3 形式で書き出す。
GitHubは通常は100MB以下のファイルしか配置できないので、ビットレート90kbps以下程度で書き出すと良さ気。

### Lame for Audacity

http://lame.buanzo.org/

Audacityで読み込んだファイルを .mp3 形式のファイルに書き出すのに必要なプラグイン。

## サイトの編集方法

### 記事の追加方法

1. `_posts/2016-10-30-yatteiki-first.md` のようなパターンでMarkdownファイルを配置する
1. 音源は `audio/2016-10-30-yatteiki-first.mp3` のようなパターンでMP3ファイルを配置する
1. `gh-pages` ブランチにpushすると https://yatteikifm.github.io/ に配置される

### ローカルでの確認方法

1. Ruby 2.2 以上をインストールする
1. `git clone git@github.com:yatteikifm/yatteikifm.github.io.git`
1. `cd yatteikifm.github.io`
1. `bundle install` で依存ライブラリをインストールする
1. `bundle exec jekyll serve` でサーバを立ち上げる
1. http://localhost:4000/ にWebブラウザでアクセスする

### 注意点

- 未来の日付の記事は表示されない
- 通常のMarkdownにはない特殊な記法が幾つかあるので、既存のファイルを参考にすること
