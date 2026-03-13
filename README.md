# Speed Minesweeper

20×20 マインスイーパ。10ms 単位タイマー・7セグ風表示・クリアタイムのハイスコア記録付き。

## 遊び方

- `index.html` をブラウザで開く
- **PC**
  - 左クリック: マスを開く
  - 右クリック: 旗を立てる／外す
  - 数字マスで左右同時クリック: 周囲が地雷/安全と分かるときに旗立てまたは一括オープン
- **スマホ**
  - タップ: マスを開く
  - 長押し（コンテキストメニュー）: 旗を立てる／外す
  - 数字マスをタップ: 左右同時クリックと同じ自動展開（旗立て or 一括オープン）

## クリア後

- クリア時だけ「スクショをダウンロード」リンクが表示されます。クリックでゲームエリアの PNG を保存できます。

## Electron（Windows exe）

- `npm install` で依存関係をインストール
- `npm start` でアプリ起動
- `npm run build` で Windows 用 exe をビルド（`dist/speedmine.exe` または `dist/win-unpacked/speedmine.exe`）
- ビルド時は **Electron のウィンドウを閉じてから** 実行すること（ファイルロックで失敗することがある）

## 技術

- HTML / CSS / JavaScript
- CDN: DSEG7 フォント、html2canvas（スクショ用）
- Electron（デスクトップ exe 化）
