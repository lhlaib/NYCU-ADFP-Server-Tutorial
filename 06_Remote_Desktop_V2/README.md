# 06｜遠端桌面連線教學

成功連線FortiClient VPN 後，我們就可以透過 **Windows 內建的遠端桌面（Remote Desktop）功能**，進入 ADFP Cloud 伺服器進行 IC 設計操作。

請依照下列步驟設定與登入，開始你的 FinFET 設計旅程！

---

## 💻 Step 1：開啟遠端桌面應用程式

在 Windows 搜尋欄輸入：  
> `遠端桌面連線` 或 `Remote Desktop Connection`  

點選進入應用程式。

<img src="https://github.com/lhlaib/NYCU-ADFP-Server-Tutorial/blob/main/06_Remote_Desktop_V2/images/remote_01.png" width="300" alt="Step 1 畫面" />

---

## 🖥️ Step 2：輸入伺服器主機位址

請輸入以下任一台 ADFP Cloud 2.0 設計伺服器的 IP：

```

cad11.si2.iee.nycu.edu.tw:4151  
cad12.si2.iee.nycu.edu.tw:4151  
cad13.si2.iee.nycu.edu.tw:4151  
cad14.si2.iee.nycu.edu.tw:4151

```

⚠️ 若你有被助教分配特定主機，請以該主機為主。

 
<img src="https://github.com/lhlaib/NYCU-ADFP-Server-Tutorial/blob/main/06_Remote_Desktop_V2/images/remote_02.png" width="300" alt="Step 2 畫面" />

---

## 🎨 Step 3：設定顯示選項與色彩品質

1. 點選左下角「**顯示選項（Show Options）**」
2. 前往「**顯示（Display）**」頁籤
3. 建議設定為：**全彩 24 位元**
4. 點選「**連線**」

<img src="https://github.com/lhlaib/NYCU-ADFP-Server-Tutorial/blob/main/06_Remote_Desktop_V2/images/remote_03.png" width="300" alt="Step 3 畫面" />

<img src="https://github.com/lhlaib/NYCU-ADFP-Server-Tutorial/blob/main/06_Remote_Desktop_V2/images/remote_04.png" width="300" alt="Step 3 畫面" />

---

## 🚪 Step 4：按「是」接受連線憑證

首次登入會出現安全性警告，請按下「是（Yes）」繼續。

<img src="https://github.com/lhlaib/NYCU-ADFP-Server-Tutorial/blob/main/06_Remote_Desktop_V2/images/remote_05.png" width="300" alt="Step 4 畫面" />

---

## 🔐 Step 5：輸入帳號與密碼

畫面將提示輸入 ADFP Server 帳號密碼  
（此帳號密碼與你 VPN 帳號相同，或由開通系統提供）

<img src="https://github.com/lhlaib/NYCU-ADFP-Server-Tutorial/blob/main/06_Remote_Desktop_V2/images/remote_06.png" width="300" alt="Step 5 畫面" />


---

## 🎉 Step 6：成功登入 ADFP 桌面環境

<img src="https://github.com/lhlaib/NYCU-ADFP-Server-Tutorial/blob/main/06_Remote_Desktop_V2/images/remote_07.png" width="300" alt="Step 6 桌面畫面" />

你會看到 CentOS 7.9 桌面環境與多個捷徑圖示，包括：

- `ADFP`：製程文件夾 
 <img src="https://github.com/lhlaib/NYCU-ADFP-Server-Tutorial/blob/main/06_Remote_Desktop_V2/images/remote_08.png" width="100" alt="Step 6: ADFP_PDF 圖示" />

- `ADFP_PDF`：浮水印限制文件夾  
<img src="https://github.com/lhlaib/NYCU-ADFP-Server-Tutorial/blob/main/06_Remote_Desktop_V2/images/remote_09.png" width="100" alt="Step 6: Floating_Docs 圖示" />

