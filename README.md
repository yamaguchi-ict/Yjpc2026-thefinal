# ASOBI PARK｜やまぐちジュニアプログラマーコンテスト2026 ファイナリスト作品展示

最終審査発表会のファイナリスト作品を、**氏名非公開・作品番号制**で展示する特設サイトです。GitHub Pages でそのまま公開できます。

## 公開手順（GitHub Pages）

1. GitHub で新しいリポジトリを作成（例：`jp-contest-exhibit`。Public を推奨）
2. このフォルダの中身（`index.html` / `assets/` / `README.md` / `.nojekyll`）をすべてアップロード
   - GitHub の「Add file → Upload files」からドラッグ＆ドロップでOK
3. リポジトリの **Settings → Pages → Source** で
   - Branch: `main` ／ Folder: `/ (root)` を選んで **Save**
4. 1〜2分後、`https://<ユーザー名>.github.io/<リポジトリ名>/` で公開されます

## 作品データの追加・編集

作品情報はすべて **`assets/works.js`** 1か所で管理しています。エディタで開いて編集してください。

```js
{
  "no": 31,                  // 作品番号（表示・並び順に使用）
  "grade": "中学2年",        // 学年
  "cat": "中学生",           // 応募カテゴリ（小学1年～3年 / 小学4年～6年 / 中学生）
  "dept": "01.ブロックプログラム",  // 部門（01=琥珀色 / 02=緑の色分け）
  "title": "作品名",
  "url": "https://...",      // 作品の公開URL
  "kind": "Scratch",         // Scratch / 動画 / Webアプリ / MakeCode
  "thumb": "assets/thumbs/31.jpg"  // 640×480(4:3)推奨
}
```

サムネイルは `assets/thumbs/` に `番号.jpg`（640×480・4:3）で追加してください。

## 氏名非公開について

審査の公平性のため、氏名・学校名はサイトに含まれていません。閲覧者は作品番号（No.）とサムネイルで作品を判断します。入賞発表時に氏名を公表する場合は、このデータに `name` フィールドを追加し、`index.html` のカード表示を修正してください。

## 構成

```
index.html          … サイト本体（単一ファイル・外部ライブラリ不要）
assets/works.js     … 作品データ（ここだけ編集すれば更新できる）
assets/works.json   … 同データの JSON 版（機械処理用）
assets/thumbs/      … サムネイル画像 01〜30.jpg
assets/mv.jpg       … コンテスト メインビジュアル（THE FINAL 2026）
assets/asobi-title.jpg … ASOBI PARK 看板バナー（ヒーロー）
assets/schedule.jpg … DAY1/DAY2 スケジュールバナー
.nojekyll           … GitHub Pages の Jekyll 処理を無効化
```
