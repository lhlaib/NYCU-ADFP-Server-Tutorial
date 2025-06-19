# 05｜VPN 連線設定與登入教學

成功安裝 FortiClient VPN 後，請依照以下步驟**設定連線**與**成功登入 ADFP Cloud 2.0**。

---

## 📌 Step 1：確認你在校內網段

連線 VPN 前請先確認你目前所在位置：

- ✅ **陽明交大校內網路（含宿舍）**
- IP 格式應為 `140.113.xxx.xxx`

⚠️ 若非校內 IP，請參考 [校外連接 ADFP VPN 使用說明](https://adfp.si2.iee.nycu.edu.tw/knowledge-base/knowledge-base-2023-10-01/)

---

## 🔧 Step 2：開啟 FortiClient VPN，建立新連線設定

1. 開啟 FortiClient VPN 軟體  
2. 點選 `Configure VPN` 建立新連線

<img src="https://github.com/lhlaib/NYCU-ADFP-Server-Tutorial/blob/main/05_VPN_Connection/images/vpn_conn_01.png" width="300" alt="Step 2 畫面" />


---

## ✍️ Step 3：輸入連線參數

⚠️ **ADFP Cloud 3.0** 的 VPN 連線設定如下：

| 欄位名稱 | 設定值 |
|----------|--------|
| **Connection Name** | ADFP VPN |
| **Remote Gateway** | `vpn.adfp.iee.nycu.edu.tw` |
| **Port** | `443` --> **無需更改**|
| **Customize port** | 不勾選，預設 |


⚠️ **ADFP Cloud 2.0** 的 VPN 連線設定如下：

| 欄位名稱 | 設定值 |
|----------|--------|
| **Connection Name** | ADFP VPN |
| **Remote Gateway** | `v2.vpn.adfp.iee.nycu.edu.tw` |
| **Port** | `4433` --> **需更改**|
| **Customize port** | ✅ 勾選 |

| 欄位名稱 | 設定值 |
|----------|--------|
| **VPN Type** | SSL-VPN |
| **Username** | 你的 ADFP VPN 帳號 |
| **Password** | 你的 ADFP VPN 密碼（啟用系統取得） |

<img src="https://github.com/lhlaib/NYCU-ADFP-Server-Tutorial/blob/main/05_VPN_Connection/images/vpn_conn_02.png" width="300" alt="Step 3 畫面：連線參數設定" />

---

## 🔐 Step 4：按下「Connect」開始連線

點選「Connect」後，VPN 將開始驗證與連線程序。


<img src="https://github.com/lhlaib/NYCU-ADFP-Server-Tutorial/blob/main/05_VPN_Connection/images/vpn_conn_03.png" width="300" alt="Step 4 畫面" />

---

## ✅ Step 5：連線中彈出提示，請按「是」

當連線狀態到達 **20% 左右** 時，會跳出確認視窗，請點選「Yes」。

⚠️ 若未按「Yes」，VPN 將會卡住無法完成連線！


<img src="https://github.com/lhlaib/NYCU-ADFP-Server-Tutorial/blob/main/05_VPN_Connection/images/vpn_conn_04.png" width="300" alt="Step 5 畫面：確認提示" />

---

## 🎉 Step 6：出現 Connected 畫面，連線成功！

連線完成後會顯示 `Connected`，此時你已成功進入 ADFP 封閉式網路環境。

⚠️ **連上 VPN 後將無法使用一般網路（如 YouTube、Google 等）**  
若需使用外部網路，請記得「中斷 VPN」後再操作。

<img src="https://github.com/lhlaib/NYCU-ADFP-Server-Tutorial/blob/main/05_VPN_Connection/images/vpn_conn_05.png" width="300" alt="Step 6 畫面：連線成功" />

---

## 🌐 Step 7：你可以使用以下 ADFP 專用服務

| 服務名稱 | 連線方式 |
|----------|----------|
| Account Service | https://account.adfp.iee.nycu.edu.tw:5001/ |
| Chat Service | https://account.adfp.iee.nycu.edu.tw:20001/ |
| FTP Service | ftp://ftp.adfp.iee.nycu.edu.tw:54238 |
| ADFP Cloud 2.0 (遠端桌面) | `cad11~14.iee.nycu.edu.tw:4151`（詳見第 6 章） |
| ADFP Cloud 3.0 (遠端桌面) | （詳見第 7 章） |

---

## 🔌 Step 8：連線完成後請勿關閉 VPN 程式

請讓 VPN 保持「連線狀態」執行中，不要誤按「Disconnect」，否則將無法存取任何 ADFP Cloud 功能。



---

## ❌ Step 9：結束使用時，記得手動「中斷連線」

- 在 FortiClient 主畫面點選「Disconnect」即可結束連線
- VPN 結束後將恢復一般網路功能

<img src="https://github.com/lhlaib/NYCU-ADFP-Server-Tutorial/blob/main/05_VPN_Connection/images/vpn_conn_06.png" width="300" alt="Step 8 畫面：連線狀態" />

---

📘 返回 [主教學首頁](../README.md)

➡️ 下一章節 ADFP Cloud 2.0：
[06 | 連線：ADFP Cloud 2.0 遠端桌面教學](../06_Remote_Desktop_V2/README.md)

➡️ 下一章節 ADFP Cloud 3.0：
[07 | 連線：ADFP Cloud 3.0 遠端桌面教學](../07_Remote_Desktop_V3/README.md)

⬅️ 上一章節：
[04 | 安裝：VPN軟體](../04_VPN_Setup/README.md)