# Team Kakusin. Official Website

## 概要
これは同人サークル「Team Kakusin.」の公式Webサイトです。

GitHub Pages + Decap CMS を使用して、パスワード保護下でGUIのみによるサイト編集を実現しています。

## 機能

✨ **完全無料** - GitHub + Netlify の無料プランを使用  
🔐 **パスワード保護** - GitHub OAuth認証でセキュア  
📝 **GUIエディタ** - コーディング知識不要  
🚀 **自動デプロイ** - 編集後すぐに反映  
📱 **レスポンシブ** - 全デバイス対応  
🎨 **モノクロデザイン** - シンプル＆洗練  

## コンテンツ管理

### 管理画面へのアクセス
1. サイト下部の「🔐 管理画面にログイン」をクリック
2. GitHub で認証
3. GUIで以下の内容を編集可能：

### 編集可能な内容

- **サイト設定**：サークル名、説明など
- **サークル紹介**：概要説明、設立年
- **メンバー紹介**：最大6人のメンバー情報（名前、役割、自己紹介、SNSリンク、プロフィール画像）
- **新曲情報**：楽曲タイトル、アーティスト、説明、ジャケット画像、各プラットフォームへのリンク
- **SNSリンク**：Twitter、YouTube、pixiv など各種SNS

## ファイル構成

```
.
├── index.html                    # メインサイト
├── admin/
│   ├── index.html               # CMS管理画面
│   └── config.yml               # CMS設定ファイル
├── _data/
│   ├── site-config.json         # サイト基本情報
│   ├── about.json               # サークル紹介
│   ├── members.json             # メンバー情報
│   ├── songs.json               # 楽曲情報
│   └── social-links.json        # SNSリンク
└── README.md
```

## セットアップ手順

### 1. GitHub Pages 有効化
1. リポジトリの Settings → Pages
2. Source を「Deploy from a branch」に設定
3. Branch を「main」に選択
4. 数分待つとサイトが公開されます

### 2. Decap CMS の認証設定

#### 方法1：Netlify Identity（簡単）
1. Netlify にサインアップ（無料）
2. 本リポジトリを接続
3. Team Kakusin. サイトにデプロイ
4. Netlify管理画面で「Identity」を有効化
5. ユーザーを追加

#### 方法2：GitHub OAuth（推奨）
1. GitHub Settings → Developer settings → OAuth Apps
2. 「New OAuth App」を作成
3. Authorization callback URL: `https://[YOUR-DOMAIN]/admin/`
4. Client ID と Client Secret を取得
5. `admin/config.yml` の `backend.repo` と認証情報を更新

詳細は [Decap CMS ドキュメント](https://decapcms.org/) を参照

## 使い方（メンバー向け）

### サイトの編集

1. **サイトへアクセス**  
   メインサイトを表示 → 下部の「🔐 管理画面にログイン」をクリック

2. **認証**  
   GitHub で認証（初回は許可が必要）

3. **編集**  
   左メニューから編集したい項目を選択  
   GUIフォームで内容を入力

4. **保存**  
   「Publish」ボタンをクリック  
   自動で GitHub にコミットされ、数秒でサイトに反映

### メンバー追加

管理画面 → 「メンバー紹介」→ 「メンバー一覧」 → 「Add entry」で追加可能

### 楽曲追加

管理画面 → 「新曲情報」→ 「楽曲一覧」 → 「Add entry」で追加可能

## トラブルシューティング

### 管理画面が真っ白
- キャッシュをクリアして再度アクセス
- ブラウザのコンソール（F12）でエラーを確認

### 編集が反映されない
- GitHub の「Commits」から最新コミットを確認
- Pages のデプロイ状況を確認（Settings → Pages）
- 数分待機後、キャッシュをクリアして再度アクセス

### 画像がアップロードできない
- `images/` フォルダが存在するか確認
- ファイルサイズが大きすぎないか確認（推奨：2MB以下）

## デザインのカスタマイズ

`index.html` の `<style>` セクションを編集することで、色やレイアウトを変更できます。

### 色の変更例
- メイン色：`color: #000000;` を編集
- 背景色：`background-color: #ffffff;` を編集

## ライセンス

MIT License - 自由に使用、改変、配布できます。

---

**制作日**：2026年6月2日  
**提供**：GitHub Copilot
