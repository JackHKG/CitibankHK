# Citibank HK PWA Demo

**這是一個基於你提供的螢幕錄影製作的 Citibank Hong Kong 流動銀行 Progressive Web App (PWA) 示範版本。**

> ⚠️ **重要聲明**：這**不是**花旗銀行的官方應用程式。這純粹是個人學習及展示用途的模擬項目，與 Citigroup / Citibank 無任何關聯、未經授權或背書。所有數據均為虛構示範數據。

---

## ✨ 功能特色（已實現）

- **完整 PWA**：可安裝到手機主畫面，像原生 App 一樣使用（支援離線基本快取）
- **多畫面導航**：首頁、帳戶、轉數快轉賬、交易記錄、服務
- **高度還原影片畫面**：
  - 深藍色 Citi 啟動畫面 + 划艇插圖
  - 首頁優惠卡片（Quick Cash、Wealth Insights 等）
  - 帳戶概覽 + 點擊進入詳細頁（利率 Booster）
  - 完整交易記錄列表（包含你影片中的大額交易）
  - 可搜尋交易記錄
  - 轉賬表單（模擬轉出後自動加入交易記錄）
- **互動元素**：按鈕、Toast 提示、Modal 彈窗、即時搜尋
- **iOS 風格**：狀態列、圓角、陰影、按下動畫
- **手機優先設計**：在 420px 寬容器內模擬 iPhone 體驗

---

## 📱 如何在 GitHub 部署（超簡單步驟）

因為你表示對程式設計認識有限，我已準備好所有檔案。你只需：

### 方法一：使用 GitHub 網頁介面（推薦新手）

1. 登入 [GitHub.com](https://github.com)（沒有帳號就註冊一個）
2. 點擊右上角 **「+」** → **「New repository」**
3. Repository name 輸入：`citibank-hk-pwa` （或其他你喜歡的名稱）
4. 保持 **Public**，不要勾選 Initialize with README
5. 點擊綠色 **「Create repository」**
6. 進入新 repo 後，點擊 **「uploading an existing file」** 或直接拖放資料夾
7. 把整個 `citibank-hk-pwa` 資料夾內的 **所有檔案**（index.html、manifest.json、service-worker.js、icon-*.png、README.md）**全部上傳**
8. 上傳完成後，點擊右上角 **「Settings」** 分頁
9. 左側選單找到 **「Pages」**
10. 在 "Build and deployment" 區塊：
    - Source 選擇 **「Deploy from a branch」**
    - Branch 選擇 **「main」**（或 master）
    - Folder 保持 **「/ (root)」**
11. 點擊 **Save**
12. 等 1-2 分鐘，頁面最下方會出現你的網址，例如：
    `https://你的用戶名.github.io/citibank-hk-pwa`

**完成！** 手機用 Chrome 或 Safari 開啟該網址，即可看到 App。

### 安裝為 PWA（加到主畫面）

- **iPhone**：Safari 開啟網址 → 分享按鈕 → 「加入主畫面」
- **Android**：Chrome 開啟網址 → 右上角 ⋮ → 「安裝 App」或「加入主畫面」

安裝後會有 Citi 圖示，像原生 App 一樣開啟，無瀏覽器地址列。

---

## 🛠️ 本地測試（選用）

如果你想在電腦上先看看效果：

```bash
# 方法 1: Python (大多數電腦都有)
cd citibank-hk-pwa
python3 -m http.server 8000

# 方法 2: Node.js (如果有安裝)
npx serve
```

然後用瀏覽器開啟 `http://localhost:8000`

---

## ✏️ 如何編輯 / 自訂（給你後續指示用）

這個專案**非常容易修改**，因為主要只有一個 `index.html` 檔案。

### 常見修改建議（你可以之後告訴我）：

- 改用戶名稱（目前是 "Kwun Long Lam"）
- 改餘額數字
- 加入更多交易記錄
- 改顏色主題
- 加入真實圖片（把 kayak 換成你喜歡的）
- 增加新功能按鈕
- 改交易記錄的日期或金額

**你之後可以這樣告訴我：**
> 「請把首頁的 Quick Cash 回贈金額改成 HK$10,000，並把交易記錄裡最大的那筆改成 HKD 120,000」

我會直接給你修改後的完整程式碼，或教你怎麼自己改。

---

## 📂 專案檔案說明

| 檔案 | 作用 |
|------|------|
| `index.html` | 整個 App 的核心（所有畫面、互動都在這裡） |
| `manifest.json` | PWA 安裝設定（名稱、圖示、顏色） |
| `service-worker.js` | 讓 App 可以離線運作的基本快取 |
| `icon-192.png` / `icon-512.png` | App 安裝圖示 |
| `README.md` | 你現在看的說明文件 |

---

## ✅ 下一步

1. 按照上面步驟把檔案上傳到 GitHub
2. 測試網頁版是否正常運作
3. 在手機上安裝為 PWA
4. **告訴我** 你想先修改什麼地方（例如：換名字、改金額、加新畫面、調整版面等）

我會繼續幫你迭代，直到你滿意為止！

---

**Enjoy your Citibank HK PWA Demo!** 🚀

如有任何問題，隨時問我。