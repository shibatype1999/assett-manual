# スクリーンショット撮影リスト

マニュアル本文で参照しているスクリーンショットの一覧です。
本文からは `https://raw.githubusercontent.com/shibatype1999/assett-manual/main/images/…` の形で参照しているため、画像は `main` ブランチに反映されると表示されます。
下の表のファイル名で、`images/ja/`（日本語UI）と `images/en/`（英語UI）にそれぞれ保存してください。
ファイル名は日本語版・英語版で共通です。

## 撮影のポイント

- **端末**: iPhone（全画像で同じ機種にそろえると、見た目が統一されます）
- **形式**: PNG
- **言語**: `ja/` はアプリの言語を「日本語」、`en/` は「English」にして撮影します（「設定」→「言語」）。
- **スキン・テーマ**: すべての画像で同じスキンにそろえます（スキンが「スタンダード」の場合は、テーマを「ライト」にすることをおすすめします）。
- **データ**: 見本用のデータ（架空の金額）を入力した状態で撮影します。個人の実際の資産が写らないようご注意ください。
  - 例: 資産「A銀行」「B銀行」「C証券」「米国株（米ドル）」「住宅ローン（負債）」、それぞれ数か月分の記録
  - 記録にサブカテゴリ（給料・評価額など）を付けておくと、増減要因のグラフが写ります。
  - 資産目標も設定しておくと、達成率や目標ラインが写ります。
  - プレミアムの機能（積み上げグラフ・自動バックアップなど）は、プレミアムが有効な状態で撮影します。
- **広告**: プレミアムを有効にして、広告が写らない状態で撮影することをおすすめします。
- **ステータスバー**: 時刻・電波・電池などが気になる場合は、トリミングしてもかまいません。

## 撮影リスト

| ファイル名 | 使用ページ（`pages/<言語>/…`） | 撮影する画面 |
| --- | --- | --- |
| `dashboard.png` | index / dashboard | 「ダッシュボード」タブ（総資産額・資産比率・資産別の総額のパネル） |
| `tab-bar.png` | getting-started | 画面下部のタブ（5つのタブが見えるように） |
| `dashboard-edit.png` | dashboard | ダッシュボードの編集モード（パネル一覧と「パネルを追加」） |
| `input.png` | recording | 「入力」タブ（上部の「シンプル」「一括」「資産別」「カレンダー」のタブが見える状態） |
| `input-simple.png` | recording | 「入力」タブの「シンプル」（資産を選んで金額を入力した状態） |
| `input-batch.png` | recording | 「一括」タブで一括入力をタップした記録の画面（前回の金額と「空欄に前回の金額を入れる」が見える状態） |
| `input-by-asset.png` | recording | 「入力」タブの「資産別」（資産一覧・残高・前月比） |
| `input-calendar.png` | recording | 「入力」タブの「カレンダー」（点の付いた日と、選んだ日の記録の一覧） |
| `asset-detail.png` | recording | 資産をタップした記録一覧（期間・並び順・表示件数と記録の表） |
| `asset-list.png` | assets | 「資産一覧」画面 |
| `asset-form.png` | assets | 「資産追加」をタップした「資産を追加」画面 |
| `category-list.png` | categories | 「設定」→「カテゴリ」画面（標準の印と含まれる資産が見える状態） |
| `category-form.png` | categories | カテゴリをタップした編集画面（色・含める資産） |
| `chart-line.png` | chart | 「チャート」タブ（「全体」・折れ線グラフ・目標ライン表示） |
| `chart-stacked.png` | chart | 「チャート」タブで「積み上げグラフ」を選んだ状態 |
| `chart-change-factors.png` | chart | 「チャート」タブで「増減要因」を選んだ状態（棒グラフと期間内の増減要因の一覧） |
| `chart-table.png` | chart | 「チャート」タブ下部の推移の表（日/月/年の切り替えと表示件数が見える状態） |
| `asset-composition.png` | asset-composition | 「資産構成」タブ（総資産額・円グラフ・日付ピッカー・表） |
| `asset-composition-treemap.png` | asset-composition | 「資産構成」タブで「ツリーマップ」を選んだ状態 |
| `currency-settings.png` | currency | 「設定」→「通貨・レート」画面全体 |
| `currency-rate-row.png` | currency | 「通貨レート設定」の入力欄（⟳ と ✓ ボタンが見える部分） |
| `backup.png` | backup | 「設定」→「バックアップ」画面 |
| `backup-list.png` | backup | 「バックアップ一覧から復元」画面（自動・手動のバックアップが数件ある状態） |
| `auto-backup.png` | backup | 「自動バックアップ」画面（有効・間隔・古い自動バックアップの削除） |
| `backup-share-sheet.png` | backup | 「データのエクスポート」をタップしたときの iOS 共有シート |
| `data-import.png` | data-import | 「設定」→「データ移行」画面 |
| `data-import-review.png` | data-import | 「取り込み内容の確認」画面（「既存」「新規」の行が見える状態） |
| `ai-bulk-create.png` | ai | 「資産一覧」→「まとめて登録」で読み取った後の確認の一覧 |
| `settings.png` | settings | 「設定」タブ全体 |
| `settings-skin.png` | settings | 「設定」→「スキン」画面（スキンの見本が並んだ状態） |
| `settings-goal.png` | settings | 「資産目標」画面（目標金額・達成したい年と「チャートに目標額を表示する」） |
| `upgrade.png` | premium | 「設定」→「アップグレード」画面 |

## Android 版を追加する場合

Android 用のスクリーンショットは `images/ja/android/`・`images/en/android/` に、同じファイル名で保存することを推奨します。
