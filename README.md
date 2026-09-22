# Neurology_Update

台灣讀者（正體中文 zh-TW）的**個人神經醫學知識庫**＋**每週公開網頁摘要**。聚焦失智症／阿茲海默症、神經科與老人醫學，並收錄當週國內外醫藥與藥政新聞。本站為靜態 HTML，不必建置。

> 這是學習筆記，不是診療、用藥或投資建議。每則條目都附真實來源、日期與 URL／DOI，不杜撰標題。

## 網站怎麼看

GitHub Pages 啟用後，預期網址：

`https://tlan1012.github.io/Neurology_Update/`

本機預覽（在倉庫根目錄）：

```bash
python3 -m http.server 8080 --directory docs
```

然後開啟 <http://127.0.0.1:8080/>。

## 目錄

```
docs/                  ← GitHub Pages 根目錄
  index.html           首頁：簡介 + 週報列表
  weeks/2026-W38.html  單週摘要（ISO 週次）
  kb/                  Markdown 知識庫（一題一檔，可累積）
  kb/index.html        知識庫導覽
  daily/               晨間三向新聞／市場與國際簡報（獨立站樹）
  assets/style.css     版型
```

本倉庫承載兩套互不交叉連結的靜態站樹：神經醫學週報（`docs/index.html`、`weeks/`、`kb/`）與晨間簡報（`docs/daily/`）。

創刊號是 **2026-W38**（2026-09-14 至 2026-09-20，對應 2026-09-19 前後約一至兩週）。

## 每週更新怎麼做

1. 用 ISO 週次開新檔：`docs/weeks/YYYY-Www.html`（可用 `date +%G-W%V`）。
2. 固定四個區塊：
   - 國內醫藥新聞
   - 國外醫藥新聞
   - 期刊選讀（失智症／神經科／老人醫學）
   - 本週可再深讀
3. 每則寫：zh-TW 短摘要、來源＋日期＋連結，以及「背景知識延伸」（機轉／臨床脈絡／為什麼重要／限制）。
4. 在 `docs/kb/` 為重要條目加或更新 Markdown 筆記，並把新週報連到 `docs/index.html`。
5. 頁尾維持：**Grok Bot 研究助理**。

舊週報不要覆蓋，讓首頁列表往上累積。

## 啟用 GitHub Pages

1. 打開倉庫 **Settings → Pages**。
2. **Build and deployment → Source** 選 **Deploy from a branch**。
3. Branch 選 `main`，資料夾選 **`/docs`**。
4. 儲存後等一兩分鐘，到 `https://tlan1012.github.io/Neurology_Update/`。

若 Pages 還沒出來：確認 `main` 已含 `docs/index.html`，且沒有把 Source 設成 GitHub Actions。

## 授權與免責

內容引用各新聞與期刊原文；版權屬原出版社。引用僅供個人學習與公開摘要。
