# Hangyodon SEPM Study Flight

畀 Blue 嘅 Hangyodon 陪讀小遊戲：按 SEPM 原本 0–11 主章節選 topic，做英文 MCQ、儲 XP、重溫錯題同收集徽章。手機同電腦瀏覽器都可以用。

Repository：[a96020183/hangyodon-sepm](https://github.com/a96020183/hangyodon-sepm)。網站部署後可於 [GitHub Pages](https://a96020183.github.io/hangyodon-sepm/) 使用。

目前有 96 題入門題，未覆蓋手冊全部小節。題幹為根據手冊編寫；每題正確選項逐字取自引用頁面（空白已正規化），答題後顯示英文原文摘錄、章節、手冊頁碼及 PDF 頁碼。廣東話輔助提示按需要展開。來源版本為 FOP_SEPM_20260824.pdf，24 Aug 2026。

## 發佈到 GitHub Pages

1. 將本目錄放入你選定的 GitHub repository，使用 `main` 分支。
2. 在 repository 的 **Settings → Pages → Build and deployment → Source** 選 **GitHub Actions**。
3. 推送 `main`，或在 **Actions → Publish study website → Run workflow** 執行部署。
4. 部署成功後，在 **Settings → Pages** 或該次 deployment 取得實際網址，再發給朋友。

部署 workflow 只發佈 `site/`。不需要 npm 安裝、API key 或後端。

首次推送可以在本目錄使用 PowerShell：

```powershell
git init -b main
git add .gitignore README.md .github site
git commit -m "Add Hangyodon SEPM study website"
git remote add origin https://github.com/a96020183/hangyodon-sepm.git
git push -u origin main
```

部署狀態及實際網址請查看 repository 的 Actions 與 Settings → Pages。

GitHub 官方部署說明：[GitHub Pages custom workflows](https://docs.github.com/en/pages/getting-started-with-github-pages/using-custom-workflows-with-github-pages)。

## 原文 PDF 對照

題目及英文引用摘錄已包含在網站。按 **Open your local manual** 可選取自己裝置上的 PDF，網站核對 SHA-256 與題庫來源一致後，開啟所引用頁面；選取的檔案不會上傳。換頁或完成題目後仍可使用已選取的手冊；重新整理網站後需重新選取。部分手機瀏覽器會下載 PDF 或忽略指定頁碼，可依畫面列出的 PDF 頁碼跳轉。

完整 PDF 留在本機，部署包不包含原本 667 頁手冊。題目及所引用摘錄會隨網站發佈。

## 溫習紀錄

XP、錯題及徽章存於目前瀏覽器的 localStorage。不同手機、電腦或瀏覽器各自保存紀錄；清除瀏覽器資料會清除紀錄。每題每日首次答對獲得 10 XP，日期按香港時間計算；錯題需連續答對兩次才移出收藏。

## 更新網站

本 repository 包含可直接發佈的靜態網站，圖片及題庫均嵌入 `site/index.html`。本機製作目錄中的 `build_app.py` 與 `build_web.py` 負責依指定版本手冊重新生成。更新題庫後重新生成，推送新的 `site/index.html` 即可重新部署。

Hangyodon 角色屬 Sanrio；本網站為個人非官方溫習作品。XP、徽章及遊戲進度只表示練習紀錄，不是操作資格或官方考核結果。
