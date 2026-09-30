# 下書き: 広告（Google AdMob）を入れる時の規約・ポリシーの変更

> **このファイルは下書きです。** `pages/` の外にあるため、サイトには取り込まれません。
> 広告を入れたアプリを公開するときに、下の文案を各ページに反映してください。
> それまでは反映しないでください（アプリの実際の動作と、規約・ポリシーの内容が食い違ってしまうため）。

## 反映するときのチェックリスト

- [ ] パーソナライズド広告（興味に合わせた広告）を使うかを決め、下の文案の【パーソナライズド広告を使う場合】の部分を残すか削除する
- [ ] 利用規約（日本語・英語）に「第9条の2（広告）」を追加する
- [ ] プライバシーポリシー（日本語・英語）の「6.」を差し替え、「6-2.」を追加する
- [ ] アプリ側
  - [ ] AdMob の組み込みと、プレミアム利用中は広告を表示しない処理
  - [ ] EU・英国の利用者向けの同意画面（Google の UMP SDK）
  - [ ] 【パーソナライズド広告を使う場合】トラッキングの許可の確認（ATT）と、Info.plist の `NSUserTrackingUsageDescription`
- [ ] App Store Connect の「Appのプライバシー」を更新する（識別子・使用状況データ・診断などの収集。パーソナライズド広告を使う場合は「トラッキングに使用」）
- [ ] マニュアルの更新: プレミアムのページ（「広告の非表示」を追加）、よくある質問（「データはどこに保存されますか」に広告の説明を追加）
- [ ] プライバシーポリシーの変更は、第9条（本ポリシーの変更）に従い、効力発生日を定めて事前に告知する（アプリ公開前なら不要）

---

## 利用規約（日本語）: 追加する条文

第9条（知的財産権）の後に追加します（番号を振り直さないよう「第9条の2」とします）。

```markdown
## 第9条の2（広告）

1. 本アプリには、運営者または第三者（Google LLC などの広告配信事業者を含みます。）による広告が表示される場合があります。
2. 広告の内容、広告からリンクされたウェブサイトやアプリ、広告主の商品・サービスについて、運営者はその内容を保証しません。利用者と広告主との間で生じた取引や紛争について、運営者は、第11条第1項に定める場合を除き、責任を負いません。
3. プレミアムを利用している間は、本アプリ内の広告は表示されません。
4. 広告の配信に伴う情報の取扱いは、プライバシーポリシーに定めるとおりとします。
```

## 利用規約（英語）: 追加する条文

```markdown
## Article 9-2 (Advertising)

1. Advertisements by the Operator or third parties (including advertising providers such as Google LLC) may be displayed in the App.
2. The Operator does not guarantee the content of advertisements, websites or apps linked from advertisements, or advertisers' products or services. The Operator is not liable for any transaction or dispute between the User and an advertiser, except as provided in Article 11, paragraph 1.
3. Advertisements are not displayed in the App while the User is using Premium.
4. Information handled in connection with advertising is as set out in the Privacy Policy.
```

---

## プライバシーポリシー（日本語）

### 「6. 解析ツール・広告・トラッキング」を差し替え

```markdown
## 6. 解析ツール・広告・トラッキング

本アプリは、利用状況の解析ツールを使用していません。
本アプリは、次の「6-2. 広告の配信」に記載する広告配信サービスを使用しています。
```

### 「6-2. 広告の配信」を追加

```markdown
## 6-2. 広告の配信

本アプリは、Google LLC が提供する広告配信サービス「Google AdMob」を使用して広告を表示します（プレミアム利用中は表示しません）。

- 広告の配信のため、端末の広告識別子（iOS の IDFA など）、IP アドレス、端末の種類や OS のバージョン、広告の表示・タップの状況などの情報が、Google に送信される場合があります。
- これらの情報は、広告の配信、広告の効果の測定、不正な広告操作の防止のために、Google が利用します。
- 本アプリに入力された資産や残高などのデータは、Google を含む広告配信事業者に送信しません。
- Google による情報の取扱いについては、[Google のプライバシーポリシー](https://policies.google.com/privacy)と[Google の広告に関するページ](https://policies.google.com/technologies/ads)をご覧ください。

【パーソナライズド広告を使う場合】
- 利用者の興味に合わせた広告（パーソナライズド広告）を表示する場合があります。iOS では、最初に表示される「トラッキングを許可しますか？」の確認で許可した場合にのみ、広告識別子をパーソナライズド広告に使用します。許可しなかった場合は、興味に合わせない広告が表示されます。
- 欧州経済領域（EEA）・英国などの利用者には、広告のための情報の利用について、同意の確認を表示します。

### 広告のための情報の利用を止める方法（オプトアウト）

- iPhone: 「設定」→「プライバシーとセキュリティ」→「トラッキング」で、本アプリのトラッキングをオフにしてください。
- Android: 端末の設定で、広告 ID を削除またはリセットしてください。
- [Google の広告設定](https://adssettings.google.com/)で、パーソナライズド広告をオフにすることもできます。
```

## プライバシーポリシー（英語）

### Replace "6. Analytics, advertising, and tracking"

```markdown
## 6. Analytics, advertising, and tracking

The App does not use analytics tools.
The App uses the advertising service described in "6-2. Advertising" below.
```

### Add "6-2. Advertising"

```markdown
## 6-2. Advertising

The App displays advertisements using Google AdMob, an advertising service provided by Google LLC (advertisements are not displayed while you are using Premium).

- To deliver advertisements, information such as your device's advertising identifier (such as the IDFA on iOS), IP address, device type and OS version, and advertisement impressions and taps may be sent to Google.
- Google uses this information to deliver advertisements, measure their effectiveness, and prevent fraudulent activity.
- Data you enter in the App, such as assets and balances, is not sent to Google or any other advertising provider.
- For how Google handles information, see [Google's Privacy Policy](https://policies.google.com/privacy) and [How Google uses information from sites or apps that use its services](https://policies.google.com/technologies/ads).

[If personalized ads are used]
- Advertisements tailored to your interests (personalized ads) may be displayed. On iOS, your advertising identifier is used for personalized ads only if you allow tracking when asked "Allow this app to track your activity?". If you do not allow it, non-personalized ads are displayed.
- Users in the European Economic Area (EEA), the UK, and similar regions are asked for consent to the use of information for advertising.

### How to opt out of the use of information for advertising

- iPhone: Go to Settings → Privacy & Security → Tracking and turn off tracking for the App.
- Android: Delete or reset your advertising ID in your device settings.
- You can also turn off personalized ads in [Google's My Ad Center](https://adssettings.google.com/).
```
