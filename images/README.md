# スクリーンショット撮影リスト

マニュアル本文で参照しているスクリーンショットの一覧です。
本文からは `https://raw.githubusercontent.com/shibatype1999/assett-manual/main/images/…` の形で参照しているため、画像は `main` ブランチに反映されると表示されます。
下の表のファイル名で、`images/ja/`（日本語UI）と `images/en/`（英語UI）にそれぞれ保存してください。
ファイル名は日本語版・英語版で共通です。

## 撮影のポイント

- **端末**: iPhone（全画像で同じ機種にそろえると、見た目が統一されます）
- **形式**: PNG
- **言語**: `ja/` はアプリの言語を「日本語」、`en/` は「English」にして撮影します（「設定」→「言語」）。
- **テーマ**: 「ライト」で統一することをおすすめします。
- **データ**: 見本用のデータ（架空の金額）を入力した状態で撮影します。個人の実際の資産が写らないようご注意ください。
  - 例: 資産「A銀行」「B銀行」「C証券」「米国株（米ドル）」「住宅ローン（負債）」、それぞれ数か月分の記録
  - 記録にサブカテゴリ（給料・評価額など）を付けておくと、増減要因のグラフが写ります。
  - 資産目標も設定しておくと、達成率や目標ラインが写ります。
  - プレミアムの機能（積み上げグラフ・自動バックアップなど）は、プレミアムが有効な状態で撮影します。
- **ステータスバー**: 時刻・電波・電池などが気になる場合は、トリミングしてもかまいません。

## 撮影リスト

| ファイル名 | 使用ページ（`pages/<言語>/…`） | 撮影する画面 |
| --- | --- | --- |
| `dashboard.png` | index / dashboard | 「ダッシュボード」タブ（総資産額・資産比率・資産別の総額のパネル） |
| `tab-bar.png` | getting-started | 画面下部のタブ（5つのタブが見えるように） |
| `dashboard-edit.png` | dashboard | ダッシュボードの編集モード（パネル一覧と「パネルを追加」） |
| `input.png` | recording | 「入力」タブ（資産一覧・残高・前月比） |
| `record-form.png` | recording | 資産の記録一覧で「新規登録」をタップした「残高を記録」画面 |
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
| `settings.png` | settings | 「設定」タブ全体 |
| `settings-goal.png` | settings | 「資産目標」画面（目標金額と「チャートに目標額を表示する」） |
| `upgrade.png` | premium | 「設定」→「アップグレード」画面 |

## Android 版を追加する場合

Android 用のスクリーンショットは `images/ja/android/`・`images/en/android/` に、同じファイル名で保存することを推奨します。
