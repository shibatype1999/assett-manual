# 資産管理アプリ マニュアル

資産管理アプリ（開発リポジトリ: `assett`）の**利用者向け操作マニュアル**です。
Bludit の **Remote Content** プラグインで取り込み、サイトとして公開することを想定した構成になっています。

- 対応OS: **iOS**（Android は今後追加予定）
- 対応言語: **日本語** / **英語**（ほかの言語は今後追加予定）

## フォルダ構成

```
assett-manual/
├── README.md                  … このファイル（Bludit には取り込まれません）
├── pages/                     … Bludit に取り込まれるページ
│   ├── ja/                    … 日本語版
│   │   ├── index.md           … 親ページ（トップ・目次）   → /ja
│   │   ├── getting-started/
│   │   │   └── index.md       … 子ページ                   → /ja/getting-started
│   │   ├── dashboard/index.md
│   │   ├── recording/index.md
│   │   ├── assets/index.md
│   │   ├── categories/index.md
│   │   ├── chart/index.md
│   │   ├── asset-composition/index.md
│   │   ├── currency/index.md
│   │   ├── backup/index.md
│   │   ├── settings/index.md
│   │   ├── premium/index.md
│   │   └── faq/index.md
│   ├── en/                    … 英語版（ja/ と同じ構成・同じフォルダ名）
│   ├── privacy-policy/        … プライバシーポリシー（日本語）→ /privacy-policy、en/ に英語版
│   └── terms-of-service/      … 利用規約（日本語）→ /terms-of-service、en/ に英語版
├── images/                    … スクリーンショット（Bludit には取り込まれず、GitHub から直接表示）
│   ├── README.md              … 撮影リスト
│   ├── ja/
│   └── en/
└── bludit/plugins/
    └── language-redirect/     … トップページをブラウザの言語に合わせて /ja・/en へ転送するプラグイン
```

## Bludit で読み込まれるしくみ

Remote Content プラグインは、指定した zip ファイルをダウンロードし、次のルールでページを作成します。

- zip の中の `pages/<親>/index.md` が**親ページ**、`pages/<親>/<子>/index.md` が**子ページ**になります（2階層まで）。
- **フォルダ名がそのままURL（スラッグ）**になります。例: `pages/ja/chart/index.md` → `https://サイト/ja/chart`
- ファイルの**1行目の `# 見出し`がページタイトル**になります。
- 2行目から続く `<!-- 項目: 値 -->` の行は、ページの設定として読み込まれます。

```markdown
# ページタイトル
<!-- position: 3 -->
<!-- description: ページの説明文（検索結果などに使われます） -->

本文…
```

| 項目 | 内容 |
| --- | --- |
| `position` | 並び順（小さい順）。親ページは言語の順、子ページは章の順にしています。 |
| `description` | ページの説明文。 |
| `type` | 必要に応じて追加できます（`published` / `static` など）。子ページは親ページの `type` を引き継ぎます。 |

> **注意**
> - `<!-- … -->` の行は**タイトルの直後に、空行を入れずに**書いてください。空行があると、それ以降は本文として扱われます。
> - 本文は Markdown として表示されます（Bludit の設定「Markdown parser」が有効な場合。初期設定は有効）。

## Bludit の設定手順

1. このリポジトリを **Public（公開）** にします。
   Bludit は認証なしで zip と画像をダウンロードするため、非公開のままだと取り込めず、画像も表示されません。
2. 変更を `main` ブランチに反映します。
3. Bludit の管理画面で **Remote Content** プラグインを有効にし、次のように設定します。
   - **Source**: `https://github.com/shibatype1999/assett-manual/archive/refs/heads/main.zip`
   - **Webhook**: 自動で生成された文字列のままでかまいません。
4. 「Try webhook」をタップすると、取り込みが実行されます。
   以後、マニュアルを更新したら Webhook のURL（`https://サイト/<Webhook の文字列>`）にアクセスすると再取り込みされます。
   GitHub の Webhook（リポジトリの Settings → Webhooks）にこのURLを登録すると、`main` へのプッシュ時に自動で更新されます。
