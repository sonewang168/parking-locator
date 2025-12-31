# 🚗 停車小幫手

一款功能完整的停車位置記錄器 PWA，幫助您輕鬆記住停車位置！

## ✨ 功能特色

### 📍 GPS 定位
- 高精度 GPS 定位記錄停車位置
- 自動反向地理編碼取得地址
- 顯示 GPS 座標與精確度

### 📸 拍照記錄
- 支援拍攝多達 6 張照片
- 自動壓縮優化儲存空間
- 點擊照片可放大檢視

### ⏰ 計時提醒
- 即時顯示已停車時間
- 可設定 30分鐘 / 1小時 / 2小時 / 3小時 / 4小時 提醒
- 系統通知 + 震動提醒

### 🗺️ 互動地圖
- 使用 Leaflet + OpenStreetMap 顯示位置
- 一鍵開啟 Google Maps 導航
- 支援分享位置給他人

### 📝 詳細記錄
- 樓層標記（如 B2）
- 區域標記（如 A區）
- 自訂備註（如 紅色柱子旁）

### 📜 歷史記錄
- 自動保存最近 50 筆停車記錄
- 顯示停車時間與總時長
- 點擊可導航至歷史位置

### 📱 PWA 支援
- 可安裝至手機主畫面
- 離線可用（已快取資料）
- 原生 App 體驗

## 🚀 快速開始

### 方法一：GitHub Pages 部署（推薦）

1. **建立 GitHub Repository**
   - 到 GitHub 建立新的 repository
   - 名稱建議：`parking-locator`

2. **上傳檔案**
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/你的帳號/parking-locator.git
   git push -u origin main
   ```

3. **啟用 GitHub Pages**
   - 進入 Repository → Settings → Pages
   - Source 選擇 **GitHub Actions**
   - 等待自動部署完成（約 1-2 分鐘）

4. **完成！** 
   - 網址：`https://你的帳號.github.io/parking-locator/`

### 方法二：Netlify 部署

1. 下載 ZIP 解壓縮
2. 拖曳資料夾到 [Netlify Drop](https://app.netlify.com/drop)

### 本地測試
```bash
# 使用任何靜態伺服器
npx serve .
# 或
python -m http.server 8000
```

## 📁 檔案結構

```
parking-locator/
├── index.html      # 主應用程式
├── manifest.json   # PWA 配置
├── sw.js           # Service Worker
├── icon.svg        # SVG 圖示
├── icon-192.png    # 192x192 圖示
├── icon-512.png    # 512x512 圖示
├── netlify.toml    # Netlify 配置
└── README.md       # 說明文件
```

## 🔧 技術架構

- **前端框架**: 原生 JavaScript (Vanilla JS)
- **地圖服務**: Leaflet + OpenStreetMap
- **地理編碼**: Nominatim API
- **資料儲存**: localStorage
- **圖片處理**: Canvas API 壓縮
- **通知服務**: Web Notifications API
- **PWA**: Service Worker + Web App Manifest

## 📱 瀏覽器支援

- Chrome / Edge 最新版
- Safari 最新版
- Firefox 最新版
- 行動版瀏覽器

## 🔐 隱私說明

- 所有資料儲存於本地裝置
- GPS 定位需要使用者授權
- 不會上傳任何個人資料
- 照片僅儲存於本地

## 📄 授權

MIT License

---

開發者：Sone Wang
