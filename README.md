# Team Kakusin. Official Website

## 概要
これは同人サークル「Team Kakusin.」の公式Web サイトです。

GitHub Pages を使用し、パスワード保護���れた GUI エディタのみによるサイト編集を実現しています。

## 機能

✨ **完全無料** - GitHub のみを使用  
🔐 **パスワード保護** - GUI管理画面でセキュアに編集  
📝 **コーディング不要** - ブラウザのみで全機能を操作  
🚀 **自動デプロイ** - 編集後すぐに反映  
📱 **レスポンシブ** - 全デバイス対応  
🎨 **モノクロデザイン** - シンプル＆洗練  

## ファイル構成

```
.
├── index.html                    # メインサイト
├── admin/
│   └── index.html               # パスワード保護された管理画面
├── _data/
│   ├── site-config.json         # サイト基本情報
│   ├── about.json               # サークル紹介
│   ├── members.json             # メンバー情報
│   ├── songs.json               # 楽曲情報
│   └── social-links.json        # SNSリンク
└── README.md
```

## セットアップ手順

### 1️⃣ GitHub Pages を有効化

1. リポジトリの **Settings** → **Pages**
2. Source: **Deploy from a branch** を選択
3. Branch: **main** を選択
4. **Save** をクリック
5. 数分待つと `https://exe-joemae.github.io/Xx_TEKITOU-NAME_xX/` で公開されます

### 2️⃣ 管理画面へアクセス

`https://exe-joemae.github.io/Xx_TEKITOU-NAME_xX/admin/` にアクセス

**パスワード:** `teamjoekita`

## 使用方法（メンバー向け）

### 📋 管理画面にアクセス

1. `https://exe-joemae.github.io/Xx_TEKITOU-NAME_xX/admin/` を開く
2. パスワード `teamjoekita` を入力してログイン
3. タブから編集したい項目を選択
4. フォームに情報を入力
5. **保存** ボタンをクリック

### 📝 編集可能な内容

#### **サイト設定**
- サークル名（英字・ひらがな）
- サイトタイトル
- サイト説明文

#### **サークル紹介**
- タイトル
- 説明文（Markdown対応）
- 設立年

#### **メンバー紹介**
- メンバー名（最大6人）
- 役割
- 自己紹介
- Twitter/pixiv へのリンク

#### **新曲情報**
- 楽曲名
- アーティスト名
- 説明
- 公開日
- YouTube/ニコニコ動画/SoundCloud へのリンク

#### **SNSリンク**
- Twitter
- YouTube
- pixiv
- その他 SNS

## 編集方法の詳細

### ✏️ 管理画面から編集

1. 対応するタブをクリック
2. フォームに情報を入力
3. 各フォーム下部または最下部の **保存** ボタンをクリック
4. 成功メッセージが表示されたら完了

### 🔄 変更内容の反映

保存後、以下の流れで自動的にサイトに反映されます：

1. 管理画面で **保存** をクリック
2. GitHub Web Editor で内容を確認・コミット
3. GitHub Pages が自動ビルド
4. 数秒～1分で公開サイトに反映

## トラブルシューティング

### 管理画面が真っ白
- ブラウザのキャッシュをクリア（Ctrl+Shift+Del）
- ページを再読み込み（Ctrl+R または F5）

### ログインができない
- パスワードが正しいか確認（`teamjoekita`）
- 大文字小文字を区別するため、正確に入力

### 編集内容が反映されない
- GitHub Web Editor でコミットを確認
- Settings → Pages でデプロイ状況を確認
- ブラウザキャッシュをクリア

### 404 エラーが出る
- サイトが正しく公開されているか確認
- Settings → Pages で "Your site is published at" を確認
- URL が正しいか確認

## 技術詳細

### 使用技術
- **ホスティング**: GitHub Pages
- **フロントエンド**: HTML5 + CSS3 + Vanilla JavaScript
- **データ形式**: JSON
- **CMS**: カスタム GUI エディタ

### セキュリティ
- パスワードはローカル認証（ブラウザ内）
- HTTPS で暗号化通信
- GitHub の権限管理でコンテンツを保護

## デザインのカスタマイズ

### 色の変更
`index.html` の `<style>` セクションを編集：

```css
/* メイン色（黒）を変更する場合 */
color: #000000;  /* ← この値を変更 */

/* 背景色（白）を変更する場合 */
background-color: #ffffff;  /* ← この値を変更 */
```

### フォントの変更
```css
font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
/* ↑ このフォント設定を変更 */
```

### レイアウトの変更
メンバーグリッド、楽曲カードなど、各セクションのスタイルを編集

## ライセンス

MIT License - 自由に使用、改変、配布できます。

---

**制作日**: 2026年6月2日  
**提供**: GitHub Copilot
