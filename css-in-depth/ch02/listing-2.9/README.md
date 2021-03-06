# Listing-2.9

ネストされた要素であっても `em` によるフォントサイズの縮小を避ける場合には、下記のようにネストされた要素では親要素から継承されたフォントサイズの値をそのまま使用するように設定を変更する。

```css
ul {
  font-size: 0.8em;
}

ul ul {
  font-size: 1em;
}
```

これで以下のようにフォントサイズの縮小を防ぐことができる。

![](assets/2021-10-23-06-36-37.png)

しかしこのように特定のフォントサイズの設定を上書きしていくような書き方は望ましくない。

そのため余白サイズや要素の自体のサイズを設定する際には `em` を使用し、フォントサイズには `rem` を使用するといい。
