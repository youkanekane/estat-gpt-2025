# e‑Stat API + ChatGPT Actions 連携（概要ページ）

このリポジトリは、ChatGPT のカスタムGPT（Actions）から **政府統計 e‑Stat API** を呼び出して、
「何を（指標）・どこを（地域）・いつ（期間）」を指定して統計を取得するためのプロジェクトです。

## 使い道
- ChatGPTに「政府統計で◯◯を新潟県・2020年で」と話しかけると、APIで取得して表にまとめます。

## 技術メモ
- 使用API：e‑Stat REST API（JSON）
- 認証：`appId`（クエリパラメータ）。**このページには appId を公開しません。**
- 取得手順：getStatsList → getMetaInfo → getStatsData（必要に応じて NEXT_KEY で分割取得）

## 注意
- ここは**公開ページ**です。秘密の情報（APIキー・個人情報）は載せません。
- データの正確性は元の政府統計に依存します。

## 連絡
- 管理者：あなたの名前（または連絡先）
