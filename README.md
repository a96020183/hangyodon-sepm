# Hangyodon SEPM Study Flight

畀 Blue 嘅 Hangyodon 陪讀小遊戲：按 SEPM 原本第 0–11 主章節選 topic，做英文 MCQ、儲 XP、重溫錯題同收集徽章。手機同電腦瀏覽器都可以用。

直接使用：[Hangyodon 陪你飛](https://a96020183.github.io/hangyodon-sepm/)。

目前 **6,837 題**，由原有 96 題擴充。已盤點 667 頁手冊、798 個編號目錄項目；**600/600 個最細目錄小節**及 **547/547 頁學習內容**均至少有一道附來源的題目，包括附錄 A、B、C。其餘頁面為 95 頁明示留白、23 頁目錄／修訂紀錄和 2 頁出版控制。

今次新增 **257 題程序練習**，考條件／行動配對、操作原因、未考過的參數及 crew rest 火警分支；首頁可按「只練新增題」集中練習。

覆蓋代表每個小節及內容頁均有題目，並不代表每一個事實、圖示標籤或 SOP 步驟均已被考核。完整程序、條件及例外仍須閱讀原手冊。首頁「全書覆蓋清單」列出各小節題數，亦可搜尋及練習指定小節。

## 每章題數

- 0 Administration & Control of Operations Manual: **204 questions**
- 1 Introduction: **179 questions**
- 2 Human Factors and Emergencies: **112 questions**
- 3 Communication: **77 questions**
- 4 Safety and Emergency Equipment: **1211 questions**
- 5 Normal Procedures / Supplementary Procedures: **510 questions**
- 6 Non Normal Procedures: **676 questions**
- 7 Post Evacuation and Survival: **253 questions**
- 8 Dangerous Goods: **193 questions**
- 9 First Aid/Illnesses/Injuries: **1024 questions**
- 10 Aircraft Specific: **1966 questions**
- 11 Security: **432 questions**

附錄 A briefing 題按內容分入相關主章節；附錄 B 設備數量表歸第 4 章；附錄 C 培訓要求歸第 1 章。引用仍保留 A／B／C 編號。

## 題目及來源

題幹、選項和原文引用使用 PDF 英文；介面及預設收起的輔助提示使用廣東話。題型包括情境／知識題、原文填詞、原生 briefing 完整答案、設備數量及培訓矩陣。

每題正確選項均有原文依據。文字題核對完整原句；表格題按原頁 cell 座標及勾選欄位核對；掃描表格／圖示題人工對照原圖，並保留來源裁圖。答題後顯示来源類型、英文證據、章節及 PDF 頁碼。來源版本為 FOP_SEPM_20260824.pdf，24 Aug 2026，Rev. 11。[覆蓋報告](site/coverage-report.json)可查看逐節及逐頁盤點。

按 **Open your local manual** 可選取自己裝置上的 PDF，网站核對 SHA-256 與題庫來源一致後開啟引用頁面，檔案不會上傳。重新整理後需重新選取；部分手機可能忽略指定頁碼，可手動輸入畫面列出的 PDF 頁碼。

完整 PDF 留在本機，網站包含題目、引用摘錄及部分原頁裁圖。

## 溫習紀錄與部署

XP、錯題及徽章存於目前瀏覽器 localStorage；不同裝置各自保存。每題每日首次答對獲得 10 XP，以香港日期計算；錯題連續答對兩次才移出收藏。原有 96 題 ID 與手冊指紋保持不變，既有進度保留。

GitHub Actions 在推送 main 後部署 site/。網站無 API key 或後端；Hangyodon 圖嵌入 HTML，來源裁圖在 assets/references/ 按需載入。修改靜態網站後推送即可部署。

Hangyodon 角色屬 Sanrio；本網站為個人非官方溫習作品。XP 及徽章是練習紀錄，不是操作資格或官方考核結果。
