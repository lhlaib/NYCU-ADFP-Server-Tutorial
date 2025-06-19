# NYCU-ADFP-Server-Tutorial

這份教學是專門為交大修習 ADFP 課程的同學所設計的「一站式入門指南」。 

無論你是第一次碰 VPN、搞不定遠端桌面，還是不知道什麼是 ADFP，只要按照這份教學逐步操作，能讓你從帳號啟用 → VPN 連線 → 繳交作業，都能**無痛上手、完成課程任務**

## ⭐️ 收藏教學筆記

 
為了讓你之後更快找到這份教學資源，請記得：

👉 **到 GitHub 頁面點一下 Star ⭐️ 收藏起來！**

[![GitHub Stars](https://img.shields.io/github/stars/lhlaib/NYCU-ADFP-Server-Tutorial.svg?style=social)](https://github.com/lhlaib/NYCU-ADFP-Server-Tutorial)   [![GitHub Follow](https://img.shields.io/github/followers/lhlaib?label=Follow&style=social)](https://github.com/lhlaib)

## 📢 加入社群
為了讓你能隨時獲得最新公告、問題解答與技術支援，請務必加入我們的 Discord 社群：
👉 [ADFP Cloud Discord 社群](https://discord.gg/3HF8b8WDju)

---

## ☁️ 關於 ADFP Cloud 2.0 / 3.0

ADFP（Advanced Design Flow Platform）是 TSMC 提供的 16nm FinFET 製程（N16），是全球第一個 FinFET 虛擬製程教學平台，能與業界技術無縫接軌。

我們實驗室建置了 **ADFP Cloud 2.0 與 3.0 雲端平台**：

- 💻 **ADFP Cloud 2.0**：採用三層式伺服器架構  
- ⚙️ **ADFP Cloud 3.0**：升級虛擬化超融合架構，硬體配置、實驗性功能、支援高負載模擬



🌟 **使用 TSMC 提供的 ADFP 虛擬製程設計晶片，只供教學用途，若要用於研究發表請用真實製程 TN16 / TN7。**

---

## 📚 教學章節目錄

| 章節 | 主題 | 內容連結 |
|------|------|-----------|
| 00 | 使用規範與注意事項 | 👉 [使用政策與基本限制](./00_Rules_and_Policy/) |
| 01 | 啟用：帳號啟用 | 👉 [啟用流程、密碼修改](./01_Account_Activation/) |
| 02 | 設定：Windows 安全性 | 👉 [密碼設定、自動鎖定教學](./02_Windows_Security/) |
| 03 | 安裝：防毒軟體 | 👉 [Windows Apex One 教學](./03_Antivirus_Setup/) |
| 04 | 安裝：VPN軟體 | 👉 [FortiClient VPN 設定](./04_VPN_Setup/) |
| 05 | 連線：VPN 連線教學 | 👉 [VPN 連線教學](./05_VPN_Connection/) |
| 06 | 連線：ADFP Cloud 2.0 遠端桌面教學 | 👉 [2.0 XRDP 使用說明](./06_Remote_Desktop_V2/) |
| 07 | 連線：ADFP Cloud 3.0 遠端桌面教學 | 👉 [3.0 XRDP 使用說明](./07_Remote_Desktop_V3/) |
| 08 | 製程資料存取 | 👉 [FinFET 資料夾與文件位置](./08_Process_Data/) |
| 09 | FTP 檔案上傳 | 👉 [檔案上傳說明](./09_FTP_Upload/) |
| 10 | ADFP Chat 問答系統 | 👉 [課程討論、學生檔案繳交](./10_Chat_System/) |
| 11 | 校外 VPN 設定教學 | 👉 [校外 VPN 連線設定](./11_OffCampus_VPN/) |

---

## ❓ 常見 Q&A（FAQ）
👉 **Q：VPN 無法連上，怎麼辦？**  
> 請先確認是否已新增自己的校外 IP（可參考「11_OffCampus_VPN」章節），或確認密碼是否已過期。

👉 **Q：登入遠端桌面後出現黑畫面？**  
> 可能是解析度不相容、或多重登入造成。建議關閉所有舊連線，重啟 VPN 並重新登入。

👉 **Q：我在 FTP 上傳檔案後去哪裡找？**  
> 登入遠端桌面，在 `/FTP_UPLOAD/` 資料夾內查看。記得立即複製到家目錄，否則會被定期清除！

👉 **Q：我要繳交作業，要放在哪裡？**  
> 每次作業請統一放入 `~/Submit/作業名稱/` 並搭配 Chat 系統留言通知助教。

👉 **Q：ADFP Chat 可以用手機看嗎？**  
> 不可以！ADFP Chat 僅能透過伺服器內網（VPN）瀏覽器開啟，**禁止翻拍螢幕分享至外部平台**！

---

## 📩 技術支援
請務必加入官方 Discord 伺服器接收公告與回報問題：
👉 https://discord.gg/3HF8b8WDju

> 📢 **請所有同學與課程助教務必加入 Discord 社群**，以便即時接收如「伺服器重啟」、「停機維護」、「帳號公告」等通知。此類資訊僅會透過 Discord 公告，不再另外寄送 Email 通知。

🚫 請注意以下事項：

- **學生請勿直接寄信給管理員，管理員不處理任何學生個別 Email 回覆**
- 所有問題請**先由學生回報給課程助教**
- 助教確認後可於 Discord 群組向管理員提問


📣 以下狀況請一律「**向課程助教回報**」，由助教代為處理與轉交：

- 帳號顯示 `Quota exceed` 或無法儲存檔案
- 忘記 VPN 或遠端桌面登入密碼
- VPN 無法連線、出現錯誤碼
- 不熟悉伺服器使用流程、不會登入 XRDP
- FTP 或 Chat 系統使用問題

📣 **請課程助教協助提醒修課同學盡快加入 Discord 社群**。

## 🚀 快速連結

| 類別 | 連結 |
|------|------|
| ADFP 帳號系統 | [https://account.adfp.iee.nycu.edu.tw:5001/](https://account.adfp.iee.nycu.edu.tw:5001/) |
| ADFP Chat | [https://account.adfp.iee.nycu.edu.tw:20001/](https://account.adfp.iee.nycu.edu.tw:20001/) |
| 實驗室官網 | [https://iclab.iee.nycu.edu.tw/iclab/](https://iclab.iee.nycu.edu.tw/iclab/) |
| 帳號申請系統 | [https://iclab.iee.nycu.edu.tw/iclab/apply_system/apply.php/](https://iclab.iee.nycu.edu.tw/iclab/apply_system/apply.php) |

---

## 🚀 運算資源總覽（ADFP Cloud 2.0 / 3.0）

### 🔹 ADFP Cloud 2.0：實體高效能伺服器資源

| Host   | CPU (Threads)                      | Memory | OS         | SSD      |
|--------|------------------------------------|--------|------------|----------|
| cad10  | AMD EPYC™ 7543 @ 2.80GHz (128)     | 256GB  | CentOS 7.9 | 185TB    |
| cad11  | AMD EPYC™ 7773X @ 2.2GHz (256)     | 1024GB | CentOS 7.9 | 7.3TB    |
| cad12  | AMD EPYC™ 7773X @ 2.2GHz (256)     | 1024GB | CentOS 7.9 | 7.3TB    |
| cad13  | AMD EPYC™ 7713 @ 2.00GHz (256)     | 1024GB | CentOS 7.9 | 7.3TB    |
| cad14  | AMD EPYC™ 7713 @ 2.00GHz (256)     | 1024GB | CentOS 7.9 | 7.3TB    |

---

### 🔸 ADFP Cloud 3.0：虛擬化教學平台（CUBE OS HCI）

| 區域     | 伺服器 CPU / Core / Clock        | Memory | SSD         | VM 數量與配置             |
|----------|----------------------------------|--------|-------------|----------------------------|
| 課程區   | AMD 9654 (192C, 3.55GHz)   × 3      | 1TB    | 30.72TB SSD | 4 × VM（100C / 400GB）     |
|          |                                  |        |             | 2 × TA-VM（100C / 400GB）  |
| 研究區   | AMD 9474F (96C, 3.95GHz) × 4      | 1TB    | 30.72TB SSD | 4 × VM（100C / 400GB）     |
|          |                                  |        |             | 2 × TA-VM（100C / 400GB）  |
| 資料 VM  | –                                | 100GB  | 80TB SSD    | 存放 ADFP 資料與授權     |

> 💡 ADFP Cloud 3.0 採用 CUBE OS HCI 架構，支援 snapshot 快照、SFTP 安全傳輸、跨 VM 快速部署，為研究與教學提供穩定彈性的資源配置。


---

## 👥 貢獻者名單（Contributors）

感謝以下夥伴協助本教學系統的撰寫與維護 🙌

- 賴林鴻（[@lhlaib](https://github.com/lhlaib)）
- 王鈺翔（[@yushinnycu](https://github.com/yushinnycu)）
- 蕭邦原（[@bonyuan](https://github.com/bonyuan)）
- 廖展儀（[@ricky-liao](https://github.com/ricky-liao)）
- 洪瑜辰（[@yuchenhong](https://github.com/yuchenhong)）


[![Contributors](https://contrib.rocks/image?repo=lhlaib/NYCU-ADFP-Server-Tutorial)](https://github.com/lhlaib/NYCU-ADFP-Server-Tutorial/graphs/contributors)


---

©2025 System Integration and Silicon Implementation Lab, NYCU  
All rights reserved. For educational use only.
