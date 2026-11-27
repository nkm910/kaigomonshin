# 主治医意見書 問診票（小嶋診療所）

介護保険の主治医意見書作成用の問診票を、患者さん・ご家族が入力し、原本と同じ書式（A4 1枚）で印刷・PDF保存できるWebアプリです。

- 入力内容は端末内（ブラウザの localStorage）にのみ保存され、外部へは送信されません。
- オフラインでも動作します（初回表示後）。

## GitHub Pages での公開手順

1. GitHub で新しいリポジトリを作成（例：`ikensho-monshin`、Public）。
2. このフォルダの中身（`index.html`、`manifest.webmanifest`、`sw.js`、`.nojekyll`、`icons/`）をすべてアップロード。
   - ブラウザの場合：リポジトリ画面の「Add file → Upload files」にドラッグ＆ドロップ → 「Commit changes」。
3. リポジトリの「Settings → Pages」で、Source を「Deploy from a branch」、Branch を `main` / `(root)` にして Save。
4. 1〜2分後に `https://（ユーザー名）.github.io/ikensho-monshin/` で公開されます。

## iPad / iPhone でホーム画面に追加

1. Safari で上記URLを開く。
2. 共有ボタン（□に↑）→「ホーム画面に追加」。

## 印刷・PDF保存

- 「印刷・PDF」ボタン → 印刷画面が開きます。
- **iPad/iPhone**：プリンタを選んで印刷。PDFにする場合は印刷画面上部の共有ボタン →「ファイルに保存」。
- **パソコン（Chrome/Edge）**：送信先で「PDFに保存」を選択。用紙 A4・倍率 100%（「ヘッダーとフッター」はオフ推奨）。

## 更新するとき

`index.html` を差し替えてコミットすれば反映されます。キャッシュを確実に入れ替えたいときは `sw.js` の `CACHE` 名（`v1`→`v2`）も変更してください。
