---
title: '<bgsound>: 背景音要素'
slug: Web/HTML/Element/bgsound
---

{{deprecated_header}}{{non-standard_header}}

**`<bgsound>`** は [HTML](/ja/docs/Web/HTML) の非推奨の要素です。そのページが使用されている間の背景として再生される音声ファイルを設定します。代わりに {{HTMLElement("audio")}} 要素を使用してください。

> **警告:** この要素を使用しないでください! ウェブページに音声を埋め込むには、{{HTMLElement("audio")}} 要素を使用してください。

## 属性

- `balance`
  - : この属性は -10,000 から +10,000 の値で、ステレオスピーカーの左右の音量バランスを指定します。
- `loop`
  - : この属性は音声が再生される回数を示します。もしくは無限回のループを示す infinite キーワードが指定可能です。
- `src`
  - : 再生する音声ファイルの URL を指定します。「.wav」、「.au」、「.mid」の何れかの拡張子を持つものでなくてはなりません。
- `volume`
  - : -10,000 から 0 の範囲の数値で、背景音の音量を指定します。

## 例

```html
<bgsound src="sound1.mid">

<bgsound src="sound2.au" loop="infinite">
```

## 使用上の注意

歴史的には、多くのブラウザーで背景の音声を再生するためにオーディオプレイヤープラグインを {{HTMLElement("embed")}} 要素で使用することができました。しかし、これもすでに適切ではなく、代わりにもっと多機能、もっと互換性が高く、プラグインが必要ない `<audio>` を使用するべきです。

`<bgsound>` を自己完結タグ (`<bgsound />`) として書くことができます。しかし、この要素は標準規格外なので、妥当性検査されることはありません。

## 仕様書

{{Specifications}}

## ブラウザーの互換性

{{Compat}}

## 関連情報

- {{htmlelement("audio")}} 要素。文書に音声を埋め込むための標準要素です。

{{HTMLSidebar}}
