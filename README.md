# pic_collector
Twitter APIとTwythonを使用して，特定のTwitterアカウントから写真をダウンロードするプログラムです。
ほとんどコピペだけど。

各種ファイルの説明と，環境の構築方法は以下から。

## 環境要件
Python 2系
Unix/Linux系OS（Windows環境では試していません）

# 概要
## main.py
Twitterの特定アカウントの写真を自動で取得するスクリプト。

実行方法
```
$ python main.py
```

## params.py
パラメータを記述する。
保存先ディレクトリの設定，取得するTweetの数を設定する。
ディレクトリの初期設定は
```
./images/
```


取得するツイートは，PAGEとTWEET_PER_PAGEの積算値を使用する。

## keys.py
使用するTwitter APIのキーを記述するファイル

## screen_names.py
取得したいTwitterのIDを記述する。一行につき一人。「@」はあってもなくても良い。

例：



screen_names = \`\`\`

@hello

good_evening

\`\`\`



# Twitter APIのキー取得方法
参考にさせていただきました。

[Twitter Apps | Twitter](https://apps.twitter.com/ "Twitter API")

[Twitter API Key を取得する方法 | phiary](https://phiary.me/twitter-api-key-get-how-to/)

# pyenvの設定
参考にさせていただきました。

[pyenvの使い方とインストール  | Python-izm](https://www.python-izm.com/tips/pyenv/)


# 参考にしたサイト
[Python2.7でTwitterタイムラインの画像を自動収集してみる | Qiita](https://qiita.com/imenurok/items/78d25e892c6557d24810)

[[Python] Twitterの画像を一括でダウンロードするスクリプト | Yura YuWite](http://yu-write.blogspot.jp/2014/01/python-twitter.html)
