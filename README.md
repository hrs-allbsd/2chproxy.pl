

# 導入方法

ubuntu14.04LTS の場合。

### 事前に必要なパッケージを導入。

`  sudo apt-get install git  libhttp-daemon-perl liblwp-protocol-https-perl`

### インストール

`  git clone https://github.com/yama-natuki/2chproxy.pl.git`

# 設定

 2chproxy.pl 内を参照。

# 起動方法

　_2chproxy.pl_ というディレクトリが作成されるので、その中の **2chproxy.pl** を直接起動させるもよし、_~/bin/_ 等にコピーして使うもよし。

　同梱の **jd.sh** はJDを起動する前に **2chproxy.pl** を起動させるシェルスクリプト。

　使う場合は、

```
    PROXY="$HOME/bin/2chproxy.pl"  
    JD="/usr/bin/jd"
```

の二つを自分の環境に合わせて変更。

# JDの設定

　設定→ネットワーク→プロキシ で2ch読み込み用のみ設定する。書き込みはプロキシを使用しない。

　また場合によっては高度な設定で 2chにアクセスするときのエージェント名や、2chのクッキーを見直す。
