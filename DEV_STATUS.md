# CA Policy Analyzer Web — 開発状況

## 最終更新
2026-03-02

## 現在のフェーズ
GitHub Pages 運用中 — Store 審査用のプライバシーポリシー・サポートページ・ユーザーマニュアルを公開

## サイト構成

### 既存ページ（Store 審査提出済み — 変更禁止）
- `index.html` — 製品紹介ページ（日英切替対応）
- `privacy-policy.html` — プライバシーポリシー（日英切替対応）
- `support.html` — サポートページ（日英切替対応）
- `sample-policies-for-review.json` — Store 審査用サンプルデータ
- `CNAME` — カスタムドメイン設定 (`app.sumikkolab.com`)

### マニュアル（2026-03-02 追加）
- `manual/styles.css` — 共有スタイルシート
- `manual/index.html` — 目次
- `manual/getting-started.html` — Ch.1: はじめに
- `manual/policy-management.html` — Ch.2: ポリシー管理
- `manual/simulation.html` — Ch.3: シミュレーション
- `manual/gap-analysis.html` — Ch.4: 乖離チェック
- `manual/coverage-analysis.html` — Ch.5: カバレッジ分析
- `manual/diagnostics.html` — Ch.6: 診断
- `manual/change-history.html` — Ch.7: 変更履歴
- `manual/design-document-export.html` — Ch.8: 設計書エクスポート
- `manual/named-locations.html` — Ch.9: ネームドロケーション
- `manual/analysis-settings.html` — Ch.10: 分析設定
- `manual/licensing.html` — Ch.11: ライセンス
- `manual/troubleshooting.html` — Ch.12: FAQ

## 検証状況
- 全12章 × 日英2言語 = 24ページ: 全 PASS（2026-03-02 確認済み）
- 言語切替（switchLang + ?lang=en パラメータ）: 正常動作
- 章間ナビゲーション（前章/次章リンク）: 全リンク正常

## 次に予定していること
1. Store 審査通過後: 既存ページ（index.html, support.html）にマニュアルへのリンクを追加
2. スクリーンショットの追加（マニュアル各章に実際の画面キャプチャ）
3. アップデート通知機能（version.json + UpdateCheckService）— 設計のみ完了、審査後に実装

## ブロッカー・メモ
- Store 審査中のため、既存ページ（index.html, privacy-policy.html, support.html, sample-policies-for-review.json）は変更禁止
- マニュアルの新規追加は審査に影響しないため実施済み
