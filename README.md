# Git について

Gitはソフトウェア開発における重要なバージョン管理ツールで、主にソースコードを扱います。多くの開発プロジェクトでは、複数の開発者が同時にコードを編集するため、誰がどのような変更を行ったかを記録する仕組みが欠かせません。Gitは各変更を「コミット」として保存し、過去の状態に遡ることができるため、バグが見つかった際も迅速に原因を特定し、以前のバージョンに戻すことが容易です。

さらに、Gitはブランチ機能を活用することで、並行して作業を行うことが可能です。開発者は新機能の追加やバグ修正を独立したブランチで進めることができ、メインのコードに影響を与えずに作業を続けられます。完成したら、そのブランチをメインのブランチに統合することで、効率的な開発が実現します。

また、GitはGitHubやGitLabといったリモートリポジトリと連携することで、プロジェクトのコードをオンラインで共有し、チーム内での協力やフィードバックを促進します。これにより、リモートワークやオープンソースプロジェクトの管理もスムーズに行えるようになります。


# GitHub について

GitHubは、Gitを基盤としたソースコードの管理と共有を目的としたプラットフォームで、開発者がリモートでプロジェクトを協力して進めるための場を提供しています。主な機能は、Gitリポジトリをオンラインでホストし、チームでのコラボレーションをスムーズにすることです。開発者は、プロジェクトのソースコードをリポジトリにアップロードし、他のメンバーと同時に編集やレビュー、バグ修正を行うことができます。

GitHubには、プルリクエストという仕組みがあり、これを通じて他の開発者が提案した変更を確認し、議論を経てメインプロジェクトに統合するかどうかを決定できます。これにより、コードの品質が向上し、チーム全体で一貫した開発を実現します。また、イシュートラッキング機能を使うことで、バグや新機能の要望を整理し、進捗状況を可視化することができるため、プロジェクト全体の管理がより簡単になります。

さらに、GitHubはオープンソースプロジェクトのホスティングにも広く利用されており、世界中の開発者が自由に貢献できる場としても重要です。無料プランからスタートし、必要に応じて有料プランに移行することも可能で、個人のプロジェクトから大規模な企業プロジェクトまで多様な用途に対応しています。

# Markdown について

Markdownは、シンプルな書式設定を行うための軽量なマークアップ言語で、読みやすく書きやすいテキスト形式を提供します。ジョン・グルーバーによって作られたこの言語の主な目的は、テキストを簡潔かつ視覚的に整えながら、HTMLなどの複雑なタグを使用せずに書式を反映することです。Markdownは、Webライティング、ドキュメント作成、ブログ、GitHubのREADMEファイルなど、さまざまな用途で利用されています。

Markdownの特徴は、その直感的な記法です。例えば、見出しには「#」を用い、リストは「-」や「*」で作成します。リンクや画像の挿入も容易で、太字や斜体の装飾もシンプルな記号で表現できます。このため、書式がシンプルでありながら、テキスト自体が読みやすいという利点があります。特別なソフトウェアなしで編集できる点も魅力です。

さらに、Markdownは多くのプラットフォームで対応しており、HTMLへの変換も簡単です。この特性から、開発者やライターが効率よくドキュメントやWebコンテンツを作成し、共有するためのツールとして広く利用されています。

# git とは

Gitは、ソースコード管理システムの一つで、複数人での開発作業を効率的に行うためのツールです。Gitはバージョン管理を行い、変更履歴を保存することで、過去の状態に戻ったり、異なるバージョンのコードを比較したりすることができます。

# git インストール

Gitをインストールするには、以下の手順を実行します。

1. Mac でターミナルを開き、次のコマンドを実行
```
brew install git
```

# git セットアップ

1. Gitのバージョン確認
```
brew install git
```

2. ユーザー名とメールアドレスを設定
```
git config --global user.name "ユーザー名"
git config --global user.email "メールアドレス"
```

# git の使い方

- **git init**
  - 新しいGitリポジトリを初期化します。
  - `git init`
- **git add**
  - 変更をステージングエリアに追加します。
  - `git add ファイル名`
- **git commit**
  - ステージングエリアの変更をリポジトリにコミットします。
  - `git commit -m "コミットメッセージ"`
- **git push**
  - リモートリポジトリにローカルの変更をプッシュします。
  - `git push origin ブランチ名`

# github アカウントの作成

GitHubのアカウントを作成するには、以下の手順を実行

1. GitHubの公式サイトにアクセスします。
2. 「Sign up」をクリックし、必要な情報を入力します。
3. メールアドレスを確認し、アカウントを有効化します。

# github への　README.md 公開方法

1. GitHubで新しいリポジトリを作成します。

2. ターミナルでリポジトリをクローンします。
```
git clone https://github.com/yoshirane/mau-j2n.git
```

3. README.mdファイルを編集します。
```
touch README.md
```

4. 変更をGitに追加します。
```
git add README.md
```

5. 変更をコミットします。
```
git commit -m "README.mdを追加しました"
```

6. 変更をプッシュします。
```
git push origin main
```