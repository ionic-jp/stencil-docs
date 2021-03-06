---
title: Stencil CLI
description: Stencil CLI
url: /docs/cli
contributors:
  - miguelyoobic95
  - adamdbradley
---

# Command Line Interface (CLI)


## `stencil build`

Stencilプロジェクトをビルドします。以下のフラグは`build`コマンドで利用可能なオプションです。

| Flag | Description | Alias |
|------|-------------|-------|
| `--ci` | 継続的インテグレーション（CI）環境の推奨設定を使用してビルドを実行します。ワーカーの数はデフォルトで4に設定されており、テストでスクリーンショットを取ると、コンソールのログを変更し追加で時間がかかります。 | |
| `--config` | `stencil.config.ts`ファイルのパス。Stencilがconfigを見つけるので、このフラグはほとんどの場合必要ありません。さらに、Stencilのconfigは必須ではありません。 | `-c` |
| `--debug` | デバッグに役立つランタイムコードを追加し、より詳細なログの出力レベルを設定します。 | |
| `--dev` | 開発ビルドを実行します。 | |
| `--docs-readme` | コンポーネントのタイプ、プロパティ、メソッド、イベント、JSDocs、CSSカスタムプロパティなどに基づいて、`readme.md`ドキュメントを生成します。 | |
| `--es5` | ES5互換のビルドを作成します。デフォルトではビルド時間を短縮するため、開発中はES5ビルドを作成しません。ただし、プロダクションビルド中は常にES5ビルドを作成します。このフラグを使用すると、開発中にもES5ビルドを作成します。 | |
| `--log` | `stencil build`のログを`stencil-build.log`に出力します。ログファイルはconfigと同じディレクトリに出力されます。 | |
| `--prerender` | ビルド完了後、`www`出力ターゲットを使用してアプリケーションを事前にレンダリングします。 | |
| `--prod` | バンドルの改善や未使用のコードを削除、最小化するなど、各ファイルを最適化して本番ビルドを実行します。本番ビルドはデフォルトであり、このフラグは`--dev`フラグを上書きする時のみに使用されます。 | |
| `--max-workers` | コンパイラが使用するワーカーの最大数。デフォルトでは、OSで使用可能なCPUの数を使用します。 | |
| `--next` | "次期の"Stencilコンパイラ機能をテストするためのオプトイン。 | |
| `--no-cache` | キャッシュの使用を無効にします。 | |
| `--no-open` | デフォルトでは `--serve`コマンドはブラウザウィンドウを開きます。`--no-open`を使用すると、ブラウザは自動的に開かなくなります。 | |
| `--port` | [Integrated Dev Server](/docs/dev-server)のポート。 デフォルトは"3333"です。 | `-p` |
| `--serve` | [Integrated Dev Server](/docs/dev-server)を起動します. | |
| `--stats` | プロジェクトに関する統計を `stencil-stats.json`に出力します。統計ファイルは、configと同じ場所に出力されます。 | |
| `--verbose` | ビルドの各ステップに関する追加情報をログに記録します。 | |
| `--watch` | 開発中にファイルを監視し、ファイルが更新されると再ビルドします。 | |


## `stencil test`

Stencilプロジェクトをテストします。以下のフラグは`test`コマンドで利用可能なオプションです。

| フラグ | 説明 |
|------|-------------|
| `--spec` | [Jest](https://jestjs.io/)を使用して `.spec.ts`ファイルをテストします。 |
| `--e2e` | [Puppeteer](https://developers.google.com/web/tools/puppeteer)と[Jest](https://jestjs.io/)を使用して`.e2e.ts`ファイルをテストします。 |

## `stencil`

| フラグ | 説明 |
|------|-------------|
| `--help` | さまざまなフラグを説明するヘルプ情報を表示します。 | `-h` |
| `--version` | 現在使用しているStencilのバージョンを表示します。 | `-v` |


## `stencil generate <sub-folder>`

インタラクティブなコンポーネントジェネレータを起動します。コンポーネントを生成するサブフォルダーを1つ以上指定できます。
