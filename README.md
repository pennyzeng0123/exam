# 台中驛鐵道文化園區｜Vibe Coding 指令說明

本文件記錄製作《台中驛鐵道文化園區》影展專題介紹網站時，與 AI 協作所使用的 Vibe Coding 指令（Prompt），以及每一步產生的成果與實務問題除錯過程。

- 專題名稱：流動時光中的軌跡：台中驛鐵道文化園區
- 部署網址：`1105.ct.ws`
- 作者/開發者：曾珮瑜
- 使用工具：Gemini、VS Code、GitHub、InfinityFree (File Manager)
- ## 1. 建立網站

### Prompt 1：依專題需求建立完整網頁架構
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
12. (3) 使用Vercel部署後的網址。
請依照1~12的需求幫我列出製作步驟

**成果**：
| 檔案 | 說明 |
| --- | --- |
| `index.html` | 首頁概覽（Landing page）：主視覺、園區簡介、專題亮點與核心模組、營業與交通資訊 |
| `about.html` | 歷史故事：百年建築的時光凝視、台中驛歷史沿革與活化歷程 |
| `area.html` | 園區介紹：鐵鹿大街、文創聚落、逛街資訊與交通指引 |
| `train.html` | 舊火車介紹：鐵道之魂、典藏舊火車與車廂工藝特色 |

### Prompt 2：素材放進 images 資料夾
成果：`images/` 內包含歷史月台空間活化（101.jpg）、行銷策略與在地連結（123.jpg）、舊火車與車廂展示（456.jpg）等多張主題圖片。


### Prompt 3：CSS 檔案切割與樣式設計
**成果**：
- `css/reset.css`：清除跨瀏覽器預設邊距與樣式。
- `css/layout.css`：定義雙欄版面配置（主內容與側邊欄比例）。
- `css/style.css`：定義深咖啡色主色調、高亮按鈕 (`.menu-btn.active`)、營業與交通資訊卡片 (`.info-card`)、懸浮卡片與 Footer 樣式。

### Prompt 4：導覽列、側邊欄按鈕與資訊卡片整合
**成果**：側邊欄採用 `.sidebar-menu` 與 `.info-card` 佈局，實現當前頁面按鈕高亮（`class="menu-btn active"`）與實用資訊展示。

---

## 2. 實務障礙與 Vibe Coding 深度排查 (Troubleshooting)
### Prompt 8：照課堂教過的寫法修改
成果：參考 HW07 課程結構進行優化：
- HTML 結構採用課堂標準（Header、Nav、Main、Aside、Footer）
- 運用標準 HTML 語意標籤與基本 CSS 選擇器，維持簡潔有條理的程式碼風格
- 移除過於複雜的 JavaScript 動態效果，聚焦於乾淨的 RWD 響應式切版與靜態網頁架構

## 4. 部署與發布
請教我怎麼把網站放到 GitHub、用 Vercel 部署，以及上傳到 InfinityFree 取代首頁。

**成果**：
成果：已完成跨平台部署與發布，成果可至以下連結查看。

---


## 繳交連結

1. Prompt 說明（本檔案）：https://github.com/pennyzeng0123/exam/edit/main/README.md
2. InfinityFree 網址**：https://0224.great-site.net/
3. 3. Vercel 網址：https://exam-ashen-chi.vercel.app/
