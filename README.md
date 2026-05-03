# Tsui Dot  

[English](README.en.md)  

Tsui Dot は、写真・イラスト・ローカルカメラ映像を 8bit 風の 2D ドット絵やガラス小窓風の小窓表示へ変換する、ブラウザ内完結の Tsui series ツールです。

- ログイン不要
- 広告なし
- インストール不要（Cloudflare版はPWAとしてインストール可能）
- 外部モジュールなし / CDNなし / JavaScriptのみ
- アプリ本体からの外部送信なし（CSP `connect-src 'none'`）
- `MODE full` による全体ドット絵化
- `MODE window` による、元画像の一部だけをガラス小窓内でドット化する表示
- PNG出力対応

---

## ウェブサイト版（Cloudflare Pages：PWA対応）

以下URLからご利用可能です。  
[https://tsuidot.pages.dev/](https://tsuidot.pages.dev/)  

## ダウンロード版

最新版は GitHub リポジトリの Releases から配布しています。

- **リポジトリ**: [https://github.com/hajimetwi3/Tsui-dot](https://github.com/hajimetwi3/Tsui-dot)
- **最新リリース**: [https://github.com/hajimetwi3/Tsui-dot/releases/latest](https://github.com/hajimetwi3/Tsui-dot/releases/latest)
- 配布物は単一ファイル `tsui-dot.html` です。インストール作業はありません。

ファイル整合性を確認したい場合は、Release ページに記載された `tsui-dot.html` の SHA-256 ハッシュとローカルのハッシュ値を比較してください。  

## クイックスタート

### 単一HTML版

```
1. tsui-dot.html をブラウザで開く
2. 「画像」で写真やイラストを読み込む
3. MODE / DOT / SIZE / GLASS等 を調整
4. 「PNG」で保存
```

### カメラ

`CAM back / front` で背面優先・前面優先を選び、`CAMERA` でローカルカメラを開始します。`FIX` で現在のフレームを固定できます。
カメラ利用にはブラウザの許可が必要です。環境によっては `file://` ではカメラが使えない場合があるため、Cloudflare Pages などの HTTPS 配信か `localhost` での確認を推奨します。


## PRIVACY

画像やカメラ映像は、本アプリ本体から外部送信されません。
`connect-src 'none'` により、`fetch` 等のネットワーク送信はブラウザレベルで禁止されます。

画像データやカメラ映像は `localStorage` や `IndexedDB` に保存しません。
保存されるのは、DOTサイズやパレットなどのUI設定のみです。


## 注意事項

- 本ソフトウェアは現状有姿で提供され、動作の正確性・可用性について保証しません。ご利用は自己責任でお願いします。
- 出力画像の保存・管理は利用者の責任で行ってください。  
- カメラ機能はブラウザと配信元のセキュリティ条件に依存します。  
- 現在、外部からのプルリクエストは受け付けていません（This repository does not accept external pull requests.）

## ライセンス  

[MIT License](LICENSE)  

(c) 2026 Hajime Tsui  

## Third-party  

なし。外部モジュールには依存しません。 

---

## 作者  

[Hajime Tsui](https://hajimetwi3.github.io/hajimetwi3/)  