- `Home`：你的個人資料夾  
<img src="https://github.com/lhlaib/NYCU-ADFP-Server-Tutorial/blob/main/06_Remote_Desktop_V2/images/remote_10.png" width="100" alt="Step 6: Home 圖示" />

- `Screenshot`：內建截圖工具 
<img src="https://github.com/lhlaib/NYCU-ADFP-Server-Tutorial/blob/main/06_Remote_Desktop_V2/images/remote_11.png" width="600" alt="Step 6: Screenshot 圖示" />
雙擊後會出現十字後框，選要擷取的地方，即可將照片擷取至 Picture資料夾
<img src="https://github.com/lhlaib/NYCU-ADFP-Server-Tutorial/blob/main/06_Remote_Desktop_V2/images/remote_12.png" width="300" alt="Step 6: Xfce Terminal 圖示" />

- `Monitor`：監控系統資源使用情況  
<img src="https://github.com/lhlaib/NYCU-ADFP-Server-Tutorial/blob/main/06_Remote_Desktop_V2/images/remote_13.png" width="300" alt="Step 6: Monitor 圖示" />

- `Xfce Terminal`：好用的終端機  
<img src="https://github.com/lhlaib/NYCU-ADFP-Server-Tutorial/blob/main/06_Remote_Desktop_V2/images/remote_14.png" width="300" alt="Step 6: Xfce Terminal 圖示" />


---

## ⚙️ Step 7：啟用 EDA 工具環境（首次登入）

在桌面按右鍵，打開 Terminal （白色介面），或是桌面捷徑、從Applications -> System Tools -> Xfce Terminal （黑色介面）。

<img src="https://github.com/lhlaib/NYCU-ADFP-Server-Tutorial/blob/main/06_Remote_Desktop_V2/images/remote_16.png" width="600" alt="Step 7: Terminal 圖示" />
在 Terminal 中輸入：

```
yes
```

即可 source 並啟用完整的 EDA Tool 開發環境路徑。

<img src="https://github.com/lhlaib/NYCU-ADFP-Server-Tutorial/blob/main/06_Remote_Desktop_V2/images/remote_17.png" width="600" alt="Step 7: Terminal 啟用 EDA Tool" />

## 🧼 Step 9：離開遠端桌面的兩種方式

### ✅ 方法一：暫時關閉遠端桌面（不中斷程式）

*   直接關閉遠端桌面視窗
    
*   適用於模擬中長時間執行或背景作業不中斷
    

⚠️ 請注意: 長時間離線或中斷連線未依流程登出，可能導致下次登入時發生異常。
因為資源仍在運行中，可能會導致帳號鎖住或資源卡住！！

<img src="https://github.com/lhlaib/NYCU-ADFP-Server-Tutorial/blob/main/06_Remote_Desktop_V2/images/remote_18.png" width="600" alt="Step 9 畫面：關閉遠端桌面" />


### ✅ 方法二：正確登出系統（關閉所有程式）

若今日工作結束，請點選右上角電源圖示 → 「Log Out」  
這將關閉所有正在執行的應用程式並釋放資源

⚠️ 請務必在每次使用完畢後Log Out 來確保連線品質

<img src="https://github.com/lhlaib/NYCU-ADFP-Server-Tutorial/blob/main/06_Remote_Desktop_V2/images/remote_19.png" width="600" alt="Step 9 畫面：登出系統" />


🔌 Step 10：中斷 VPN 以恢復一般網路
-------------------------

最後，請回到 FortiClient VPN → 按下 `Disconnect`  
即可結束 ADFP 封閉式連線，恢復正常網路瀏覽。



📌 小提醒
------

| 操作 | 注意事項 |
| --- | --- |
| 忘記登出 | 可能導致帳號鎖住或資源卡住 |
| 長時間使用 | 請確認已改用 meaningful 程式名（勿用 a.out） |
| 無法登入 | 檢查是否未中斷上次連線，或詢問助教協助 reset |



📘 返回 [主教學首頁](../README.md)