# RECORE Community Portal Site

RECOREコミュニティの全体ポータルサイトです。リユース業界のプロフェッショナルが知見を共有し、共に成長する「成長の生態系」を紹介しています。

**公開URL:** https://ueda-recore.github.io/recore-portalsite/

## サイト概要

孤独な試行錯誤を終わらせ、リユース業界全体の発展を目指すRECOREコミュニティの公式ポータルサイト。全国のRECOREユーザーが参加でき、オフラインイベントとSlackでのオンライン交流を通じて、実践的なノウハウを共有できるプラットフォームです。

## ページ構成

### 1. トップページ（index.html）

#### ナビゲーション
- RECORE Community ロゴ
- メニュー項目：
  - コミュニティとは
  - ビジョン
  - 次回イベント
  - イベントレポート
  - ロードマップ
- 参加するボタン（ゴールド）

#### セクション

**ヒーロー（Hero）**
- キャッチコピー：「孤独な試行錯誤を終わらせる。」
- コミュニティの説明文
- Call-to-Action ボタン：2つ
  - コミュニティに参加する
  - イベントレポートを見る
- 統計情報：
  - 83% 業務効率化実績
  - 100+ 参加企業
  - 定期開催 全国イベント

**About セクション**
- RECOREコミュニティとは
- コミュニティで得られるもの（4項目）
- 基本ルール

**Vision セクション**
- 共有・解決・共創・信頼（4つのビジョンカード）

**Next Events セクション**
- 関東コミュニティ Vol.3（2026年5月18日～22日候補）
- 関西コミュニティ Vol.1（2026年開催予定）

**Event Reports セクション**
- Vol.1（関東）：Liquidと生成AI活用
- Vol.2（関東）：LINEミニアプリとLTV最大化
- Vol.1（関西）：第1回関西コミュニティレポート

**Roadmap セクション**
- Phase 1「繋がる」（現在進行中）
- Phase 2「深掘り」
- Phase 3「創る」

**Join Us セクション**
- 参加メリット（5項目）
- 参加方法の詳細
- お問い合わせ：seino@recore-corp.jp

### 2. イベントレポート（report.html）

第1回RECORE関西コミュニティイベントのレポートページ
- 開催日時：2026年6月5日（金）17:00～19:00
- 開催場所：NEXT51 三国ヶ丘店（堺市）
- 参加者数：6名

## デザイン仕様

### カラースキーム
- グリーン（深）：#1E3A14
- グリーン（中）：#2D4E1C
- ゴールド：#C4D44A
- テキスト：#2C2C2C

### フォント
- 見出し：Zen Kaku Gothic New（900 weight）
- 本文：Noto Sans JP（400/500/700 weight）

### レスポンシブ
- デスクトップ対応（1200px以上）
- モバイル対応（768px以下）
- Fade-inアニメーション実装

## ファイル構成

\\\
recore-portalsite/
├── README.md           # このファイル
├── index.html          # 全体ポータルサイト
└── report.html         # 関西コミュニティイベントレポート
\\\

## 関連リポジトリ

- **関西コミュニティ** — https://github.com/seino-jpg/recore-community-kansai
- **関東コミュニティ** — recore-community-kanto（準備中）

## セットアップ

### ローカル開発

\\\ash
git clone https://github.com/ueda-recore/recore-portalsite.git
cd recore-portalsite
python -m http.server 8080
# http://localhost:8080/index.html
\\\

## GitHub Pages

- **公開URL** — https://ueda-recore.github.io/recore-portalsite/
- **ブランチ** — main
- **ビルドタイプ** — Static HTML

## 更新方法

\\\ash
git add .
git commit -m "Update: [変更内容]"
git push origin main
\\\

## お問い合わせ

📧 **seino@recore-corp.jp**

## ライセンス

© 2026 RECORE Community by 株式会社RECORE. All rights reserved.

---

**更新日** — 2026年6月17日  
**管理者** — RECORE カスタマーサクセスチーム
