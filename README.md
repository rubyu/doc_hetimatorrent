![](cover.jpg)
# なぜなにTorrent

<hr>

###  author kyorohiro

##### Torrentクライアント開発時のメモとか



<hr>

* はじめに
   * [はじめに](intro/Introduction.md)
   * [Torrentとは](intro/About.md)
   * [ゴール](intro/Goal.md)
* おまかな仕組み
* Torrentファイルを読み込む
   * [TorrentFile](torrentfile/About.md)
   * [Bencode](torrentfile/Bencode.md)
   * [Bencodeの実装](torrentfile/Implementation.md)
   * [TorrentFileの中身](torrentfile/Content.md)
* UPnpによるポートマップ
   * [UPnPによるポートマップ](upnp/About.md)
   * [UPnPの実装](upnp/Implementation.md)
* Trackerへアクセスしてみる
   * [Trackerへアクセスしてみる](tracker/About.md)]
   * [TrackerはHttpサーバ](tracker/Http.md)
   * [リクエストの中身](tracker/Request.md)
   * [レスポンスの中身](tracker/Response.md)
   * [テスト](tracker/Test.md)
* リダイレクトに対応
   * [リダイレクト](tracker/Redirect.md)
* DHTに対応してみる
   * [Tracker無しでPeerを探す](dht/About.md)
   * [KademuliaのkBucketを利用している](dht/kBucket.md)
   * [RootingTableを実装してみよう](dht/kBucketImpl.md)
   * [FindNodeでネットワークの構築](dht/FindNodes.md)

   * [GetPeersでInfoHashに対応するPeerを探す](dht/GetPeers.md)


