# Node.js Hello World <!-- omit in toc -->

`Node.js`でアプリケーションを実行してHello Worldを表示します。

- [Getting Started](#getting-started)
  - [実行環境の準備](#実行環境の準備)
  - [アプリケーションの実行① - nodeコマンドで実行する](#アプリケーションの実行---nodeコマンドで実行する)
  - [アプリケーションの実行② - npmスクリプトで実行する](#アプリケーションの実行---npmスクリプトで実行する)

---

# Getting Started

## 実行環境の準備

1. `Node.js`をダウンロード・インストールします。
   1. https://nodejs.org/ にアクセスします。
   2. 画面から最新のLTS（Long Term Support。安定版）を選択してインストーラーをダウンロードします。
      ※サイトにアクセスしたマシンのOSに応じたインストーラーが自動で選択されます。
   3. ダウンロードしたインストーラーを起動して`Node.js`をインストールします。
2. Node.jsが正しくインストールされたことを確認します。
   1. 以下のコマンドを入力して`Node.js`のバージョン情報が返却されることを確認します。
        ```bash
        # Node.jsのバージョン。
        node -v
        # 例：
        # > v18.0.0
        ```
    2. 以下のコマンドを入力して`npm`（`Node Package Manager`。パッケージ管理ツール。）のバージョン情報が返却されることを確認します。
        ```bash
        # Node Package Managerのバージョン。
        npm -v
        # 例：
        # > 8.6.0
        ```

## アプリケーションの実行① - nodeコマンドで実行する

以下のコマンドを入力して、コンソールに「Hello World」が表示されることを確認します。

```bash
node index.js
# > Hello World
```

## アプリケーションの実行② - npmスクリプトで実行する

以下のコマンドを入力して、コンソールに「Hello World」が表示されることを確認します。  
[package.json](./package.json)にnpmスクリプトを記載しています。

```bash
npm start
# > nodejs-hello-world@1.0.0 start
# > node index.js

# > Hello World
```