5. トップページ（`https://サイト/`）を開いた人をブラウザの言語に合わせて `/ja`・`/en` へ転送するには、[Language Redirect プラグイン](bludit/plugins/language-redirect/README.md) をサーバーに設置します。

> **ご注意**
> 取り込みを実行すると、**Bludit に登録されている既存のページとアップロード済みの画像はすべて削除**され、このリポジトリの内容に置き換わります。
> Bludit 上で直接作成・編集したページは消えるため、ページの追加や修正は必ずこのリポジトリで行ってください。

## 執筆ルール

- **フォルダ名（スラッグ）は全言語で共通**にします。例: 日本語 `pages/ja/chart/`、英語 `pages/en/chart/`
- スラッグは半角英小文字とハイフンで付けます（URLになるため）。
- アプリの画面上の文言は「」（英語版は **太字**）で囲み、アプリ内の表記と一致させます。
- **ページ間のリンク**
  - 子ページから同じ言語の別の子ページへ: スラッグだけを書きます。例: `[カテゴリを管理する](categories)`
  - 親ページ（`pages/<言語>/index.md`）から子ページへ: `言語/スラッグ` と書きます。例: `[カテゴリを管理する](ja/categories)`
  - 見出しへのリンク（`#…`）は Bludit では使えないため、書かないでください。
- **画像**は GitHub 上のファイルを絶対URLで参照します（取り込み時に Bludit のアップロード画像が削除されるため）。
  ```markdown
  ![入力タブ](https://raw.githubusercontent.com/shibatype1999/assett-manual/main/images/ja/home.png)
  ```

## 画像（スクリーンショット）について

本文には画像のURLがすでに入っています。撮影が必要な画像の一覧は [images/README.md](images/README.md) を参照してください。
画像を所定のファイル名で `images/ja/`・`images/en/` に置き、`main` ブランチに反映すると表示されます。

## 言語を追加するには

1. `pages/ja/` フォルダをコピーして、言語コード名のフォルダ（例: `pages/ko/`）を作ります。
2. 各ファイルを翻訳します。子ページのフォルダ名は変えません。
3. 親ページ（`pages/<言語>/index.md`）の目次リンクを `ko/…` のように書き換え、`position` を既存の言語の後ろの番号にします。
   Language Redirect プラグインの設定画面で、「対応言語」にも追加します（例: `ja,en,ko`）。
4. `images/<言語コード>/` を作ってその言語のUIで撮影したスクリーンショットを置き、画像URLの `/images/ja/` を `/images/<言語コード>/` に置き換えます。
5. 画面上の文言は、アプリ側の翻訳ファイル（`assett` リポジトリの `lib/l10n/app_<言語>.arb`）の表記に合わせます。

## Android 版を追加するには

操作の大部分は iOS と Android で共通です。OS によって操作が異なる箇所は、同じページの中で次のような見出しで書き分けます。

```markdown
### iOS の場合
…
### Android の場合
…
```

現在 OS ごとに違いが出るのは、主に次の箇所です。

- `pages/<言語>/backup/index.md`（共有シート・ファイル選択画面）
- `pages/<言語>/faq/index.md` の機種変更に関する項目
- `pages/<言語>/premium/index.md`（App Store でのサブスクリプションの購入・解約）

Android 用のスクリーンショットは `images/<言語>/android/` に置くことを推奨します。

## 未確定の項目

- アプリの「プライバシーポリシー」「利用規約」は `https://asset.fubuki.info/privacy-policy`・`https://asset.fubuki.info/terms-of-service` を開きます。これらは `pages/privacy-policy/`・`pages/terms-of-service/`（日本語）と、その下の `en/`（英語、`/privacy-policy/en` など）で管理しています。**フォルダ名を変えるとアプリのリンクが切れる**ので注意してください。

## 用語

マニュアルの用語は、アプリの画面表示に合わせています。

| 用語 | 意味 |
| --- | --- |
| 資産 | 残高を記録する単位（例: A銀行、B証券）。以前のバージョンの「カテゴリ」 |
| カテゴリ | 資産をまとめるグループ（例: 預金・現金）。以前のバージョンの「グループ」 |
| サブカテゴリ | 記録1件ごとに付けるラベル（例: 給料、評価額） |
