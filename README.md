# 縁線 ENSEN — ポップアップイベント告知LP

蒲郡駅コンコースで開催するポップアップイベント「縁線(ENSEN)」の告知用ランディングページ。
HTML / CSS / JavaScript を `index.html` 1ファイルにまとめた静的サイト。外部ライブラリ不使用(Google Fonts のみ)。

## 構成
- `index.html` … ページ本体(全セクション・CSS・JS)
- `images/placeholder.svg` … 画像未配置時に自動表示される仮画像
- `images/favicon.svg` … ファビコン(仮)
- `images/*.jpg` … **未配置**。差し替え必須(一覧は index.html 冒頭コメント参照)

## セクション
1. ファーストビュー(ロゴ / 日程 / 時間 / 会場 / メインビジュアル)
2. コンセプト(名前の由来)
3. 出店者紹介(伴装有限会社 / 有限会社ナカモリ)
4. 商品ギャラリー(6枚、最大9枚まで拡張可)
5. 開催概要(表 + Googleマップ埋め込み)
6. フッター(問い合わせ / SNS / 主催)

## 技術メモ
- モバイルファースト(375px基準)、PC 1080px コンテナ
- `prefers-reduced-motion` 対応のフェードイン(IntersectionObserver)
- 画像 404 時は JS で `images/placeholder.svg` に差し替え
- OGP / meta description / favicon 設定済み(og:url は要変更)
- データ保存・DB なし

## 残作業(公開前)
- 【要記入】箇所の記入(本文中を「要記入」で検索)
- 画像の配置(hero / bansou_01 / nakamori_01 / gallery_01〜06 / ogp)
- 「入場無料・予約不要」の行は事実確認のうえ必要なら削除
- og:url を公開URLに変更、og:image を絶対URLに

## 公開
未公開。Netlify Drop または Hosted Deploy で公開可能。
