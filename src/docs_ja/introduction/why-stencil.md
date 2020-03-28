---
title: Stencil - A Compiler for Web Components
description: Stencil has a number of add-ons that you can use with the build process.
url: /docs/introduction
contributors:
  - jthoms1
---

# Stencil: Webコンポーネント用のコンパイラ

Stencilは、Webコンポーネント（より正確に言うと、カスタムエレメント）を生成するコンパイラです。 
Stencilは、最も人気のあるフレームワークの最高の概念をシンプルなビルド時ツールに結合します。

Stencilは次のような機能を持ちます。

- Virtual DOM
- 非同期レンダリング(inspired by React Fiber)
- リアクティブデータバインディング
- TypeScript
- JSX

そして、これらの機能を取り込んだWeb標準のWebコンポーネントを生成します。

StencilはWeb標準に準拠したWebコンポーネントを生成するため、多くの一般的なフレームワークですぐに使用できます。また、Webコンポーネントにすぎないため、フレームワークなしでも使用できます。 さらに、Stencilは、Webコンポーネントだけでなく、プリレンダリング、オブジェクトのプロパティを利用することもできます。

カスタムエレメントを直接作成する場合と比較して、StencilはWebコンポーネントを簡単に記述するためのAPIを提供します。Virtual DOM、JSX、非同期レンダリングなどのAPIは、Webコンポーネントとの100％の互換性を維持しながら、高速で強力なコンポーネントを簡単に作成できるようにします。

デベロッパーエクスペリエンス(DX)も考慮されており、Live Reloadとコンパイラに組み込まれた小さな開発サーバーが付属しています。


## なぜStencilか?

Stencilは、[Ionic Framework](http://ionicframework.com/)チームによって作成されました。すべての主要なフレームワークで機能する、より高速で機能性の高いWebコンポーネントを支援します。

Ionicは主にCordovaアプリを対象としていましたが、Web開発者にとって急速に成長するターゲットとしてのProgressive Web Appsの出現は、Webアプリ開発のパフォーマンスに対する異なるアプローチを要求していました。Ionicは従来のフレームワークとバンドルテクニックを古典的に使用していたため、チームはさまざまなプラットフォームとデバイスで高速ネットワークと低速ネットワークで同等に動作するProgressive Web Appsのレイテンシとコードサイズの要件を満たすのに苦労していました。

さらに、フレームワークを複数使用する場合、あるフレームワーク用に構築されたコンポーネントが別のフレームワークと連動しないという、Web開発の相互運用性の悪夢が生まれました。

Webコンポーネントは両方の問題の解決策を提供し、パフォーマンスを向上させるためにより多くの作業をブラウザーにプッシュし、すべてのフレームワークが使用できる標準ベースのコンポーネントモデルをターゲットにしました。

ただし、Webコンポーネントだけでは十分ではありませんでした。 高速なWebアプリを構築するには、従来のWebフレームワークの内部に閉じ込められていた革新が必要でした。Stencilは、これらの機能を従来のフレームワークから引き出して、急速に出現するWebコンポーネント標準にそれらをもたらすために構築されました。