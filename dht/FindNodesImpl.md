# FindNodesを実装してみよう
<hr>
* **FindNodeクエリでネットワークを構築する**
<br>
* **リスポンスを受けたらRootingTableを更新する**
<br>
<hr>


通信ライブラリとして、hetimanetを使用しています。APIのインターフェイスは他の通信ライブラリと大きな違いはありません。なので、お使いのものと読み替えて読み進めてください。


### (1) KNodeはUDPサーバー機能を持つ。

まずは、UDPを用いて、通信部分を書いてみましょう。Torrentの仕様では、DHTとして動作するPeerをNodeと読んでいます。
DHTの通信を行う主体として、KNode class を定義することにします。

UDP serverは、メッセージを受け取るメッセージはbencodeなのでした。パースして必要な処理に回します。

```
class KNode {
  Future start({String ip: "0.0.0.0", int port: 28080}) async {
    (_isStart != false ? throw "already started" : 0);
    _udpSocket = this._socketBuilder.createUdpClient();
    return _udpSocket.bind(ip, port, multicast: true).then((int v) {
      _udpSocket.onReceive().listen((HetiReceiveUdpInfo info) {
        KrpcMessage.decode(info.data, this).then((KrpcMessage message) {
          onReceiveMessage(info, message);
        });
      });
      //////
      _isStart = true;
    });
  }

}
```
