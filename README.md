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
  - 次回イベント
  - イベントレポート
  - ロードマップ
  - 参加する

#### セクション

**ヒーロー（Hero）**
- キャッチコピー：「孤独な試行錯誤を終わらせる。」
- コミュニティの説明文
- グラデーション背景（グリーン）

**About セクション**
- RECOREコミュニティとは（冒頭テキスト：18px大）
- コミュニティで得られるもの（4項目）：
  - 継続的なビジネス成果を創出する土台
  - 他のRECOREユーザーとの情報交換・相談
  - 活用事例・成功事例の共有
  - 業者間取引の斡旋
- 基本ルール

**Next Events セクション**
開催予定イベント2つ：
- **関東コミュニティ Vol.3**
  - 日程：2026年5月18日～22日（候補）
  - 場所：東京都内（詳細未定）
  
- **関西コミュニティ Vol.1**
  - 日程：2026年 開催予定
  - 場所：大阪・兵庫エリア（詳細未定）

**Event Reports セクション**
過去のイベントレポート3件：
- Vol.1（関東）：Liquidと生成AIを活用した出品効率化
- Vol.2（関東）：LINEミニアプリと会員ランク制度によるLTV最大化戦略
- Vol.1（関西）：第1回RECORE関西コミュニティレポート

**Roadmap セクション**
コミュニティの3段階進化：
- **Phase 1「繋がる」（現在進行中）** — Slack＆オフラインイベント
- **Phase 2「深掘り」** — テーマ別分科会による共創
- **Phase 3「創る」** — RECORE開発チームとの共同開発パートナーシップ

**Join Us セクション**
- コミュニティ参加のメリット（5項目）
- 参加方法の詳細：
  - 参加資格：RECOREをご利用中の企業様
  - 参加費：無料（イベント2次会は有料の場合あり）
  - 活動形式：オフラインイベント + Slack交流
  - お問い合わせ：seino@recore-corp.jp

### 2. イベントレポート（report.html）

第1回RECORE関西コミュニティイベントのレポートページ

- **開催日時** — 2026年6月5日（金）17:00～19:00
- **開催場所** — NEXT51 三国ヶ丘店（堺市）
- **参加者数** — 6名
- **参加企業** — 3社

セクション：
- 開催概要（詳細テーブル）
- イベント概要（目的・こだわり）
- タイムテーブル（4つのセッション）
- イベント当日の様子（ギャラリー）
- 参加者の声（4つのコメント）
- まとめ

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

変更は自動的に GitHub Pages で公開されます（数秒以内）。

## お問い合わせ

📧 **seino@recore-corp.jp**

## ライセンス

© 2026 RECORE Community by 株式会社RECORE. All rights reserved.

---

**更新日** — 2026年6月17日  
**管理者** — RECORE カスタマーサクセスチーム
