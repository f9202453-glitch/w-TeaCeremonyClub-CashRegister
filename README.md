# 🍵 茶道部 会計レジシステム 説明書

学園祭のお茶会会計をスムーズにし、複数端末で売上をリアルタイム共有するためのWebアプリです。
（HTML/JS + Google Firebase + GitHub Pages で構築 / Google AI Studio を活用して開発）

---

## 📱 【当日使う人向け】基本の使い方

### 1. アプリの開き方
- URL: `https://f9202453-glitch.github.io/w-TeaCeremonyClub-CashRegister/`

### 2. 会計の手順
1. 上部で「1日目 / 2日目」と「現在の席（第◯席）」を選ぶ。
2. 「人数」をタップ（5名以上の場合は入力欄に直接打ち込む）。
3. 「お預かり金額」をタップ（または直接入力）。
4. お釣りを確認して「会計完了」を押す。
   ※他の端末ともリアルタイムで合計売上が同期されます。

### 3. よくあるトラブル対応
- **打ち間違えた！**:
  - 画面下の「直近の会計」一覧にある赤い **[取消]** ボタンを押すと、その会計を取り消せます。
- **席料が変わった場合**:
  - 右上の **[⚙ 設定]** をタップ ➔ 新しい金額を入力して「保存」を押せばOKです。
- **「オフライン動作中」と表示されたら**:
  - 学祭の混雑で一時的に電波が弱くなっていますが、**そのまま会計を続けて大丈夫です**。電波が戻ったら裏で勝手に同期されます。

### 4. 終了後（売上の保存・印刷）
- 画面下の **[売上データをCSV保存]** を押すと、全データがダウンロードされます。
- パソコンで開けばExcelで印刷・集計できます。

### 🌐 Quick English Guide
1. Open the URL on your mobile browser.
2. Select the number of guests and amount received.
3. Tap [会計完了 (Complete)] to submit.
4. To cancel a mistaken order, tap [取消 (Cancel)] in the history list below.
---

## ⚙ 【来年度の管理者向け】引き継ぎ・管理情報

### 1. 本番前にやること（超重要）
- **テストデータの全消去**:
  - 事前に部員でレジの練習をしたデータが残っている場合は、画面右上の **[⚙ 設定]** ➔ **[⚠️ 売上データを全てリセットする]** を押し、「リセット」と入力して本番前にまっさらにしてください。

### 2. アカウントと管理場所
- **コード管理（GitHub）**:
  - プログラムの保管場所・管理ページ（リポジトリURL）: https://github.com/f9202453-glitch/w-TeaCeremonyClub-CashRegister
  - コードは `index.html` 1ファイルだけで完結しています。
- **データベース（Google Firebase）**:
  - 管理画面: https://console.firebase.google.com/
  - ログインアカウント: `wteaceremony@gmail.com`
  - ログインパスワード：`vynnak-winsuZ-9fytxo`

### 3. アプリを改造・修正したい場合
- ボタンを増やしたい、メニューを追加したいなどの改修は、**GeminiやChatGPTなどのAIに `index.html` のコードを丸ごと貼り付けて、「〇〇という機能を追加して」と頼むだけ**で誰でも簡単に直せます！
