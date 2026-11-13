# RPYS_FACTORY 紹介サイト(GitHub Pages 用)

このフォルダの中身をそのまま GitHub に上げれば公開できます。

- `index.html`: トップ。紹介だけで、ストアへのリンクは置いていません(Unity Asset Store のルール対策)。
- `products.html`: パック一覧。ここにだけ BOOTH・Unity・Fab へのリンクがあります。
- `style.css`, `favicon.svg`, `images/`: 見た目と画像。
- `.nojekyll`: GitHub Pages にそのまま表示させるための空ファイル(消さないでください)。

## 公開のしかた

1. GitHub で新しいリポジトリを作る。
   - 名前を `<GitHubのユーザー名>.github.io` にすると、URL が `https://<ユーザー名>.github.io/` になります(おすすめ)。
   - 別の名前(例: `rpys-factory`)なら `https://<ユーザー名>.github.io/rpys-factory/` になります。
   - Public(公開)にする。
2. リポジトリの画面で「Add file」→「Upload files」。このフォルダの中身(`index.html` など全部と `images` フォルダ)をドラッグして「Commit changes」。
   - `.nojekyll` は見えないことがあります。上がらなくても表示はたぶん大丈夫です。
3. 「Settings」→「Pages」→ Source を「Deploy from a branch」、Branch を `main` / `(root)` にして Save。
4. 1〜2 分待って、表示された URL を開いて確認。
5. その URL(トップページ)を Unity Asset Store のパブリッシャー情報の「Website」欄に入れる。

## あとで直すところ(products.html)

- ストアのボタンは `href=""` のものは表示されません。URL を入れると出てきます。
  - 消防設備パックの「Unity Asset Store」ボタンに、公開ページの URL を入れてください。
  - Fab の審査が通ったら Fab の URL を入れてください。
- BOOTH のボタンはいまショップのトップ(https://rpys-factory.booth.pm/)です。各商品ページの URL に変えるとより親切です。
- 工事・区画用品パックを出したら、「COMING SOON」の行(`<span class="badge-soon">`)を消して、ストアのボタンを足してください(ほかのパックの `<div class="stores">` をまねる)。

## 注意

- トップページ(index.html)には「購入」ボタンやストアへのリンクを置かないでください(Unity の審査で却下される原因になります)。
- メールアドレスは載せていません。問い合わせは各ストアのメッセージ機能から、としています。
