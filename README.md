# Web Accessibility Pro - 網路無障礙助手 Chrome 擴充功能

> 最佳的無障礙瀏覽網際網路輔助工具，專為提供包容、無障礙的網路體驗而設計。遵循 WCAG 2.2 與 EN 301 549 國際標準。

---

## 🌟 核心功能特色

### 1. 一鍵情境模式預設集 (Profiles)
- **🛡️ 癲癇安全模式 (Epilepsy Safe)**：暫停所有 CSS 動畫、影片及過渡效果，採用低飽和護眼色彩，杜絕高頻閃爍引發的風險。
- **📖 閱讀障礙友善模式 (Dyslexia Friendly)**：自動替換為閱讀障礙友善專用字型，放大字距與行距，並開啟跟隨滑鼠的導讀輔助尺。
- **🎯 專注 / ADHD 模式 (ADHD & Cognitive)**：啟用聚焦閱讀遮罩（Focus Mask），遮蔽上下干擾區，弱化干擾圖片。
- **👁️ 視力障礙高對比模式 (Visually Impaired)**：150% 大字體、WCAG AAA 黑底黃字高對比、超大白色游標及醒目超連結框。
- **🎨 色盲輔助模式 (Color Blindness)**：色彩校正矩陣，支援紅色盲（Protanopia）、綠色盲（Deuteranopia）、藍色盲（Tritanopia）與全色盲。

### 2. 精細文字與排版調整
- **字體大小縮放**：100% ~ 200% 多段縮放。
- **行高與字距**：提供 1.5x、1.8x、2.0x 行距與寬鬆/特寬字距。
- **文字對齊方式**：支援靠左、置中、靠右與兩端對齊。
- **閱讀障礙字體切換**。

### 3. 色彩與視覺對比
- 6 種對比主題：標準原貌、深色模式、黑底黃字 (AAA)、色彩反轉、單色灰階、柔和護眼。
- 內建色盲 SVG 濾鏡矩陣，無損覆蓋所有網頁。

### 4. 認知與動態抑制
- **暫停所有動畫**：即時強制停止 CSS Animation, Transitions 與網頁影片播放。
- **隱藏/弱化圖片**：淡化圖片與視覺元素，滑鼠懸停時才復原，降低資訊過載。
- **一鍵靜音媒體**：杜絕自動播放音訊干擾。

### 5. 導航與輔助工具
- **導讀輔助尺 (Reading Guide)**：隨游標水平延伸的黃色導讀尺（快捷鍵 `Alt + A`）。
- **聚焦閱讀遮罩 (Focus Mask)**：隨游標移動的聚光橫條，遮蔽非焦點文字。
- **超連結加強標註**：為所有連結加上螢光黃底色與高對比虛線框。
- **標題結構標籤**：視覺化標註 H1 ~ H6 標籤階層。
- **ARIA & 圖片 Alt 檢視器**：滑鼠懸停時即時提示元素標籤、alt 屬性與 aria-label。
- **巨型滑鼠游標**：支援 48px 黑色與白色巨型光標。

### 6. 語音朗讀輔助 (Text-to-Speech)
- **點擊段落朗讀**：開啟後直接點擊任何段落或標題進行語音播放，伴隨螢光綠高亮指示。
- **選取文字朗讀**：反白文字後按下 `Alt + S` 或右鍵選單立即朗讀。
- **語速調整**：0.75x ~ 1.75x 自由調節。

### 7. 隱私與安全性 (Privacy by Design)
- 100% 本地運算，不依賴任何外部雲端伺服器，不收集或儲存任何個人隱私數據（PII）。
- 嚴格遵守 GDPR、COPPA 及 ISO 27001 精神。

---

## 🚀 如何安裝與使用 (開發人員模式)

1. 打開 Google Chrome 瀏覽器，在網址列輸入：
   ```
   chrome://extensions/
   ```
2. 在右上角開啟 **「開發人員模式」**（Developer mode）開關。
3. 點擊左上角的 **「載入未封裝項目」**（Load unpacked）按鈕。
4. 選擇本專案資料夾：
   ```
   C:\Users\a0953\.gemini\antigravity\scratch\web-accessibility-pro
   ```
5. 載入完成後，在 Chrome 工具列右上角點擊擴充功能圖示（拼圖形狀），並將 **Web Accessibility Pro** 釘選至工具列。
6. 開啟任意網頁或打開本專案中的示範頁面：
   ```
   file:///C:/Users/a0953/.gemini/antigravity/scratch/web-accessibility-pro/test/test-page.html
   ```
   即可點擊擴充功能圖示開啟控制面板體驗所有功能！

---

## ⌨️ 快捷鍵清單

- **Alt + A**：快速開啟 / 關閉導讀輔助尺
- **Alt + S**：朗讀當前選取反白的文字
- **滑鼠右鍵**：選取文字後右鍵選擇「🔊 朗讀所選取的文字」

---

## 📁 專案檔案結構

```
web-accessibility-pro/
├── manifest.json              # Manifest V3 設定檔
├── icons/                     # 擴充功能圖示 (16x16, 48x48, 128x128)
├── popup/                     # 控制面板介面
│   ├── popup.html
│   ├── popup.css
│   └── popup.js
├── content/                   # 注入目標網頁的腳本與樣式
│   ├── content.js
│   └── content.css
├── background/                # 背景服務
│   └── service-worker.js
├── test/                      # 測試示範網頁
│   └── test-page.html
└── README.md                  # 說明文件
```
