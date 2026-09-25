# Red Lantern Design

正式網站：https://0-exas.github.io/ex/

## 更新與發布

GitHub Pages 使用 `main` 分支的根目錄。將變更推送至 `main` 後，GitHub 會自動發布；到 Actions 查看 `pages-build-deployment` 是否成功。

- `index.html`：唯一維護的首頁。
- `css/style.css`：主要樣式。
- `images/`：網站圖片。
- `.nojekyll`：直接發布靜態檔案。

`html/index.html`、`ex-main/index.html` 和 `ex-main/html/index.html` 為舊網址入口，會轉到正式首頁。`ex-main/css/style.css` 引用主要樣式，避免維護兩套樣式；舊圖片保留以相容既有網址。

首頁資源使用相對路徑，確保部署在 `/ex/` 下仍可載入。Services、Portfolio、Contact 目前連到現有首頁區塊；尚無獨立子頁、聯絡表單或聯絡信箱。
