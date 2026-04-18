# 台股技術面篩選 PWA

## 部署到 GitHub Pages（免費）

### 步驟一：建立 GitHub 帳號
前往 [github.com](https://github.com) 註冊（若已有帳號跳過）

### 步驟二：建立新 Repository
1. 點右上角 `+` → `New repository`
2. Repository name 填：`taiwan-stock-screener`
3. 設定為 **Public**
4. 按 `Create repository`

### 步驟三：上傳檔案
1. 在新建的 repo 頁面，點 `uploading an existing file`
2. 把以下檔案全部拖曳上傳：
   - `index.html`
   - `manifest.json`
   - `sw.js`
   - `icons/` 資料夾（含 icon-192.png 和 icon-512.png）
3. 點 `Commit changes`

### 步驟四：開啟 GitHub Pages
1. 進入 repo 的 `Settings`
2. 左側選 `Pages`
3. Source 選 `Deploy from a branch`
4. Branch 選 `main`，folder 選 `/ (root)`
5. 按 `Save`

等約 1 分鐘後，網址會是：
```
https://[你的帳號].github.io/taiwan-stock-screener/
```

### 步驟五：在 iPhone 加入主畫面
1. 用 Safari 開啟上面的網址
2. 點下方分享按鈕 `⬆`
3. 選「加入主畫面」
4. 完成！桌面會出現 app icon

---

## 使用說明

- **查詢日期**：選擇你要查的交易日
- **市場**：上市或上櫃
- **FinMind Token**：免費申請可提高流量上限，前往 https://finmindtrade.com/
- **篩選條件**：可自由組合，例如：
  - 收盤/MA5 > 0（收盤在五日線以上）
  - 漲跌幅 > 3（當日上漲超過3%）
  - 成交量 > 1000（成交量超過1000張）

## 注意事項
- 全市場掃描約需 3~10 分鐘（FinMind 免費 API 限制）
- 資料僅供參考，不構成投資建議
