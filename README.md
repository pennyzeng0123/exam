# 台中驛鐵道文化園區｜Vibe Coding 指令說明

本文件記錄製作《台中驛鐵道文化園區》影展專題介紹網站時，與 AI 協作所使用的 Vibe Coding 指令（Prompt），以及每一步產生的成果與實務問題除錯過程。

- 專題名稱：流動時光中的軌跡：台中驛鐵道文化園區
- 部署網址：`1105.ct.ws`
- 作者/開發者：曾珮瑜
- 使用工具：Gemini、VS Code、GitHub、InfinityFree (File Manager)
- ## 1. 建立網站

### Prompt 1：整理內容與素材

### Prompt 2：依專題需求建立完整網頁架構
**成果**：| 檔案 | 說明 |
| --- | --- |
| `index.html` | 首頁概覽：主視覺 Banner、專題亮點三大核心模組卡片 |
| `about.html` | 歷史故事：帝冠式建築紅磚美學、鐵路高架化與空間再生沿革 |
| `area.html` | 園區介紹：鐵鹿大街商場、舊軌月台散步區與詳細交通指南 |
| `train.html` | 舊火車介紹：經典蒸汽機關車、懷舊客車車廂典藏展示 |

## 2. 建立網站與架構
### Prompt 3：依專題需求建立完整網頁架構
1. 題目：大二：「您自己的影展專題介紹」
2. 請依照開學至今所有之前所學，建議一個有導覽列、側邊欄，並有分頁的完整網頁。
3. 需要具有完整的SEO內容、Grid System、RWD 功能（可用手持裝置觀看可以顯示完整資訊）等。
4. 需要將CSS檔案進行切割後放置在CSS 檔案匣內。
5. 需要將圖片放置在images 檔案匣內。
6. 請製作一md(markdown)檔案放在Github上，介紹自己用的Vibe Coding指令，並給出連結。
7. 請將此項目取代掉在https://www.infinityfree.com/ 自己網址的首頁。
8. 請用Github及Vercel建立一網頁。
9. 交付三個連結：
10. (1) 此專案所用的Prompt 說明，製作一個md檔案，並使用Github連結網址。
11. (2) 在https://www.infinityfree.com/ 自己的網址（可直接呈現首頁/landing page畫面）
12. (3) 使用Vercel部署後的網址。請依照1~12的需求幫我列出製作步驟

**成果**：
| 檔案 | 說明 |
| --- | --- |
| `index.html` | 首頁概覽：主視覺 Banner、專題亮點三大核心模組卡片 |
| `about.html` | 歷史故事：帝冠式建築紅磚美學、鐵路高架化與空間再生沿革 |
| `area.html` | 園區介紹：鐵鹿大街商場、舊軌月台散步區與詳細交通指南 |
| `train.html` | 舊火車介紹：經典蒸汽機關車、懷舊客車車廂典藏展示 |

### Prompt 4：CSS 檔案切割與樣式設計
**成果**：
- `css/reset.css`：清除跨瀏覽器預設邊距與樣式。
- `css/layout.css`：定義雙欄版面配置（主內容與側邊欄比例）。
- `css/style.css`：定義深咖啡色主色調、高亮按鈕 (`.menu-btn.active`)、營業與交通資訊卡片 (`.info-card`)、懸浮卡片與 Footer 樣式。

### Prompt 5：導覽列、側邊欄按鈕與資訊卡片整合
**成果**：側邊欄採用 `.sidebar-menu` 與 `.info-card` 佈局，實現當前頁面按鈕高亮（`class="menu-btn active"`）與實用資訊展示。

---

## 3. 實務障礙與 Vibe Coding 深度排查 (Troubleshooting)

在專案部署與測試過程中，遇到數個實務排版與上傳問題，透過對話式指令進行精準排查：

### Prompt 6：排查 HTML 結構錯亂問題
## 4. 部署與發布

### Prompt 10：部署至 InfinityFree 伺服器
請告訴我如何正確將檔案部署至 InfinityFree，並解決 index.php 優先權衝突的問題。

**成果**：
1. 登入 InfinityFree 控制台，進入 File Manager 的 `1105.ct.ws/htdocs/` 資料夾。
2. 檢查並刪除預設的 `index.php` 檔案，避免伺服器優先讀取 PHP 而覆蓋 `index.html`。
3. 完整上傳 `index.html`、`about.html`、`area.html`、`train.html` 以及 `css/`、`images/` 資料夾。

---

## 繳交連結

1. **Prompt 說明檔案 (PROMPTS.md)**：*(請貼上你的 GitHub PROMPTS.md 檔案網址)*
2. **InfinityFree 專題網站網址**：`http://1105.ct.ws`
3. **GitHub 專案儲存庫**：*(請貼上你的 GitHub Repository 網址)*
