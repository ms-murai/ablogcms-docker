# ablogcms-docker

## dockerでの構築手順
https://developer.a-blogcms.jp/download/
<br>
から新規インストールパッケージをダウンロード
<br>
解凍後、
<br>
```acms3.1.22\acms3.1.22\ablogcms```
<br>
配下のものを```www```配下に入れる
```
www-index.php
   -setup
   -storage
   -themes
   -private
   -php
   -lang
   ...
```

以下のコマンドを実行します 
```bash
docker-compose up -d
```

hostsファイル編集、以下を追加
```
127.0.0.1 acms.lab
```


ブラウザでアクセスする
```
http://acms.lab
```

データべース設定
```
以下参照
https://h2ham.net/a-blog-cms-docker/
```