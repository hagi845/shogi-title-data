# shogi-title-data

iOSアプリ「将棋タイトル」が起動時に読み込むタイトル戦データ。

- `shogi_data.json` を更新して push すると、アプリは次回起動時に自動で最新データに差し替わる
- 更新時は `dataVersion` を必ず +1 し、`updatedAt` を更新すること(古い dataVersion は無視される)
- 各局の `result`: 保持者勝ち=`"holder"` / 挑戦者勝ち=`"challenger"` / 未対局=`null`
