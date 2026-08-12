---
# 標題帶上姓名：這頁是人名查詢最主要的落地頁，h1 只寫「關於我」等於浪費一次識別機會。
title: "關於曾建瑋 Peter Tseng"
# 需要自己的描述；沿用站台預設的話，搜尋摘要會跟首頁一模一樣。
description: "曾建瑋（Peter Tseng）：花蓮慈濟醫院公共傳播室，負責醫療衛教新聞監測、官網內容維護與網路健康議題輿情分析。個人網站記錄 AI、程式開發與生活隨筆。"
permalink: /about/
layout: single
author_profile: true
toc: true
toc_label: "目錄"
---

你好，我是**曾建瑋（Peter Tseng）**，在花蓮工作與生活。

## 我的工作

我服務於[花蓮慈濟醫院](https://hlm.tzuchi.com.tw/home/)公共傳播室。日常工作圍繞三件事：醫療衛教新聞的監測、醫院官網的內容維護，以及針對網路健康議題的輿情分析。

說得直白一點，就是讓醫院想說的話被聽見，也讓外界在說什麼被聽見。

## 我用程式做了什麼

資訊背景出身，工作卻落在醫院的傳播端。這個位置有個好處：看得見問題，手邊剛好也有工具。多數東西都是從「這樣做太蠢了吧」開始的。

### 醫療資料與 AI

- [**口腔癌篩檢異常預測**](https://github.com/petertsengtw/Oral-Cancer-Screening-Abnormality-Prediction) — 以人口特徵、生活習慣風險因子與歷次篩檢紀錄，用機器學習預測篩檢是否出現異常。資料來自花蓮慈濟醫院四癌篩檢資料庫（機構自有、去識別化，原始資料不進版控）。這其實是我十年前那份工作的下一章：當年把篩檢流程收攏成資料庫，現在試著讓那些資料回答問題。
- [**智慧醫療輿情助理**](/ai/2025/12/08/TZUCHI_ai_news.html) — 用 Groq + Llama 3.1 做醫院新聞輿情監測，含爬蟲、風險評分與自動摘要。原本每天要人工翻新聞，現在讓它自己跑。
- [**圖書館 AI 客服**](https://github.com/petertsengtw/REG-TZUCHI-Library) — 用 RAG 讓醫院圖書館的常見問題自己回答。

### 建院四十週年

那年院慶的數位需求，大致上是這三件事：

- [**紀念網站**](https://hlm.tzuchi.com.tw/anniversary/) — 純 HTML/CSS/JS，無框架、無後端、無 CDN，含開場動畫與特刊互動翻頁書。（[開發紀錄](/project/2026/03/31/ai_anniversary_40th.html)、[原始碼](https://github.com/petertsengtw/tzuchi_hospital-40th)）
- [**攝影比賽評分系統**](https://rate-photo.petertseng.me) — FastAPI + SQLite，評審匿名互不可見、投稿者資訊全程隔離、評分送出後鎖定。我跑模擬才發現同分機率高達 96%，於是設計了破同分規則。（[設計過程](/diary/2026/07/09/photo-contest.html)、[原始碼](https://github.com/petertsengtw/rate-photo)）
- [**拍攝時段預約系統**](https://photography-booking-5d7b5.web.app/) — 每 10 分鐘一個時段，靠 Firestore 做多裝置即時同步，杜絕重複預約。

### 把重複勞動變成工具

- [**繁體中文 PDF 校稿工具**](https://github.com/petertsengtw/chinese-proofreader) — 上傳 PDF、自動判斷橫書直書、呼叫 Claude API 抓錯別字，產出可下載的校稿報告。公傳室的稿子很多，這個省下的時間最實在。
- [**Word 轉 Joomla**](https://github.com/petertsengtw/doc-to-joomla) — Word 轉 HTML、自動提取圖片上傳伺服器，直接接上 Joomla。
- [**醫院新聞自動上稿**](https://github.com/petertsengtw/lotusnotes-com-tools) — 透過 COM API 從 Lotus Notes 撈出新聞稿，再接 Joomla API 直接上架。跟上面那個 Word 工具是同一條線的上下游：稿子從哪裡來、怎麼轉、怎麼進去。
- [**颱風門診公告產生器**](/diary/2026/07/10/typhoon.html) — 受夠了颱風夜反覆截圖改公告，寫了個上傳 Excel 就自動產生 HTML 的小工具。

### 官網與院內平台

- [**公共傳播室網站**](https://petertsengtw.github.io/hlm-pc/) — 公傳室的對外形象頁，順手把 Joomla 管理教學文件、傳播成效儀表板（YouTube／社群／GA 數據）和圖片轉 WebP 的小工具都收在同一個站上。院內同仁要找什麼，指這裡就好。（[原始碼](https://github.com/petertsengtw/hlm-pc)）
- [**多版本 Web Server 環境**](https://github.com/petertsengtw/tc_taichung_web) — 用 Docker 讓 PHP 7.4 和 8.3 的 Joomla 站並存，前面掛 Nginx Proxy Manager 依 domain 分流。舊網站一時升不上去，那就讓它們各自活著。

### 在學校寫的

- [**文獻分析助手**](https://github.com/petertsengtw/paper-analyzer) — 上傳論文 PDF，自動產出繁中摘要與優缺點，也能多篇比較。跑在本機的 Ollama + Qwen2.5 上，不外傳、不付 API 費。TAICA「生成式 AI 的人文導論」期末專案。
- [**HackMD 筆記同步**](https://github.com/petertsengtw/hackmd-sync) — 把雲端筆記整批抓成本地 `.md`，丟進 Obsidian 或給 LLM 讀。筆記寫在雲端很方便，要拿來用的時候就不方便了。
- [**AI 猜圖小遊戲**](https://github.com/petertsengtw/ai_pictionary) — Flask + Gemini，你在畫布上亂畫，它用繁中猜你畫了什麼。

### 其他

醫院的[大愛溯源館 360° 環景](https://hlm.tzuchi.com.tw/vr/museum.html)、[2024 醫療科技展環景](https://hlm.tzuchi.com.tw/home/index.php/expo2024-vr)、重陽敬老禮金的資格驗證系統，還有[玉里協天宮](https://github.com/petertsengtw/Yuli_Xietian)的官網——那間廟創建於清光緒元年，是花東第一廟。溯源館除了環景，另外有一套[電視牆播放系統](https://github.com/petertsengtw/Tzu-Chi-museum-tv-broadcast-system)，三個螢幕輪播影音——那是我第一次用 PHP 寫東西，沒有後台，檔案還得自己 FTP 丟上去。

再往外一點，[**土雞蛋訂購與管理系統**](https://github.com/petertsengtw/liff-egg-ordering-system)是少數跟醫院、公部門都無關的一個：LINE LIFF 當店面、Flask 接後端、Firestore 存資料、綠界收款，另外做了分批出貨、出貨修正和完整的審計紀錄。農產品沒辦法一次出貨，帳就得追得住。

## 在這之前

我的職涯大半在花蓮，起點卻在新竹。2000 到 2008 年，我在青草湖社區大學負責行政與學生資訊系統，也帶過國際志工計畫。

2009 年進花蓮慈濟醫院癌症中心，一待就是十年。那段時間主要在做國家癌症防治計畫的**花蓮慈濟醫院癌症篩檢管理系統**——把原本散落在紙本和各個窗口的篩檢流程，收攏成一套能追蹤、能提醒、能回報的東西，最特別的是用 HIS 資料來分析癌篩轉介成功率做決策，並設計有效的獎勵機制來提高癌篩率。這套系統後來拿到 **2018 年醫學中心組癌症篩檢創意金獎**，以及**智慧化癌症篩檢的 SNQ 國家品質標章**。

2019 到 2022 年我轉往花蓮縣政府社會處，負責智慧福利服務躍升計畫，用系統設計去改善社工的工作流程；也做了**花蓮縣長 LINEBOT**，讓縣民不必打電話就能查到社福資訊。

2022 年底回到慈濟醫院，就是現在的位置。2024 年起，我在國立東華大學資訊工程學系念碩士班。

回頭看，換過的單位不少，但做的其實一直是同一件事：把一套東西做出來，讓需要的人真的用得上。

## 這個部落格

站名叫「**碼上心經**」。人到中年，用寫程式和除錯的心態記錄人生，大概是這個意思。

這裡的文章其實分成兩種：

一種是**技術筆記** — AI Agent、LLM 應用、影片生成、開發環境設定，多半是我邊學邊記的實作過程，寫給未來會忘記的自己看。

另一種是**生活隨筆** — 跑步、家人、看過的電影、想不通的事。我從一個跑三圈操場就喘的胖子練到跑完半馬，也會在深夜陪女兒看動畫時毫無預警地哭出來。

兩種文章擺在一起看起來有點分裂，但對我來說是同一件事：都是把一段時間裡真正想過的事情留下來。

## 找我

如果你對醫療場域的 AI 應用、或這個網站上的任何內容有興趣，歡迎從左側的社群連結找到我。
