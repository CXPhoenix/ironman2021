---
title: "Day 1: 「你還在手動啊？」一起來看看簡單的自動化吧！"
tags: "2021鐵人賽"
---

Day 1: 「你還在手動啊？」- 一起來看看簡單的自動化吧！\
鳳黃酥的 Google 自動化旅程
==

### **引言**
大家好，我是 CXPhoenix ，你可以叫我 Phoenix ，平時都是在學校服務廣大~~妖魔鬼怪~~莘莘學子資訊科技的奧妙。但是其實在學校的老師往往不只是要會教書，你還要根據你的科別或是你的行政職而擁有十八般武藝。\
舉個例子，我是資訊科技老師兼任資訊組的協助行政，所以基本上我要會：
* 架網站
* 寫軟體
* 修網路
* 回答老師們的資訊相關問題
* ~~通靈~~
* ~~插插頭~~


先說，我沒有要抱怨的意思（真的啦！）

但是也就在這段歲月裡，我也不小心多學了一些稀奇古怪的知識，本持著每次跟學生說的「開源精神」，想跟大家分享分享我學習到的東東。\
接下來的 30 天裡，我將要跟各位分享我最近在處理眾多神奇的案件中，發現意外好用的:
<center><img src="https://i.imgur.com/JngRRpw.png" title="source: imgur.com" /></center>

---
<br>

### **Google Apps Script**
其實我相信版友們對於這個 Google 大神所推出的服務並不會陌生，~~至少沒看過 GAS 跑起來也聽過 GAS 的芳名吧~~。

Google Apps Script （簡稱 GAS 或是 gas）是以一個大家耳熟能詳的前端三本柱之一 JavaScript 為基礎的伺服器端腳本語言 (server-side scripting language)，他並非是一般的 JavaScript 一樣 ~~（廢話）~~ 是以一般瀏覽器為主 (browser-based) 的語言，而是運作於 Google 的伺服器上，能夠直接存取存放在 Google 伺服器中的資料。近來更是支援 Modern JS 的撰寫方式，讓大家在程式設計上更方便。

GAS 其實原本只是 Google 工程師 Mike Harm 想要在 Google Sheets 上實現跟 MS Excel 可以用 VB 撰寫程式的一個 side project。沒想到這樣的功能 ~~（哈欠）~~ 卻被 Google 青睞，因此被拿來...作為...zzzz....

恩？發生什麼事情？...阿～我睡著了..

好了，不開玩笑了！

其實網路上查得到非常多的相關資料，為了讓廣大版友發揮 108 課綱的「終生學習」精神， ~~絕對不是我想偷懶，~~ 因此我就不在這邊贅述太多關於 GAS 的理論知識了。
~~反正講這些無聊的會睡著你是知道的...~~

**就讓我們來專注於實作吧！**

由於，本篇的主要目標族群是針對一些可能跟前端語言沒這麼熟的版友，因此我將會從基礎出發，延伸至 GAS 的應用：
* JS 的基本語法與使用
* GAS 的基本操作
* 看懂 GAS 的神奇文件
* 利用 GAS 操作 **文件**、**雲端硬碟**、**表單**、**試算表** 等等 Google 常用服務。
* 利用 GAS 結合 HTML 技術打造雲端網頁
* 實作一些 GAS 應用的自動化功能系統

<br>

就讓我們一起探索這個神奇的 Google Apps Script 世界中吧！

---
<br>

## **目錄**

&emsp;&emsp;Day 1: 「你還在手動啊？」- 一起來看看簡單的自動化吧！（就是本篇）

&emsp;&emsp;Day 2: 「先來看看你的實驗對象吧！」- GAS 編輯器初探

JavaScript 篇\
&emsp;&emsp;Day 3: 「JS 好棒棒！」- JS 初探與資料儲存\
&emsp;&emsp;Day 4: 「往左走往右走」- JS 的結構化程式設計 1 - 選擇條件結構\
&emsp;&emsp;Day 5: 「跑操場的痛苦修行」- JS 的結構化程式設計 2 - 重複結構\
&emsp;&emsp;Day 6: 「不要一直寫重複的話」- JS 的模組化程式設計

Google Apps Script 基礎篇\
&emsp;&emsp;Day 7: 「87% 的純度」 - 從 JS 到 GAS\
&emsp;&emsp;Day 8: 「推廣一下終身學習」 - GAS 的參考文件去哪看？\
&emsp;&emsp;Day 9: 「簡單的實作」 - GAS 的基礎功能\
&emsp;&emsp;Day 10: 實作 1: 用 GAS 寄封信吧!

GAS X 試算表\
&emsp;&emsp;Day 11: 「神奇的 Google DB」試算表的 CRUD 1 - 新增與讀取\
&emsp;&emsp;Day 12: 「神奇的 Google DB」試算表的 CRUD 1 - 更新與刪除\
&emsp;&emsp;Day 13: 實作 2: 自動化會議通知

GAS X 雲端硬碟\
&emsp;&emsp;Day 14: 獲得雲端硬碟中的資料\
&emsp;&emsp;Day 15: 在雲端硬碟中創造檔案\
&emsp;&emsp;Day 16: 刪除在雲端硬碟中的檔案\
&emsp;&emsp;Day 17: 實作 3: 

GAS X 文件\
&emsp;&emsp;Day 18: 還在想..