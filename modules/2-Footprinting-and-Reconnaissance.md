# <u>偵查與足跡收集</u>

> ⚡️ **此章節包含[實戰實驗室](https://github.com/Samsar4/Ethical-Hacking-Labs/tree/master/1-Footprinting-and-Reconnaissance)**

## <u>足跡收集（Footprinting）</u>
足跡收集是偵查過程的一部分，用於收集有關目標計算機系統或網絡的可能資訊。

在計算機安全術語中，"足跡收集" 通常指攻擊前的階段之一；在實際攻擊之前執行的任務。**用於足跡收集的一些工具包括 Sam Spade, nslookup, traceroute, Nmap 和 neotrace。**

## 足跡收集類型：<u>主動和被動</u>

- **主動** - 需要攻擊者接觸設備或網絡
  - 社交工程和其他需要與目標互動的通信
- **被動** - 從公開可用的來源收集資訊的措施
  - 網站、DNS 記錄、商業資訊數據庫

### 足跡收集有助於：

- **了解安全狀態** - 收集到的資料將有助於我們了解公司的安全狀態，例如防火牆的存在、應用程序的安全配置等詳細資訊。

- **減少攻擊範圍** - 可以識別特定範圍的系統並僅專注於特定目標。這將大大減少我們關注的系統數量。

- **識別漏洞** - 我們可以建立一個資訊數據庫，其中包含目標組織系統中的漏洞、威脅、漏洞。

- **繪製網絡地圖** - 有助於繪製目標組織網絡的網絡地圖，涵蓋拓撲、可信路由器、服務器的存在和其他資訊。

足跡收集可以是**被動**和**主動**的。查看公司網站是被動足跡收集的一個例子，而通過社交工程試圖獲得敏感資訊則是主動資訊收集的一個例子。

在此階段，駭客可以收集以下資訊（僅為高級資訊）：

- **域名 (Domain name)**
- **IP 位址 (IP Addresses)**
- **命名空間 (Namespaces)**
- **員工資訊 (Employee information)**
- **電話號碼 (Phone numbers)**
- **電子郵件 (E-mails)**
- **工作資訊 (Job Information)**

可以是：
  - **匿名 (Anonymous)** - 收集資訊而不暴露自己的任何資訊
  - **偽名 (Pseudonymous)** - 使別人為你的行為承擔責任

**競爭情報 (Competitive Intelligence)** - 企業收集的競爭對手資訊

**Alexa.com** - 提供有關網站統計資料的資源

## 足跡收集目標

- **網絡 (Network)**
  - DNS
  - IP 網絡
  - 可訪問系統
  - 網站
  - 訪問控制
  - VPN 端點
  - 防火牆供應商
  - IDS 系統
  - 路由/路由協議
  - 電話系統（模擬/網絡語音）

- **組織 (Organization)**
  - 組織結構
  - 網站
  - 電話號碼
  - 目錄資訊
  - 辦公地點
  - 公司歷史
  - 商業聯繫

- **主機 (Hosts)**
  - 監聽服務
  - 操作系統版本
  - 互聯網可達性
  - 枚舉資訊
  - SNMP 資訊
  - 用戶/組
  - 行動設備

## <u>方法和工具</u>

### 搜索引擎

- **[NetCraft](https://www.netcraft.com/)** - 繪製有關目標網站的技術和資訊的綜合清單。

- **求職網站** - 可從招聘信息中獲取有關技術的資訊。
- **Google 搜索 | Google dorks：** 
  - `filetype:`  - 查找文件類型
  - `index of` - 目錄列表
  - `info:` - 包含 Google 對該頁面的資訊
  - `intitle:` - 標題中的字符串
  - `inurl:` - URL中的字符串
  - `link:` - 查找已連結的頁面
  - `related:` - 查找相似的頁面
  - `site:` - 查找特定網站的頁面
    - **示例**：
    - ![google-dorks](https://miro.medium.com/max/659/0*GGRvHnh59qi5lVB9.png)
  - [GHDB](https://www.exploit-db.com/google-hacking-database) 非常適合學習 Google Dorks 以及它在現實世界情境中是如何實現的
- **Metagoofil** - 命令行界面，使用 **Google hacks** 在元標籤中查找資訊（域名、文件類型等；是終端機的 google dorks）。

### 網站腳印追踪

- **網站鏡像 | 網站克隆** - 允許離線進行隱蔽測試
  - **HTTrack** - *您可以使用 CLI 版本或 Web Interface 版本*
  - **Wget** - Linux 命令 
    - `wget -mk -w 10 http://hackthissite.org/`
  - **Black Widow**
  - **WebRipper**
  - **Teleport Pro**
  - **Backstreet Browser**
- **Archive.org / [Wayback machine](https://archive.org/web/)** 
- 提供不同日期的緩存網站，可能包含已刪除的敏感資訊。
  - **Wayback Machine -> Google.com**：
    - ![wayback](https://searchengineland.com/figz/wp-content/seloads/2011/01/archive41-500x256.png)

### 電子郵件腳印追踪

- **電子郵件標頭** - 可能顯示伺服器及其位置
  - 電子郵件標頭可以提供：**姓名、地址（IP、電子郵件）、郵件伺服器、時間戳、認證等。**
    - ![emailheader](https://www.wikihow.com/images/thumb/7/72/Read-Email-Headers-Step-7.jpg/v4-460px-Read-Email-Headers-Step-7.jpg.webp)
  - **EmailTrackerPro** 是一款 Windows 軟件，可以追踪電子郵件回到其真實的來源點 (譯註: 這個產品於2023年停產)

- **電子郵件追踪** - 服務可以追踪各種資訊，包括打開郵件的 IP 地址、郵件去向等。

### DNS 腳印追踪

- 端口

  - 名稱查找(Name lookup) - UDP 53
  - 區域傳輸(Zone transfer) - TCP 53

- 區域傳輸複製所有記錄

- **名稱解析器** 回答請求

- **權威伺服器** 持有一個命名空間的所有記錄

- **DNS 記錄類型**

  - | 名稱  | 描述        | 用途                                        |
    | ----- | ------------------ | ---------------------------------------------- |
    | SRV   | 服務            | 指向特定服務                   |
    | SOA   | 起始授權 | 表示命名空間的權威 NS |
    | PTR   | 指針            | 將 IP 映射到主機名                       |
    | NS    | 名稱伺服器         | 列出命名空間的名稱伺服器          |
    | MX    | 郵件交換      | 列出電子郵件伺服器                            |
    | CNAME | 別名     | 將名稱映射到 A 記錄                    |
    | A     | 地址            | 將主機名映射到 IP 地址              |

- **DNS 汙染（DNS Poisoning）** - 改變機器上的緩存，將請求重定向到惡意伺服器

- **DNSSEC** - 通過加密記錄來防止 DNS 汙染

- **SOA 記錄字段**

  - **源主機（Source Host）** - 主要 DNS 的主機名
  - **聯繫電子郵件（Contact Email）** - 負責區域檔案的人的電子郵件
  - **序列號（Serial Number）** - 每次更改都會遞增的修訂號
  - **刷新時間（Refresh Time）** - 應進行更新的時間
  - **重試時間（Retry Time）** - NS 應等待失敗的時間
  - **過期時間（Expire Time）** - 允許區域傳輸完成的時間
  - **TTL** - 區域內記錄的最小 TTL

- **IP 地址管理**

  - **ARIN** - 北美洲
  - **APNIC** - 亞太地區
  - **RIPE** - 歐洲，中東
  - **LACNIC** - 拉丁美洲
  - **AfriNIC** - 非洲

- **Whois** - 從命令行或網絡界面獲取域的註冊信息。
  - 在 Kali 上，命令行界面上已經預裝了 whois；例如：`whois google.com`
  - 在 Windows 上，您可以使用 **SmartWhois** GUI 軟件執行 whois，或使用像 domaintools.com 這樣的網站
- **Nslookup** - 執行 DNS 查詢；（Nslookup 已預裝在 Kali Linux 上）

  - `nslookup www.hackthissite.org`
  - ```
    Server:         192.168.63.2
    Address:        192.168.63.2#53

    Non-authoritative answer:
    Name:   www.hackthissite.org
    Address: 137.74.187.103
    Name:   www.hackthissite.org
    Address: 137.74.187.102
    Name:   www.hackthissite.org
    Address: 137.74.187.100
    Name:   www.hackthissite.org
    Address: 137.74.187.101
    Name:   www.hackthissite.org
    Address: 137.74.187.104
    ```
    - 前兩行顯示了我的當前 DNS 伺服器；返回的 IP 地址是“**A 記錄**”，意味著域的 IPv4 地址；最後一行 NsLookup 查詢指定的 DNS 伺服器，並檢索與域關聯的請求的記錄。

  - **以下類型的 DNS 記錄在 Nslookup 上特別有用：**


    - | 類型  | 描述        |
      | ----- | ------------------ |
      | A     | 域名的 IPv4 地址          |
      | AAAA  | 域名的 IPv6 地址          |
      | CNAME | 典型名稱 — 允許一個域名映射到另一個域名。這允許多個網站引用單個 Web 伺服器。          | 
      | MX    | 處理域的電子郵件的伺服器。        |
      | NS    | 域的一個或多個授權名稱伺服器記錄。          | 
      | TXT   | 包含供 DNS 伺服器之外使用的信息的記錄。內容以 name=value 的形式呈現。這些信息用於許多事物，包括 SPF 和 DKIM 等身份驗證方案。          |

  - **Nslookup - 交互式模式區域傳輸** (交互式模式允許用戶查詢名稱伺服器以獲得有關各種主機和域的資訊，或打印域中主機的列表)。
    - `nslookup`
    - `server <IP 地址>`
    - `set type = <DNS 類型>`
    - `<目標域>`
  - ```
    nslookup 
    > set type=AAAA                                                                                                                                            
    > www.hackthissite.org
    Server:         192.168.63.2                                                                                                                               
    Address:        192.168.63.2#53                                                                                                                            
                                                                                                                                                              
    非授權回答：                                                                                                                                
    Name:   www.hackthissite.org                                                                                                                               
    Address: 2001:41d0:8:ccd8:137:74:187:103                                                                                                                   
    Name:   www.hackthissite.org                                                                                                                               
    Address: 2001:41d0:8:ccd8:137:74:187:102                                                                                                                   
    Name:   www.hackthissite.org                                                                                                                               
    Address: 2001:41d0:8:ccd8:137:74:187:101                                                                                                                   
    Name:   www.hackthissite.org                                                                                                                               
    Address: 2001:41d0:8:ccd8:137:74:187:100
    Name:   www.hackthissite.org
    Address: 2001:41d0:8:ccd8:137:74:187:104
    ```
- **Dig** - 類似於 nslookup 的 Unix-based 命令

  - `dig <目標>`
  - ```
    dig www.hackthissite.org

    ; <<>> DiG 9.16.2-Debian <<>> www.hackthissite.org
    ;; global options: +cmd
    ;; Got answer:
    ;; ->>HEADER<<- opcode: QUERY, status: NOERROR, id: 51391
    ;; flags: qr rd ra; QUERY: 1, ANSWER: 5, AUTHORITY: 0, ADDITIONAL: 1

    ;; OPT PSEUDOSECTION:
    ; EDNS: version: 0, flags:; MBZ: 0x0005, udp: 4096
    ;; QUESTION SECTION:
    ;www.hackthissite.org.          IN      A

    ;; ANSWER SECTION:
    www.hackthissite.org.   5       IN      A       137.74.187.104
    www.hackthissite.org.   5       IN      A       137.74.187.101
    www.hackthissite.org.   5       IN      A       137.74.187.100
    www.hackthissite.org.   5       IN      A       137.74.187.102
    www.hackthissite.org.   5       IN      A       137.74.187.103

    ;; Query time: 11 msec
    ;; SERVER: 192.168.63.2#53(192.168.63.2)
    ;; WHEN: Tue Aug 11 15:05:01 EDT 2020
    ;; MSG SIZE     rcvd: 129

    ```
  - 若要獲得電子郵件記錄，請指定 `-t MX`
    - `dig <目標> -t MX`
  - 若要獲得區域傳輸，請指定 `axfr`

### 網絡腳印追踪

- IP 地址範圍可以從地區註冊商獲得（例如：美洲的 ARIN，歐洲的 RIPE 等）

- 使用 `traceroute` 查找中間服務器
  - Windows 中的 traceroute 使用 ICMP echo（tracert）
  - traceroute 適用於檢測防火牆和網絡路徑

**使用示例**：
  - **`traceroute -I nsa.gov`**
    - 指定目標：`traceroute <target>`
    - 在此情況下，使用 ICMP ECHO 進行路由跟踪：`-I`
```
traceroute -I nsa.gov
traceroute to nsa.gov (104.83.73.99), 30 hops max, 60 byte packets
 1  192.168.63.2 (192.168.63.2)  0.194 ms  0.163 ms  0.150 ms
 2  * * *
 3  * * *
 4  * * *
 5  * * *
 6  * * *
 7  * * *
 8  * * *
 9  * * *
10  * * *
11  a104-83-73-99.deploy.static.akamaitechnologies.com (104.83.73.99)  42.742 ms  42.666 ms  25.176 ms

```
> ⚠️ **Windows 命令 - `tracert`**
> ⚠️ **Linux 命令 - `traceroute`**

## <u>其他相關工具</u>

### **OSRFramework**

> ⚡︎ **OSRFramework 有一個[實踐實驗室](https://github.com/Samsar4/Ethical-Hacking-Labs/blob/master/1-Footprinting-and-Reconnaissance/4-OSRFramework.md)**


使用開源情報收集目標資訊。*(用戶名檢查、DNS 查詢、資訊洩漏研究、深度網絡搜索、正則表達式提取等)*。

### **網絡蜘蛛(Web Spiders)**
從網站獲取資訊，如頁面等。

### **[Recon-ng](https://github.com/lanmaster53/recon-ng)**

> ⚡︎ **Recon-ng 有一個[實踐實驗室](https://github.com/Samsar4/Ethical-Hacking-Labs/blob/master/1-Footprinting-and-Reconnaissance/3-Recon-ng.md)**

Recon-ng 是一個基於網絡的開源偵察工具，用於從目標組織及其人員中提取資訊。

提供了一個強大的環境，其中可以自動、快速、全面地進行開源網絡偵察。

### **[Metasploit Framework](https://github.com/rapid7/metasploit-framework)**

> ⚡︎ **Metasploit 有一個[實踐實驗室](https://github.com/Samsar4/Ethical-Hacking-Labs/blob/master/1-Footprinting-and-Reconnaissance/5-Metasploit-Basics.md)**

Metasploit 框架是一個提供有關安全漏洞的資訊並協助滲透測試和 IDS 簽名開發的工具；**這是一個龐大的框架，也提供 Recon 工具。**

### **[theHarvester](https://github.com/laramies/theHarvester)**

> ⚡︎ **theHarvester 有一個[實踐實驗室](https://github.com/Samsar4/Ethical-Hacking-Labs/blob/master/1-Footprinting-and-Reconnaissance/6-theHarvester.md)**


theHarvester 是一個 OSINT 工具；可用於收集以下資訊：
  - 電子郵件
  - 子域名
  - 主機
  - 員工姓名
  - 開放端口
  - 來自不同公共來源（如搜索引擎、PGP 密鑰服務器和 SHODAN 電腦數據庫）的橫幅廣告。

**使用示例**：
- **`theHarvester -d www.hackthissite.org -n -b  google`**
  - 發出 theHarvester 命令：`theHarvester`
  - 指定域名：`-d <url>`
  - 執行 DNS 查找：`-n`
  - 指定搜索引擎/來源：`-b google`


```
theHarvester -d www.hackthissite.org -n -b  google
table results already exists

*******************************************************************
*  _   _                                            _             *                                                                                        
* | |_| |__   ___    /\  /\__ _ _ ____   _____  ___| |_ ___ _ __  *                                                                                        
* | __|  _ \ / _ \  / /_/ / _` | '__\ \ / / _ \/ __| __/ _ \ '__| *                                                                                        
* | |_| | | |  __/ / __  / (_| | |   \ V /  __/\__ \ ||  __/ |    *                                                                                        
*  \__|_| |_|\___| \/ /_/ \__,_|_|    \_/ \___||___/\__\___|_|    *                                                                                        
*                                                                 *                                                                                        
* theHarvester 3.1.0                                         *                                                                                             
* Coded by Christian Martorella                                   *                                                                                        
* Edge-Security Research                                          *                                                                                        
* cmartorella@edge-security.com                                   *                                                                                        
*                                                                 *                                                                                        
*******************************************************************                                                                                        
                                                                                                                                                           
                                                                                                                                                           
[*] Target: www.hackthissite.org 
                                                                                                                                                           
[*] Searching Google. 
        Searching 0 results.
        Searching 100 results.
        Searching 200 results.
        Searching 300 results.
        Searching 400 results.
        Searching 500 results.

[*] No IPs found.

[*] Emails found: 2
----------------------
ab790c1315@www.hackthissite.org
staff@hackthissite.org

[*] Hosts found: 7
---------------------
0.loadbalancer.www.hackthissite.org:
22www.hackthissite.org:
2522www.hackthissite.org:
253dwww.hackthissite.org:
www.hackthissite.org:137.74.187.104, 137.74.187.100, 137.74.187.101, 137.74.187.103, 137.74.187.102
x22www.hackthissite.org:

[*] Starting active queries.
137.74.187.100
[*] Performing reverse lookup in 137.74.187.0/24
module 'theHarvester.discovery.dnssearch' has no attribute 'DnsReverse'
```

### **[Sublist3r](https://github.com/aboul3la/Sublist3r)**
Sublist3r **使用許多搜索引擎（如 Google、Yahoo、Bing、Baidu 和 Ask）列舉子域名**。Sublist3r 還使用 Netcraft、Virustotal、ThreatCrowd、DNSdumpster 和 ReverseDNS 列舉子域名

**使用示例**:
- **`python3 sublist3r.py -d hackthissite.org`**
  - Specify the domain: `-d <url>`
```
python3 sublist3r.py -d hackthissite.org

                 ____        _     _ _     _   _____    
                / ___| _   _| |__ | (_)___| |_|___ / _
                \___ \| | | | '_ \| | / __| __| |_ \| '__| 
                 ___) | |_| | |_) | | \__ \ |_ ___) | |  
                |____/ \__,_|_.__/|_|_|___/\__|____/|_| 
   
                # Coded By Ahmed Aboul-Ela - @aboul3la                                                                                              
                                                      
[-] Enumerating subdomains now for hackthissite.org                                                                                                        
[-] Searching now in Baidu..
[-] Searching now in Yahoo..
[-] Searching now in Google..
[-] Searching now in Bing..
[-] Searching now in Ask..
[-] Searching now in Netcraft..
[-] Searching now in DNSdumpster..
[-] Searching now in Virustotal..
[-] Searching now in ThreatCrowd..
[-] Searching now in SSL Certificates..
[-] Searching now in PassiveDNS..
[-] Total Unique Subdomains Found: 41
www.hackthissite.org
admin.hackthissite.org
api.hackthissite.org
ctf.hackthissite.org
vm-005.outbound.firewall.hackthissite.org
vm-050.outbound.firewall.hackthissite.org
vm-099.outbound.firewall.hackthissite.org
vm-150.outbound.firewall.hackthissite.org
vm-200.outbound.firewall.hackthissite.org
forum.hackthissite.org
forums.hackthissite.org
git.hackthissite.org
irc.hackthissite.org
(...)
```

### [DIRB](https://tools.kali.org/web-applications/dirb)
DIRB 是一個網絡內容掃描器。它尋找現有的（和/或隱藏的）Web 物件。它主要通過針對 Web 服務器發起基於字典的攻擊/暴力破解攻擊並分析響應來工作。
- 有助於在 Web 應用程序中找到子目錄

**使用示例**:
- **`dirb https://www.hackthissite.org/ /usr/share/wordlists/dirb/small.txt`**
  - Specify the url by issuing dirb command: `dirb <url>`(譯註:原文件寫`dib <url>`)
  - Specify the 字典檔位置: `/path/to/wordlist`

```
dirb https://www.hackthissite.org/ /usr/share/wordlists/dirb/small.txt 

-----------------
DIRB v2.22    
By The Dark Raver
-----------------

URL_BASE: https://www.hackthissite.org/
WORDLIST_FILES: /usr/share/wordlists/dirb/small.txt

-----------------

GENERATED WORDS: 959                                                           

---- Scanning URL: https://www.hackthissite.org/ ----
+ https://www.hackthissite.org/api (CODE:200|SIZE:10)                                                                                                     
+ https://www.hackthissite.org/blog (CODE:200|SIZE:20981)                                                                                                 
+ https://www.hackthissite.org/cgi-bin/ (CODE:403|SIZE:199)  
```

### Maltego

> ⚡︎ **Maltego 有[實踐實驗室](https://github.com/Samsar4/Ethical-Hacking-Labs/blob/master/1-Footprinting-and-Reconnaissance/2-Maltego-Basics.md)**

Maltego 是一個功能強大的 OSINT 工具，您可以通過網絡、技術和人員（電子郵件、電話號碼、推特）提取廣泛類型的資訊。

- 您可以：
  - 識別 IP 地址
  - 識別域和域名方案
  - 識別服務器端技術
  - 識別面向服務架構（SOA）資訊
  - 識別名稱服務器
  - 識別郵件交換器
  - 識別地理位置
  - 識別實體
  - 發現電子郵件地址和電話號碼

![alt text](https://gist.githubusercontent.com/Samsar4/62886aac358c3d484a0ec17e8eb11266/raw/6fe1dc406ed480aea2acfb2e9f34d51a0536e042/maltego-WebSite-IP-Location-WhoisOnDomain-5.png "IP Address, Location")


### 社交工程框架 (SEF, Social Engineering Framework)
這是一個開源的社交工程框架（腳本），可以幫助生成釣魚攻擊和偽造郵件。它包括釣魚頁面、偽造郵件、帶文件附件的偽造郵件以及其他有助於進行社交工程攻擊的材料。

![sef](https://hacknews247.com/wp-content/uploads/2018/10/20181002_212155_533793.png) (死圖)


## <u>基於網絡的偵查</u>

### **[NetCraft](https://www.netcraft.com/)**
Netcraft 是一個網站分析服務器，通過這個網站我們可以找到網站的基本和重要信息，例如：

- **背景** - 包括基本的域名信息。
  - 運行哪個操作系統、網絡服務器；哪個互聯網服務提供商；
- **網絡** - 包括從 IP 地址到域名到域名服務器的信息。
- **SSL/TLS** - 提供目標的 ssl/tls 狀態
- **托管歷史** - 提供目標托管歷史的信息
- **發件人政策框架 (SPF)** - 描述誰可以代表域名發送郵件
- **DMARC** - 這是一種機制，域名所有者可以指示聲稱來自其域的郵件如何進行身份驗證
- **網絡追踪器** - 這些追踪器可用於在整個網絡中監控單個用戶行為
網站技術 - 此部分包括以下詳細信息：
  - 雲端與 PaaS
  - 服務器端技術（例如：PHP）
  - 客戶端技術（例如：JavaScript 庫）
  - CDN 信息
  - CMS 信息（例如：WordPress，Joomla等）
  - 移動技術
  - 網絡統計（例如：網絡分析、收集等）
  - 字符編碼


![netcraft](https://i0.wp.com/hackingblogs.com/wp-content/uploads/2018/01/Capture-min-2.png) (死圖)

### **[Shodan](https://www.shodan.io/)**
*Shodan 與傳統的搜索引擎（如 Google）不同，它不使用網絡爬蟲遍歷整個網站，而是直接進入互聯網背後的通道，對各類型的端口設備進行審計，不斷尋找互聯網及其所有相關的**伺服器、攝像機、打印機、路由器等**。

- 有些人還將其描述為一個服務橫幅搜索引擎，這些橫幅是伺服器發送回客戶端的元數據。

- Shodan對基本的單詞搜索效果很好。以下是您可以使用的基本搜索過濾器：
  - **城市（city）**：查找位於某個特定城市的設備
  - **國家（country）**：查找位於某個特定國家的設備
  - **地理（geo）**：您可以傳遞坐標
  - **主機名（hostname）**：查找與主機名匹配的值
  - **網絡（net）**：基於 IP 或 /x CIDR 進行搜索
  - **操作系統（os）**：根據操作系統進行搜索
  - **端口（port）**：查找特定的開放端口
  - **before/after**：在某個時間範圍內查找結果


![shodan](https://logz.io/wp-content/uploads/2019/05/Shodan.png)
![shodan2](https://securityonline.info/wp-content/uploads/2017/10/shodan-1-615x1024.png)

### **[Censys](https://censys.io/overview/)**
*Alternative for Shodan.*

![censys](https://gist.githubusercontent.com/Samsar4/62886aac358c3d484a0ec17e8eb11266/raw/403be7a4514b6e0af36e0f568328372a5ce09cbf/censys.png)

