# Ticket NFT

チケットとして機能するような NFT を活用する Web アプリケーションのサンプルです。NFT を保有している人だけが特定の Web ページを見られように、アクセスしてきたユーザに対してウォレット アドレスによる認証・認可を行います。

## ディレクトリ構成

このレポジトリは、以下に示す 3 つのディレクトリを含んでいます。それぞれのディレクトリが、個別のレポジトリへのサブ モジュールになっています。

* **[backend](https://github.com/takeiyuto/ticket-backend)** ディレクトリ<br>
バックエンドを記述した TypeScript のプロジェクトです。ビルドして起動すると、Express を利用した Web サーバが開始します。

* **[blockchain](https://github.com/takeiyuto/ticket-contract)** ディレクトリ<br>
スマート コントラクトを記述した Truffle プロジェクトです。スマート コントラクトは、コンパイルした後、ブロックチェーンにデプロイします。

* **[frontend](https://github.com/takeiyuto/ticket-frontend)** ディレクトリ<br>
TypeScript と Vue 3 でフロントエンドを記述した webpack 5 のプロジェクトです。ビルドすると、ユーザー向けのページと管理者向けのページが `dist` ディレクトリに生成されます。

次のコマンドで、全サブ モジュールも含めて、再帰的にクローンします。

```bash
git clone --recursive https://github.com/takeiyuto/tickets.git
```

## 動作方法

以下の順序で、それぞれのプロジェクトの README の手順に従います。

1. `blockchain` ([README](https://github.com/takeiyuto/ticket-contract/blob/main/README.md))
2. `frontend` ([README](https://github.com/takeiyuto/ticket-frontend/blob/main/README.md))
3. `backend` ([README](https://github.com/takeiyuto/ticket-backend/blob/main/README.md))

## ライセンス表示

このサンプル プロジェクトは、[MIT License](LICENSE)で提供しています。

# 参照

[徹底解説 NFTの理論と実践](https://www.ohmsha.co.jp/book/9784274230608/)の第8章を参照してください。[本書の Web サイト](https://takeiyuto.github.io/nft-book)も参考にしてください。
