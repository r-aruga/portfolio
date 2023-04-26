# Strategies for Portfolio <!-- omit in toc -->

- [Purpose of this repository](#purpose-of-this-repository)
- [Getting Started](#getting-started)
  - [Folder structure](#folder-structure)
  - [Initialize Repository](#initialize-repository)

---

# Purpose of this repository

エンジニアの日々の学びの蓄積と、学びをもとにしたポートフォリオを集約したリポジトリを作成するためのテンプレートです。

継続的な学習のモチベーションの向上を図ることと、最終的にはリポジトリをGitHubで公開し、学習の成果を第三者から客観的に見えやすくすることが目的です。

---

# Getting Started

## Folder structure

このリポジトリは4つのフォルダで構成されています。

1. [curriculums](curriculums/) ->
   - 講座・学習教材でインプットした内容や進捗を書き出します。（markdown形式）
   - 学習した内容の要点、疑問や不明点を記載します。その時に何を感じたかを記録に残すためです。
   - markdownファイルのタイトルは何の講座・学習教材を参照したか分かりやすいものを記載します。
   - 講座・学習教材単位でフォルダ・ファイルを分けます。管理しやすい単位で問題ありません。
   - 例 -> `curriculums/progate/sql.md`または`progate/sql/学習レッスンⅠ.md`など。
2. [today-i-Learned](today-i-learned/) ->
   - 自学でインプットした内容（TIL：今日学んだこと）を書き出します。（markdown形式）
   - 自分に向けたメモ書き、備忘録として記載します。
   - 各アーキテクチャ分野の単位でフォルダ・ファイルを分けます。
   - フォルダ分けは `言語（アーキテクチャの種類） > フレームワーク or ライブラリ`の単位が望ましいです。
   - 例 -> `today-i-Learned/linux/bashの便利なコマンド集.md`など。
3. [architectures](architectures/) ->
   - 学んだことをアウトプットした内容を書き出します。（markdown形式）
   - ナレッジとして第三者に公開するイメージで、丁寧な文面と正しい情報を心がけて記載します。
   - markdownファイルのタイトルは何のアーキテクチャに関連しているか分かりやすいものを記載します。
   - 各アーキテクチャ分野の単位でフォルダ・ファイルを分けます。
   - フォルダ分けは `言語（アーキテクチャの種類） > フレームワーク or ライブラリ`の単位が望ましいです。
   - 例 -> `architectures/python/django-rest-framework/アクセストークンを発行する方法.md`など。

4. [applications](applications/) ->
   - これまでの学習内容をもとに、自身が作成したアプリケーションを配置します。
   - 適切に環境構築、ビルドすれば正常に動作する形で登録することが望ましいです。
   - リポジトリの容量圧迫を避けるため、ビルドした資材そのものは登録しないようにします。
   - アプリケーションの単位でフォルダを分けます。
   - 例 -> `applications/todo-app-with-react`など。

## Initialize Repository

1. このリポジトリをローカル環境にクローンします。

   ```bash
   # HTTPS経由
   git clone https://github.com/r-aruga/portfolio.git
   ```

2. 以下のコマンドを実行し、.gitフォルダを削除してリポジトリ情報を初期化します。

   ```bash
   rm -rf .git && git init
   ```

