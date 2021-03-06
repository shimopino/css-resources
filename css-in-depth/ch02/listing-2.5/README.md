# Listing-2.5

`em` は対象の要素のフォントサイズを基準として相対的な単位ではあるが、フォントサイズ自身の値にも使用することができる。

この場合には、**継承された** フォントサイズが基準となる。

そこで `slogan` クラスを適用している要素では、`<body>` タグで指定されているフォントサイズを継承するように指定する。

```html
<body>
  We love coffee
  <p class="slogan">We love coffee</p>
</body>
```

ここでは以下のように指定する。

```css
body {
  font-size: 16px;
}

/* 1.2em = 16px * 1.2 = 19.2px */
.slogan {
  font-size: 1.2em;
}
```

`em` を指定する場合は、要素が継承しているフォントサイズ（例えば `16px`）と、希望しているフォントサイズ（例えば `10px`）がわかっている場合には、計算で求めることが可能である。（`10 / 16 = 0.625em`）
