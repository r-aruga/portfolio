# 目次　<!-- omit in toc -->

- [Markdown記法について](#markdown記法について)
- [基本的な書き方](#基本的な書き方)
  - [Headings - 見出し](#headings---見出し)
  - [italic - 斜体](#italic---斜体)
  - [bold - 太字](#bold---太字)
  - [strikethrough - 打ち消し](#strikethrough---打ち消し)
  - [break（new line） - 改行](#breaknew-line---改行)
  - [link - リンク](#link---リンク)
  - [images - 画像埋め込み](#images---画像埋め込み)
  - [blockquote - 引用](#blockquote---引用)
  - [horizontal rules - 水平線](#horizontal-rules---水平線)
  - [bullet list - 順序なしリスト](#bullet-list---順序なしリスト)
  - [ordered list - 順序ありリスト](#ordered-list---順序ありリスト)
  - [comment out - コメントアウト](#comment-out---コメントアウト)
  - [code spans - コードスパン（インライン表示）](#code-spans---コードスパンインライン表示)
  - [code blocks - コードブロック](#code-blocks---コードブロック)
  - [table - 表](#table---表)
- [【補足】Markdown All in Oneのインストール（VSCode拡張機能）](#補足markdown-all-in-oneのインストールvscode拡張機能)
  - [ショートカットの使用](#ショートカットの使用)
  - [目次を自動で作成・更新](#目次を自動で作成更新)
- [参考](#参考)

---

# Markdown記法について

Markdown記法とは、テキストを構造的に記述する`マークアップ言語`の一つです。（代表的なものだと`HTML`や`XML`がマークアップ言語に分類されます。）

- 特定のルールに則った記号を使い、段落や見出し、装飾といった文書の構造を記載します。
- Markdown記法に対応したアプリケーションはこのルールに従い、読み込んだ文書をHTML構造に変換します。
- 直接HTMLを書くよりも少ない記述で文書の構造を表すことができます。
- HTMLとの互換から、HTMLタグを直接埋め込んでも機能します。（アプリケーションによって例外あり。）
- `GitHub`や`Qiita`などのサービスでMarkdownを使った文章を書くことができ、自動でHTMLに変換されて表示されます。
- `Visual Studio Code`や`Atom`などのテキストエディタがMarkdown記法をサポートしています。（リアルタイムにHTMLプレビューを表示するなど。）

以下はHTMLとMarkdownの比較です。

```html
<!-- HTMLの場合 -->

<h1>見出し1</h1>
<h2>見出し2</h2>
<h3>見出し3</h3>

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

- 順序なしリスト1
- 順序なしリスト2
- 順序なしリスト3

1. 順序ありリスト1
2. 順序ありリスト2
3. 順序ありリスト3

<!-- 直接HTMLタグを埋め込むことも可能。 -->
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

以下に[GitHub Flavored Markdown](https://github.github.com/gfm/)がサポートする記法の一部をまとめます。

## Headings - 見出し

書き方：「#」を付けます。個数によって見出し番号が変わります。

```markdown
# 見出し1
## 見出し2
### 見出し3
```

## italic - 斜体

*斜体*

書き方：「*」で囲みます。

```markdown
*斜体*
```

## bold - 太字

**太字**

書き方：「*」2個で囲みます。

```markdown
**太字**
```

## strikethrough - 打ち消し

~~打ち消し~~

書き方：「~」（チルダ）2個で囲みます。

```markdown
~~打ち消し~~
```

## break（new line） - 改行

文章1  
文章2  
文章3  

書き方：行末に半角スペース2個を付けます。

```markdown
文章1  
文章2  
文章3  
```

## link - リンク

[GitHub 公式](https://github.com/)

書き方：「[]」でタイトル、「()」でURLを囲みます。URLは外部リンク、ページ内リンクとも指定可能です。

```markdown
[タイトル](URL)
```

## images - 画像埋め込み

書き方：先頭に「!」を付け、「[]」でタイトル、「()」でURLを囲みます。画像のURLは外部リンク、ページ内リンクとも指定可能です。

```markdown
![代替テキスト](画像のURL)
```

## blockquote - 引用

> 引用1
>
>> 引用2
>
>>> 引用3

書き方：行頭に「>」と半角スペースを付けます。段落を深くする場合は一行空行を空けます。

```markdown
> 引用1
>
>> 引用2
>
>>> 引用3
```

## horizontal rules - 水平線

---

書き方：以下のいずれかの書き方をします。

```markdown
* * *
***
- - -
---
```

## bullet list - 順序なしリスト

- 順序なしリスト1
- 順序なしリスト2
- 順序なしリスト3
  - 順序なしリストa
  - 順序なしリストb
  - 順序なしリストc

書き方：行頭に「-」と半角スペースを付けます。段落を深くする場合は行頭に対してさらに段落と同じ分のスペースを付けます。

```markdown
- 順序なしリスト1
- 順序なしリスト2
- 順序なしリスト3
  - 順序なしリストa
  - 順序なしリストb
  - 順序なしリストc
```

## ordered list - 順序ありリスト

1. 順序ありリスト1
2. 順序ありリスト2
3. 順序ありリスト3
  1. 順序ありリストa
  2. 順序ありリストb
  3. 順序ありリストc

書き方：行頭に数字と「.」と半角スペースを付けます。段落を深くする場合は行頭に対してさらに段落と同じ分のスペースを付けます。

```markdown
1. 順序ありリスト1
2. 順序ありリスト2
3. 順序ありリスト3
  1. 順序ありリストa
  2. 順序ありリストb
  3. 順序ありリストc
```

## comment out - コメントアウト

書き方：プレビュー時コメントアウトで囲まれた箇所を無視します。HTMLと同じ記法です。

```markdown
<!--  -->
```

## code spans - コードスパン（インライン表示）

`コードスパン`

書き方：「`」（バッククォート）で囲みます。

```markdown
`コードスパン`
```

## code blocks - コードブロック

```html
  <p>パラグラフ1</p>
  <p>パラグラフ2</p>
```

書き方：「`」（バッククォート）または「~」（チルダ）3個でコード部分を囲みます。

※`'''html`のように、先頭側の後ろに拡張子の名前を付けると拡張子に対応した記法のシンタックスハイライトがつくようになります。


## table - 表

| タイトル/左寄せ | タイトル/中央寄せ | タイトル/右寄せ |
| :-------------- | :---------------: | --------------: |
| 項目1           |       項目1       |           項目1 |
| 項目2           |       項目2       |           項目2 |
| 項目3           |       項目3       |           項目3 |

書き方：各要素を「|」で区切ります。上から列タイトル、列の寄せ方の指定、項目の順です。列と行は任意の数だけ増やすことができます。（ただし、列タイトルと列の寄せ方の指定はそれぞれ二行以上書くことはできません。）


```markdown
| タイトル/左寄せ | タイトル/中央寄せ | タイトル/右寄せ |
| :-------------- | :---------------: | --------------: |
| 項目1           |       項目1       |           項目1 |
| 項目2           |       項目2       |           項目2 |
| 項目3           |       項目3       |           項目3 |
```

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

以下の手順でMarkdownファイルに自動で目次を挿入できます。

1. `Visual Studio Code`で任意のMarkdownファイルを開きます。
2. `Ctrl/Cmd` + `Shift` + `P`でコマンドパレットを表示します。
3. コマンドパレットメニューから`Markdown All in One: Create Table of Contents`を選択します。（見出しを数えてくれます。）

![markdown-syntax-cheatsheet-01.jpg](/.sample/.assets/markdown-syntax-cheatsheet-01.jpg)

また、`settings.json`で`markdown.extension.toc.updateOnSave`をONにするとファイルを保存した時自動で目次を更新してくれるようになります。  
（`ユーザー/ワークスペースの設定`から設定を有効にできます。）

![markdown-syntax-cheatsheet-01.jpg](/.sample/.assets/markdown-syntax-cheatsheet-02.jpg)

---

# 参考

- [GitHub Flavored Markdown Spec](https://github.github.com/gfm/)
- [Markdownとは · 日本語Markdownユーザー会](https://www.markdown.jp/what-is-markdown/)
- [Markdown記法 チートシート - Qiita](https://qiita.com/Qiita/items/c686397e4a0f4f11683d)
