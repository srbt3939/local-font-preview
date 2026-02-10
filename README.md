# Font Preview Tool

システムにインストールされているすべてのフォントを一覧表示し、任意の文字列でプレビューできるWebツールです。

![Font Preview Tool](https://img.shields.io/badge/license-MIT-blue.svg)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)

## 🎯 特徴

- **自動フォント検出**: Local Font Access APIを使用してシステムフォントを自動取得
- **一覧表示**: すべてのフォントで同じテキストを同時に比較
- **リアルタイムプレビュー**: フォントサイズ・行間を即座に調整可能
- **フォント検索**: フォント名での絞り込み検索
- **カスタムフォント対応**: TTF/OTF/WOFF/WOFF2ファイルのアップロード
- **レスポンシブデザイン**: モバイル・タブレット・デスクトップに対応

## 🚀 デモ

[GitHub Pagesでデモを見る](https://srbt3939.github.io/local-font-preview/) 

## 📋 必要環境

### 対応ブラウザ

インストール済みフォント機能を使用するには以下のブラウザが必要です：

- Google Chrome 103+
- Microsoft Edge 103+
- Opera 89+

※ Local Font Access APIに対応していないブラウザでも、フォントファイルアップロード機能は利用可能です。

### ブラウザ対応状況

| ブラウザ | フォント自動検出 | ファイルアップロード |
|---------|----------------|-------------------|
| Chrome 103+ | ✅ | ✅ |
| Edge 103+ | ✅ | ✅ |
| Firefox | ❌ | ✅ |
| Safari | ❌ | ✅ |

## 🔧 使い方

### オンラインで使用

1. [GitHub Pages](#)にアクセス（デプロイ後）
2. フォントアクセスの許可を承認
3. テキストを入力してフォントをプレビュー

### ローカルで使用

1. リポジトリをクローン
```bash
git clone https://github.com/yourusername/font-preview-tool.git
cd font-preview-tool
```

2. HTMLファイルをブラウザで開く
```bash
# Chromeで開く例
open font-preview-list.html  # macOS
start font-preview-list.html  # Windows
xdg-open font-preview-list.html  # Linux
```

または、ローカルサーバーを起動（推奨）：
```bash
# Pythonを使用する場合
python -m http.server 8000

# Node.jsを使用する場合
npx http-server
```

ブラウザで `http://localhost:8000/font-preview-list.html` にアクセス

## 📖 機能詳細

### インストール済みフォント一覧

- システムにインストールされているすべてのフォントを自動検出
- フォント名でのリアルタイム検索
- 任意の文字列で一括プレビュー
- フォントサイズ: 12px～72px
- 行間: 0.8～3.0

### フォントファイルアップロード

- 対応形式: TTF, OTF, WOFF, WOFF2
- ドラッグ&ドロップ対応
- フォントサイズ: 12px～120px
- 行間: 0.8～3.0

## 🔒 プライバシーとセキュリティ

- すべての処理はブラウザ内で完結（サーバーへのデータ送信なし）
- フォント情報はローカルで処理され、外部に送信されません
- Local Font Access APIは初回アクセス時にユーザーの許可が必要です

## 🛠️ 技術スタック

- HTML5
- CSS3 (Flexbox, Grid)
- Vanilla JavaScript (ES6+)
- [Local Font Access API](https://developer.mozilla.org/en-US/docs/Web/API/Local_Font_Access_API)

## 📁 ファイル構成

```
font-preview-tool/
├── font-preview-list.html   # メインアプリケーション
├── README.md                # このファイル
└── LICENSE                  # ライセンスファイル
```

## 🤝 貢献

プルリクエストを歓迎します！大きな変更の場合は、まずissueを開いて変更内容を議論してください。

1. このリポジトリをフォーク
2. フィーチャーブランチを作成 (`git checkout -b feature/amazing-feature`)
3. 変更をコミット (`git commit -m 'Add some amazing feature'`)
4. ブランチにプッシュ (`git push origin feature/amazing-feature`)
5. プルリクエストを作成

## 📝 ライセンス

このプロジェクトは[MIT License](LICENSE)の下でライセンスされています。

## 🐛 既知の問題

- Local Font Access APIはChrome/Edge以外のブラウザでは動作しません
- 一部のシステムフォントは表示されない場合があります
- フォント数が多い環境では初期読み込みに時間がかかる場合があります

## 📧 お問い合わせ

質問や提案がある場合は、[Issues](https://github.com/yourusername/font-preview-tool/issues)を開いてください。

## 🙏 謝辞

- [Local Font Access API](https://wicg.github.io/local-font-access/)の仕様策定者の皆様
- このツールの改善に貢献してくださったすべての方々

---

⭐ このプロジェクトが役に立った場合は、スターをつけていただけると嬉しいです！
