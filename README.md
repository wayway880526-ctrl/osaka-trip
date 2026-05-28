# 大阪五日自由行 | 11月經典行程

2026 年 11 月大阪自由行完整靜態網站，適合直接部署到 GitHub Pages、Netlify、Vercel 等平台。

## 專案結構（標準靜態網站格式）

```
osaka-itinerary/
├── index.html          ← 網站主入口（repo root，可直接部署）
├── .nojekyll           ← GitHub Pages 專用（避免 Jekyll 處理）
├── images/             ← 所有客製化圖片（11 張，相對路徑）
│   ├── 1.jpg
│   ├── 2.jpg
│   ├── 3.jpg
│   ├── ...
│   └── 11.jpg
└── README.md
```

- `index.html` 放在最外層，符合標準靜態網站部署規範。
- 所有圖片路徑皆為相對路徑（`images/xxx.jpg`），可直接上傳使用。
- 無需任何建置步驟（no build step）。

## 快速開始（本地預覽）

1. 下載整個資料夾
2. 直接用瀏覽器打開 `index.html`
3. 或使用 Live Server（VS Code 推薦）：
   - 安裝 Live Server 擴充功能
   - 右鍵 `index.html` → 「Open with Live Server」

## 部署方式（推薦）

### 1. Netlify（最簡單，推薦新手）

1. 前往 [netlify.com](https://netlify.com) 登入
2. 點擊「Add new site」→ 「Deploy manually」
3. 將整個 `osaka-itinerary` 資料夾直接拖曳上去
4. 部署完成，立即獲得網址

### 2. GitHub Pages（完全符合你的要求）

本專案已整理為 **GitHub Pages 最佳格式**：

- `index.html` 位於最外層（repo root）
- 所有圖片放在 `images/` 資料夾
- 所有路徑皆為**相對路徑**（`images/xxx.jpg`）
- 已加入 `.nojekyll` 檔案（避免 Jekyll 處理問題）

#### 部署步驟：

1. 在 GitHub 建立新 Repository（建議命名為 `osaka-itinerary`）
2. 將整個 `osaka-itinerary` 資料夾的內容**上傳到 Repository 的根目錄**（或使用 git push）
   - 確保 `index.html` 直接在 repo 最外層
3. 進入 Repository → **Settings** → **Pages**
4. 在 "Build and deployment" 區塊：
   - Source 選擇 **Deploy from a branch**
   - Branch 選擇 `main`（或 master）
   - Folder 選擇 `/ (root)`
5. 點擊 Save
6. 等待 30 秒 ~ 2 分鐘，頁面會顯示綠色 "Your site is live at" 網址
7. 網址格式：`https://你的帳號.github.io/osaka-itinerary`

**小提醒**：
- 如果你把檔案放在 `/docs` 資料夾，請改選 Folder 為 `/docs`，但本專案推薦放在 root（最乾淨）。
- 第一次部署可能需要 1-2 分鐘才會生效。

### 3. Vercel

1. 前往 [vercel.com](https://vercel.com) 登入
2. Import Git Repository 或直接拖曳資料夾上傳
3. 自動偵測為靜態網站，立即部署

## 網站特色

- 完整五天大阪自由行（以西成區新今宮酒店為基地）
- **石切神社** 安排在 Day 3 上午／下午
- **道頓堀** 安排在多個晚上（符合夜間最佳氛圍）
- 其他夜間亮點：
  - 法善寺橫丁（燈籠石板路）
  - 梅田スカイビル空中庭園夜景
  - 大阪城イルミナージュ（2026 年 11 月營業時間）
- 11 張 AI 客製化高品質圖片
- 響應式設計（手機、平板、電腦皆適用）
- 實用資訊包含最新交通、門票、預算參考

## 技術說明

- 使用 Tailwind CSS（透過 CDN）
- Font Awesome 圖示
- 單一 HTML 檔案 + 圖片資源
- 完全離線可開啟（除了 CDN 資源）

## 注意事項

- 圖片皆為 AI 生成示意圖，實際造訪請以現場為準
- 門票與營業時間以 2026 年 11 月最新資訊為主，建議出發前再確認官網
- 如需修改行程、日期、加入更多景點，請直接編輯 `index.html`

---

**準備好出發大阪了嗎？**  
直接部署後分享給家人朋友即可使用！ 

如有任何修改需求，歡迎隨時提出。