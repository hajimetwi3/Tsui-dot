# Tsui Dot
Tsui Dot は、写真・イラスト・ローカルカメラ映像を 8bit 風の 2D ドット絵やガラス小窓風の小窓表示へ変換する、ブラウザ内完結の Tsui series ツールです。


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

