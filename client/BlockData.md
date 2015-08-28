# ブロックデータ
<hr>
* **Bitfieldを実装**
* **BlockDataを実装**
<hr>


## Bitfield実装

Bitfieldを実装していきす。 Bitfield Bool値(0, 1)を持つ任意の長さの配列です。

```
class Bitfield {
 bool List<bool> data = [];
 Bitfield(int length) {
   data = new List.filled(length, 0);
 }

  bool operator [](int idx) => data[idx];
  void operator []=(int index, bool value) => setIsOn(index, value);
}
```

