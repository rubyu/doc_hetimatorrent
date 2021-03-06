# テストファーストの環境を整える (1)

本書ではテストファーストで開発を進める事を推奨しています。
テストで固めて、コードをリファクタリングできるように維持していきましょう。

本章では、「Observatory」の使い方についての日本語訳を掲載します。

## Observatory: A Profiler for Dart App
引用(https://www.dartlang.org/tools/observatory/)

Observatoryは profiling と debugging 用のツールです。

```
ObservatoryはFreeでGETできます。
https://www.dartlang.org/downloads/ から取得できます。
issueやrequestは、 http://dartbug.com/new で受け付けています。
```

Observatoryは動作中のDart VM の中身を覗くことができます。そして、即座にレポートしてくれます。

* どの部分に時間を費やしていたか
* allocatedした メモリーを調べます。
* コードのどの部分が実行されたわかります
* メモリーリークをデバックできます
* メモリーの断片化をデバックできます


次のビデオは、Dart Developer Summit をレコードしたものです。John McCutchan と Todd Turnidge で　使い方について解説しています。

https://youtu.be/y39pZCExsOs?list=PLOU2XLYxmsIIQorIS8gagUiMau9S84vZV


### Using Observatory
* [get started with Observatory](Observatory_GetStarted.md)

To learn about specific features, read these pages:

* [Allocation Profile](https://www.dartlang.org/tools/observatory/allocation-profile.html)
* [Code Coverage](https://www.dartlang.org/tools/observatory/code-coverage.html)
* [CPU Profile](https://www.dartlang.org/tools/observatory/cpu-profile.html)
* [Debugger](https://www.dartlang.org/tools/observatory/debugger.html)
* [Evaluating Expressions](https://www.dartlang.org/tools/observatory/evaluate.html)
* [Heap Map](https://www.dartlang.org/tools/observatory/heap-map.html)
* [Isolate](https://www.dartlang.org/tools/observatory/isolate.html)
* [Metrics](https://www.dartlang.org/tools/observatory/metrics.html)
* [User and VM Tags](https://www.dartlang.org/tools/observatory/tags.html)
 
The following pages have reference information about Observatory:

* [dart: The Standalone VM](https://www.dartlang.org/tools/dart-vm/#observatory)
* [Glossary of VM Terms](https://www.dartlang.org/tools/observatory/glossary.html)
* [Screens in Observatory](https://www.dartlang.org/tools/observatory/screens.html)

##### Support and discussion

Join the [Observatory discussion mailing list](https://groups.google.com/a/dartlang.org/forum/#!forum/observatory-discuss) to ask questions and chat with users.

##### Filing bugs and feature requests
To see existing issues or create a new one directly, see all [Observatory issues](https://github.com/dart-lang/sdk/labels/Area-Observatory).