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
- **関東コミュニティ Vol.4 — ブックオフ出品倉庫 見学会**
  - 日程：2026年10月19日（月）12:00〜17:00 ※仮
  - 場所：東名横浜ロジスティクスセンター（神奈川県横浜市瀬谷区北町25-9）
  - 内容：ささげ・EC出品・ピッキング・梱包・出荷のオペレーション見学

- **関西コミュニティ Vol.2**
  - 日程：準備中
  - 場所：準備中

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

### 2. 参加申し込み（apply.html）

イベントカードの「参加を申し込む」ボタンから遷移する専用ページ。

- 対象イベント：関東コミュニティ Vol.4（ブックオフ出品倉庫 見学会）
- 入力項目：会社名・お名前・メールアドレス・電話番号・懇親会の参加（参加する／参加しない）が必須、ご質問・ご要望は任意
- 送信先は Google Apps Script のWebアプリ（`APPLY_ENDPOINT` 定数で指定）
- 申し込み内容はスプレッドシート「RECOREコミュニティ 参加申し込み」のイベント別タブ（現在は `【関東】vol.4`）に追記される
- 申込者へ自動返信メールを送信、運営へは Slack「recoreコミュニティ運営」チャンネルに通知（Slackが使えないときはメールにフォールバック）
- GAS のソースは `~/gas-community-form`（clasp管理）

### 3. イベントレポート（report.html）

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
└── apply.html          # 参加申し込みフォーム（関東 Vol.4）
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
