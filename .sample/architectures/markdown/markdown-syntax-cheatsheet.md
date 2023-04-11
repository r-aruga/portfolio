# 目次　<!-- omit in toc -->

- [Markdown記法について](#markdown記法について)
- [基本的な書き方](#基本的な書き方)
  - [見出し](#見出し)
  - [太字 - bold](#太字---bold)
  - [斜体 - italic](#斜体---italic)
  - [打ち消し - strikethrough](#打ち消し---strikethrough)
  - [順序なしリスト - bullet list](#順序なしリスト---bullet-list)
  - [順序ありリスト - ordered list](#順序ありリスト---ordered-list)
- [【補足】Markdown All in Oneのインストール（VSCode拡張機能）](#補足markdown-all-in-oneのインストールvscode拡張機能)
  - [ショートカットの使用](#ショートカットの使用)
  - [目次を自動で作成・更新](#目次を自動で作成更新)
  - [Markdown -\> HTMLに変換](#markdown---htmlに変換)
- [参考](#参考)

---

# Markdown記法について

Markdown記法とは、テキストを構造的に記述する`マークアップ言語`の一つです。（代表的なものだと、`HTML`や`XML`がマークアップ言語に分類されます。）

特定のルールに則った記号を使い、段落や見出し、装飾といった文書の構造を記載します。  
Markdown記法に対応したアプリケーションはこのルールに従い、読み込んだ文書をHTML構造に変換します。  
直接HTMLを書くよりも少ない記述で文書の構造を表すことができます。

また、HTMLとの互換から、HTMLタグを直接埋め込んでも機能します。（アプリケーションによって例外あり。）


```html
<!-- HTMLの場合 -->

<h1>見出し1</h1>

<h2>見出し2</h2>

<h3>見出し3</h3>

<strong>太字</strong>

<s>打ち消し</s>

<ul>
    <li>順序なしリスト1</li>
    <li>順序なしリスト2</li>
    <li>順序なしリスト3</li>
</ul>

<ol>
    <li>順序ありリスト1</li>
    <li>順序ありリスト2</li>
    <li>順序ありリスト3</li>
</ol>

<dl>
    <dt>説明リスト1</dt>
    <dd>説明リスト1</dd>
    <dt>説明リスト2</dt>
    <dd>説明リスト2</dd>
    <dt>説明リスト3</dt>
    <dd>説明リスト3</dd>
</dl>

```

```markdown
<!-- Markdownの場合 -->

# 見出し1

## 見出し2

### 見出し3

**太字**

~~打ち消し~~

- 順序なしリスト1
- 順序なしリスト2
- 順序なしリスト3

1. 順序ありリスト1
2. 順序ありリスト2
3. 順序ありリスト3

<!-- 直接HTMLタグを埋め込むことが可能。 -->
<dl>
    <dt>説明リスト1</dt>
    <dd>説明リスト1</dd>
    <dt>説明リスト2</dt>
    <dd>説明リスト2</dd>
    <dt>説明リスト3</dt>
    <dd>説明リスト3</dd>
</dl>

```

---

# 基本的な書き方

以下に[GitHub Flavored Markdown](https://github.github.com/gfm/)がサポートする記法をまとめます。

## 見出し

## 太字 - bold

## 斜体 - italic

## 打ち消し - strikethrough

## 順序なしリスト - bullet list

## 順序ありリスト - ordered list

---

# 【補足】Markdown All in Oneのインストール（VSCode拡張機能）

`Visual Studio Code`でMarkdownを編集する場合、拡張機能の[Markdown All in One](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one)をインストールすると以下の機能が使えるようになります。

## ショートカットの使用

一部の操作で[ショートカット](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one#keyboard-shortcuts-1)を利用できます。

| キー                       | 動作                                   |
| -------------------------- | -------------------------------------- |
| `Ctrl/Cmd` + `B`           | 太字 - bold                            |
| `Ctrl/Cmd` + `I`           | 斜体 - italic                          |
| `Alt` + `S`                | 打ち消し - strikethrough               |
| `Ctrl/Cmd` + `Shift` + `]` | 見出しの番号を上げる                   |
| `Ctrl/Cmd` + `Shift` + `[` | 見出しの番号を下げる                   |
| `Ctrl/Cmd` + `M`           | 数式の挿入                             |
| `Alt` + `C`                | タスクリストのチェックのON/OFF切り替え |
| `Ctrl/Cmd` + `Shift` + `V` | サイドにプレビューを表示               |
| `Ctrl/Cmd` + `K` → `V`     | タブにプレビューを表示                 |

## 目次を自動で作成・更新

## Markdown -> HTMLに変換

---

# 参考

- [GitHub Flavored Markdown Spec](https://github.github.com/gfm/)
- [Markdownとは · 日本語Markdownユーザー会](https://www.markdown.jp/what-is-markdown/)
- [Markdown記法 チートシート - Qiita](https://qiita.com/Qiita/items/c686397e4a0f4f11683d)
