# About
<hr>
<br>
* **データを配信してくれるPeerを探すところから始まる**
* **Trackerサーバーを利用する方法について解説します**

<br>

<hr>

 これまでの成果で、Torrentファイル から必要な情報を取り
出す事が出来るようになりました。Torrentクライアント は、
Torrentファイルを解析が終わると、Trackerサーバーにアクセスし
ます。

　P2Pアプリケーションは、データを配信してくれるPeerを探すところから始まります。Googleで検索ワードを指定しても欲しい情報を探すように、P2Pアプリもなんらかの方法で、データを配信してくれるPeerを発見する必要があります。TorrentはTrackerサーバーを利用する方法でこれを実現しています

　本章では、実際に簡易の Trackerサーバーを作成しながら、Tracker から Peer の一覧を取得する方法について解説し
ます。


(※) Torrentでは、Peerの一覧をP2Pネッワーク上で管理する方法も提供しています。DHTの章で紹介します。



-------
Kyorohiro work

http://kyorohiro.strikingly.com