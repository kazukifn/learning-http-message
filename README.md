# HTTPでやりとりする仕組み

<!-- Markdown記法のヒント

コード記法（1行の中に埋めたい場合）

`code`

コードブロック記法（複数行）

```
print('a')
print('b')
```

-->

## 実習でやったこと (Y)

www.kobedenshi.ac.jpにおいて、更新した時のnetworkタブの観察、headerのGeneral,Response Headersを確認した。kd.txtの確認をした。

## 自分で調べたこと

HTTPについてバージョンごとの仕様をくわしく調べた。参考サイト-https://student-engineer.net/http/

## HTTPメッセージ (kd.txt) のうち、最も重要だと思う部分を貼り付けてください

```
GET / HTTP/1.0

HTTP/1.0 200 OK

Date: Fri, 07 Jun 2019 02:25:23 GMT

Server: Apache

X-Cached: Fri, 07 Jun 2019 02:25:26 GMT

X-Pingback: https:/xmlrpc.php

Last-Modified: Fri, 07 Jun 2019 02:25:26 GMT

X-Accel-Expires: 0

Cache-Control: max-age=300

Expires: Fri, 07 Jun 2019 02:30:23 GMT

Vary: Accept-Encoding

Connection: close

Content-Type: text/html; charset=UTF-8

```

## それはなぜですか？

HTTPのステータスが確認することできるからである。

## わかったこと・気づいたこと

更新することでnetworkタブの欄のファイルが多く表示されるようになった。
HTTPリクエストを打ち込んだ後、GET / HTTP/1.0というコマンドを打ち込むとwebのhtmlの要素が確認できた。
kd.txtを確認してみると92行目にGET / HTTP/1.0がありhttpのバージョンが1.0であると確認できた。94行目はHTTP/1.0 200 OKと表記されておりリクエストが正常に受理されたことが確認できた。
