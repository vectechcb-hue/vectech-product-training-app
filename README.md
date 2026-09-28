# VECTECH 產品教育訓練教材產生器

手機優先的 PWA 教材製作工具。

> GitHub Pages 已啟用自動部署。

## 功能
- 教材標題與自訂檔名
- 步驟新增、刪除、排序
- 單張／批次圖片匯入與自動壓縮
- 每步驟文字說明
- A4 直式 PDF 匯出
- 16:9 PowerPoint 匯出
- Firebase Anonymous Auth + Firestore 雲端紀錄
- PWA 安裝到 iPhone / Android 主畫面

## GitHub Pages
Repository Settings → Pages → Build and deployment → Source 選 GitHub Actions 或 Deploy from a branch。
若使用 branch，選 main / root。

部署後網址：
https://vectechcb-hue.github.io/vectech-product-training-app/

## Firebase
本版本預留 Firebase 設定入口：
在 index.html 的 script module 載入前設定 window.VECTECH_FIREBASE_CONFIG。
正式部署時建議使用自己的 Firebase Web App 設定，並啟用 Anonymous Authentication 與 Firestore。

## 手機安裝
iPhone：Safari 開啟網站 → 分享 → 加入主畫面。
Android：Chrome 開啟網站 → 選單 → 加入主畫面／安裝 App。

## 注意
PDF 與 PPT 使用瀏覽器端產生，圖片會先壓縮以降低手機記憶體與 Firestore 使用量。
