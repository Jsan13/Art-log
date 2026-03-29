# ART LOG — 鑑賞記録

美術展・アートイベントの鑑賞記録PWAアプリ。

---

## 📁 ファイル構成

```
artlog-pwa/
├── index.html      ← アプリ本体
├── manifest.json   ← PWA設定
├── sw.js           ← Service Worker（オフライン対応）
├── icon.svg        ← アイコン原稿
├── icon-192.png    ← アイコン（要変換）
├── icon-512.png    ← アイコン（要変換）
└── README.md
```

---

## 🚀 GitHub Pagesで公開する手順

### 1. アイコンを準備する

`icon.svg` をPNGに変換して `icon-192.png`（192×192）と `icon-512.png`（512×512）を用意してください。

変換方法：
- オンラインツール: https://svgtopng.com
- またはmacOSのプレビューアプリで書き出し

### 2. GitHubにリポジトリを作成

1. https://github.com にアクセスしてログイン（アカウントがなければ無料で作成）
2. 右上の「＋」→「New repository」
3. Repository name: `artlog`（なんでもOK）
4. **Public** を選択
5. 「Create repository」をクリック

### 3. ファイルをアップロード

1. 作成したリポジトリページで「uploading an existing file」をクリック
2. このフォルダ内のファイルをすべてドラッグ＆ドロップ
3. 「Commit changes」をクリック

### 4. GitHub Pagesを有効化

1. リポジトリの「Settings」タブを開く
2. 左メニューの「Pages」をクリック
3. Source: 「Deploy from a branch」
4. Branch: `main` / `/(root)` を選択
5. 「Save」をクリック

数分後、`https://あなたのユーザー名.github.io/artlog/` でアクセスできるようになります。

---

## 📱 スマホのホーム画面に追加

### iPhoneの場合（Safari）
1. Safariでアプリのページを開く
2. 画面下の共有ボタン（□↑）をタップ
3. 「ホーム画面に追加」をタップ
4. 「追加」をタップ

### Androidの場合（Chrome）
1. Chromeでアプリのページを開く
2. 画面上部に「ホーム画面に追加」の通知が出たらタップ
3. または右上の「⋮」→「アプリをインストール」

---

## 💾 データのバックアップ

データはブラウザのlocalStorageに保存されます。
定期的に「DATA → ⬇ エクスポート」でJSONファイルをバックアップしてください。

機種変更時は：
1. 旧端末でエクスポート
2. 新端末でアプリを開き「⬆ インポート」
