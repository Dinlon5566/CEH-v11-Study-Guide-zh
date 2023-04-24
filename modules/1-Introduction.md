# <u>簡介</u>

## <u> 基本安全概念 </u>
整個原則是通過**CIA 三位一體**（機密性，完整性和可用性）來避免系統的**竊取，篡改和破壞**。

<p align="center">
<img width="50%" src="https://i.ytimg.com/vi/AJTJN4wDBM8/hqdefault.jpg">
</p>

- **機密性 (Confidentiality)**
防止未經授權的人員訪問、查看、閱讀系統和數據。
信息只對授權人員可訪問。

- **完整性 (Integrity)**
數據或資源的可信賴性：保護數據免受未經授權方修改或刪除，並確保當授權人員進行不應該進行的更改時，可以撤銷造成的損害。

- **可用性 (Availability)**
當授權用戶需要時可訪問：系統、訪問通道和身份驗證機制必須正常運行，以便在需要時提供和保護它們提供的信息。

- **真實性 (Authenticity)**
指通信、文件或任何數據的特性，確保其真實性。

**注意：** *此外，其他屬性（如真實性、問責性、不可否認性和可靠性）也可能涉及（ISO/IEC 27000:2009）。*

- **審計與問責 (Auditing & Accountability)**
基本上跟踪所有事物，例如，誰在何時登錄，誰在訪問這些數據。

- **不可否認性 (Non-Repudiation)**
不可否認性是確保某人不能否認某事物有效性的保證。不可否認性是一個法律概念，廣泛用於信息安全，指的是提供數據來源和數據完整性證明的服務。

### **安全性、功能性和可用性之間的平衡**

這三個属性之間存在相互依赖。當**安全性提高時，可用性和功能性降低**。任何組織應在這三個品質之間取得平衡，以實現平衡的信息系統。

<p align="center">
<img width="50%" src="https://gist.githubusercontent.com/Samsar4/62886aac358c3d484a0ec17e8eb11266/raw/f14455ed4def635e1bc93b85657f43dbbf4a3127/triad2.png">
</p>

## <u>黑客類型</u>

<p align="center">
<img width="50%" src="https://www.simplilearn.com/ice9/free_resources_article_thumb/types-hacker.JPG">
</p>

> - **黑帽 (Black Hat)** - 尋求執行惡意活動的黑客。
> - **灰帽 (Gray Hat)** - 執行好的或壞的活動的黑客，但未獲得其所攻擊的組織的許可。
> - **白帽 (White Hat)** - 合法黑客；他們利用自己的技能通過在惡意黑客之前暴露漏洞來提高安全性。

**腳本小子/菜鳥 (Script Kiddie / Skiddies)** - 使用他人開發的惡意腳本或程序（例如 Web Shell）攻擊計算機系統和網絡，破壞網站的無技術人員。

**國家資助的黑客 (State-Sponsored Hacker)** - 受政府或相關實體雇傭的黑客。

**駭客活動家 (Hacktivist)** - 為某一事業而黑客；政治議程。

**自殺型黑客 (Suicide Hackers)** - 是不怕去監獄或面對任何形式懲罰的黑客；為完成任務而駭客。

**網絡恐怖分子 (Cyberterrorist)** - 受宗教或政治信仰驅使，制造恐懼或破壞性。

## <u>駭客術語</u>

- **駭客價值 (Hack value)** - 攻擊者眼中目標的感知價值或價值。
- **漏洞 (Vulnerability)** - 系統缺陷，系統上的弱點（在設計、實現等方面）。
- **威脅 (Threat)** - 利用漏洞。
- **漏洞利用 (Exploit)** - 漏洞利用是通過安全漏洞獲取系統訪問權限並利用漏洞謀取利益的一種方法。
- **有效負載 (Payload)** - 攻擊的組件；它是私人用戶文本的一部分，可能還包含諸如蠕蟲或病毒之類的惡意軟件，用於執行惡意操作；刪除數據、發送垃圾郵件或加密數據。
- **零日攻擊 (Zero-day attack)** - 在供應商知道或能夠修補漏洞之前發生的攻擊。
- **雛菊鏈 / 轉向 (Daisy Chaining / Pivotting)** - 它涉及獲取訪問網絡和/或計算機的權限，然後使用相同的信息獲取包含所需信息的多個網絡和計算機的訪問權限。
- **曝光私隱 (Doxxing)** - 通常出於惡意目的，公開有關個人的個人身份信息。
- **企業信息安全架構 (Enterprise Information Security Architecture, EISA)** - 通過過程、要求、原則和模型確定組織信息系統的結構和行為。

## <u> 威脅類別 </u>
* **網絡威脅 (Network Threats)**
  - 信息收集
  - 嗅探和竊聽
  - DNS/ARP中毒
  - MITM (中間人攻擊)
  - DoS/DDoS
  - 基於密碼的攻擊
  - 防火牆和IDS攻擊
  - 會話劫持

* **主機威脅 (Host Threats)**
  - 密碼破解
  - 惡意軟件攻擊
  - 足跡
  - 配置文件
  - 任意代碼執行
  - 背門訪問
  - 權限提升
  - 代碼執行

* **應用程序威脅 (Application Threats)**
  - 注入攻擊
  - 不正確的數據/輸入驗證
  - 不正確的錯誤處理和異常管理
  - 隱藏字段操縱
  - 破碎的會話管理
  - 密碼學問題
  - SQL注入
  - 網絡釣魚
  - 緩衝區溢出
  - 信息披露
  - 安全配置不當

## <u> 攻擊向量 </u>
*通過攻擊向量，駭客可以訪問主機，以便傳遞有效負載或惡意結果*

- **APT - 高級持續性威脅 (Advanced Persistent Threats)**
  - 高級持續性威脅是一個隱蔽的威脅行為者，通常是國家或國家支持的團體，它在未經授權的情況下訪問計算機網絡並在很長一段時間內未被檢測到；通常使用零日攻擊。
- **雲計算 / 雲技術 (Cloud computing / Cloud-based technologies)**
  - 一個客戶端應用程序雲中的漏洞可能允許攻擊者訪問其他客戶端的數據
- **病毒，蠕蟲和惡意軟件 (Viruses, worms, and malware)**
  - 病毒和蠕蟲是最普遍的網絡威脅，它們能在幾秒鐘內感染網絡。
- **勒索軟件 (Ransomware)**
  - 限制對計算機系統文件和文件夾的訪問，並要求向攻擊者支付網絡贖金以解除限制。
- **移動設備威脅 (Mobile Device threats)**
- **僵屍網絡 (Botnets)**
  - 由入侵者使用的大量受感染系統組成的網絡，用於執行各種網絡攻擊
- **內部攻擊 (Insider attacks)**
    - 不滿的員工可以從內部損壞資產。
    - 大量受感染的主機網絡。(用於DDoS攻擊)。

- **網絡釣魚攻擊 (Phishing attacks)**
- **Web應用程序威脅 (Web Application Threats)**
  - 包括SQL注入、XSS（跨站腳本攻擊）等攻擊。
- **物聯網威脅 (IoT Threats)**


## <u>攻擊類型</u>
### 1. 操作系統
*針對操作系統漏洞或內部的安全問題進行攻擊，例如訪客賬戶或默認密碼。*
>  - **向量**: 緩衝區溢出，協議實現，軟件缺陷，補丁級別，身份驗證方案

### 2. 應用程序層次
*針對編程代碼和軟件邏輯的攻擊。*
>  - **向量**: 緩衝區溢出，漏洞，XSS，DoS，SQL注入，MITM

### 3. 錯誤配置
*攻擊利用了由於不正確配置或默認配置而配置錯誤的系統。*

>  - **示例**: SQL用戶的不當權限；訪問列表允許所有(permit all)

### 4. 縮放包裝代碼
*利用未打補丁或配置不當的軟件中的漏洞。*
>  - **示例**: 軟件1.0版本中的缺陷；CGI腳本示例中的缺陷；默認密碼

## <u>漏洞</u>

- **CVSS - 通用漏洞評分系統** [[+]](https://nvd.nist.gov/vuln-metrics/cvss)
  - 根據嚴重程度給出數值評分
  - ![cvss](https://3.bp.blogspot.com/-5V1cb_wTvsk/Wl78iF4Sd8I/AAAAAAAAF7U/KmK4pMXi54YworDgh4uI8aZtHgy0bbznQCLcBGAs/s1600/CVSS.png
  )
- **CVE – 通用漏洞和披露** [[+]](https://cve.mitre.org/)
  - 由MITRE維護的公開披露漏洞和披露列表。
  - ![cve](https://i0.wp.com/gbhackers.com/wp-content/uploads/2016/10/cve.png?resize=486%2C408&ssl=1)
- **NVD - 國家漏洞數據庫**  [[+]](https://nvd.nist.gov/)
  - 由NIST維護的數據庫，與MITRE CVE列表完全同步；美國政府漏洞存儲庫。

### 漏洞類別

- **錯誤配置** - 不正確地配置服務或應用程序
- **默認安裝** - 未更改默認情況下附帶的應用程序設置
- **緩衝區溢出** - 代碼執行漏洞
- **缺失補丁** - 未打補丁的系統
- **設計缺陷** - 系統設計中固有的缺陷，如加密和數據驗證
- **操作系統漏洞** - 特定於每個操作系統的漏洞
- **默認密碼** - 保留系統/應用程序附帶的默認密碼


## <u>滲透測試階段 (CEH)</u>
1. **攻擊前階段** - 偵查和收集數據。
2. **攻擊階段** - 嘗試穿透網路並執行攻擊。
3. **攻擊後階段** - 清理以將系統恢復到攻擊前狀態並提交報告。

> ⚠️ 對於考試，EC-Council 提供了他們自己的方法，這就是您需要的所有考試內容；如果您有興趣，可以在[這裡](https://owasp.org/www-project-web-security-testing-guide/latest/3-The_OWASP_Testing_Framework/1-Penetration_Testing_Methodologies)查看其他滲透測試方法；如果您正在學習成為一名專業的滲透測試者，除了認證內容之外，我建議使用 [OSSTMM](https://www.isecom.org/research.html)（開源安全測試方法手冊）。

## <u>五個道德駭客階段</u>

### 1. **偵查 (Reconnaissance)**
*收集有關不標的證據*；偵查有兩種類型：
- **被動偵查 (Passive Reconnaissance)**：在**不直接與系統交互**的情況下，獲取有關目標計算機和網絡的信息。
    - 例如：Google 搜索、公共記錄、新版本、社交媒體、Wardrive 掃描周圍的網路。
- **主動偵查 (Active Reconnaissance)**：涉及與目標直接互動。
    - 例如：給目標打電話、面試；可以將 Nmap、Nessus、OpenVAS、Nikto 和 Metasploit 等工具視為主動偵查。

### 2. **掃描和枚舉 (Scanning & Enumeration)**
*獲取有關目標的更深入信息。*
- 例如：網絡掃描、端口掃描、正在運行的服務版本。

### 3. **獲取訪問權限 (Gaining Access)**
*為了獲得系統訪問權限而發起攻擊。*
- 例如：可以在本地（離線）、局域網或互聯網上完成。
  - 例如(2)：偽裝以偽裝成合法用戶或不同系統的方式利用系統，他們可以向目標系統發送包含漏洞的數據包以利用漏洞。
  - 可以使用許多技術，例如命令注入、緩衝區溢出、DoS、暴力破解憑證、社交工程、配置錯誤等。

### 4. **維持訪問權限 (Maintaining Access)**
*實施措施以確保未來的訪問。*
- 例如：可以使用Rookit、特洛伊木馬、後門等。

### 5. **掩蓋痕跡 (Covering Tracks)**
*採取措施隱瞞成功和入侵行為；不被注意到。*
  - 例如：清除日誌；混淆特洛伊木馬或惡意後門程序。


## 三種類型的主動防禦
- **惱人（Annoyance）**
  - 涉及追踪駭客並將其引入偽造的伺服器，浪費其時間，並使其容易被檢測。
- **歸屬（Attribution）**
  - 識別攻擊者；使用工具將攻擊的源追溯到特定位置，甚至是個別駭客。
- **攻擊（Attack）**
  - 這是最具爭議性的。要進行“反駭”，公司會訪問涉嫌駭客的計算機以刪除其數據，甚至進行報復。這兩個步驟都被認為是非法的。

## <u>資訊保證 (IA, Information Assurance) </u>
*指在使用、處理、存儲和傳輸資訊過程中，確保資訊和資訊系統的完整性、可用性、保密性和真實性。*

* **有助於實現 IA 的流程：**
  - 制定本地政策、流程和指南。
  - 設計網絡和用戶認證策略。
  - 識別網絡漏洞和威脅（漏洞評估概述網絡的安全狀態）。
  - 識別問題和資源需求。
  - 為確定的資源需求制定計劃。
  - 應用適當的 IA 控制。
  - 對資訊系統執行 C&A（認證與授權）過程有助於追踪漏洞並實施安全措施。
  - 向聯邦和私營組織的所有人員提供資訊保證培訓。

## <u>資訊安全管理計劃 (Information Security Management Program) </u>
*政策、流程、程序、標準和指南的組合，旨在確立所需的**資訊安全水平**。*

- 旨在確保業務在降低風險的狀態下運行。
- 涵蓋了與資訊安全相關的所有組織和運營流程及參與者。

![infosec](https://gist.githubusercontent.com/Samsar4/62886aac358c3d484a0ec17e8eb11266/raw/950220d4b802bb726fe84470c7a13055b056a621/infosec.jpg)


> ⚠️ **IA** 專注於風險評估、緩解方面；  
> ⚠️ **資訊安全 (InfoSec)** 專注於實際實施安全措施以保護系統。

## <u>企業資訊安全架構 (EISA, Enterprise Information Security Architecture) </u>
*確定組織資訊系統結構和行為的要求、流程、原則和模型。*

* **EISA 的目標**：
  - 有助於監控和檢測網絡行為
  - 檢測並恢復安全漏洞
  - 組織資源的優先排序
  - 有助於對組織的 IT 資產進行風險評估
  - 在安全條款（如事件響應、災難恢復、事件關聯等）中納入成本考慮。

## <u>實體安全控制 (Physical Security Controls)</u> 

- **預防控制（Preventive control）**：阻止行為者執行威脅。
    - 例如：圍欄、伺服器鎖(Server lock)、防盜門等。

- **偵查控制（Detective control）**：識別行為者的威脅。
    - 例如：背景審查、閉路電視（CCTV）。

- **威懾控制（Deterrent control）**：阻止行為者**嘗試**威脅。
    - 例如：警告標誌。

- **恢復（Recovery）**：減輕已顯現威脅的影響。
    - 例如：備份。

- **補償控制（Compensating control）**：為上述任何功能提供替代解決方案。


*大部分的安全控制都是預防性階段控制*。

⚠️ **深度防禦（Defense in Depth）**：多層安全控制；在控制失效時提供冗餘。（例如：下面的圖片）

![defense-in-depth](https://www.fairwarning.com/wp-content/uploads/2019/03/Defense-in-Depth-for-Cloud-Security-Rainbow-Diagram.png)
(原圖死了)

### 安全控制類型

| 描述          | 示例                                      |
| ----------- | ---------------------------------------- |
| **實體**      | 警衛、燈光、攝像頭、滅火器、防洪設施                        |
| **管理**      | 信息安全培訓意識、政策、程序和指南                     |
| **技術**      | 入侵檢測/防禦系統（IDS/IPS）、防火牆、加密、智能卡、訪問控制列表 |

| 描述         | 示例                     |
| ---------- | ---------------------- |
| **預防性**     | 認證、警報鈴                |
| **偵查性**     | 審計、備份                 |
| **糾正性**     | 恢復操作                  |

## <u>風險管理 (Managing the Risk)</u>
**風險**可以定義為內部或外部負債可能損害、造成損失或產生其他負面影響的威脅或事件的發生概率。

### 風險矩陣

**風險矩陣**在**風險評估**期間用於通過考慮**概率或可能性**類別與**嚴重性**後果類別來確定風險等級。

- 這是一個簡單的機制，用於提高風險的可見性，並協助管理決策。

![matrix](https://paladinrisk.com.au/wp-content/uploads/2018/11/risk-1-1024x434.jpg)

### 風險管理
*是對風險的識別、評估和優先排序，然後協調和經濟地應用資源以最小化、監控和控制不幸事件的概率或影響，或最大化機會的實現。*

### 風險管理階段

<p align="center">
<img width="60%" src="http://informeanual.abengoa.com/export/sites/abengoa_ia/2010/resources/images/responsabilidad_social/C12ING/12.6.jpg" />
</p>

- **風險識別**
  - 識別內部和外部風險的來源、原因和後果。
- **風險評估**
  - 評估組織風險並提供風險可能性和影響的估計
- **風險處理**
  - 選擇並實施對已識別風險的適當控制
- **風險追踪**
  - 確保實施適當的控制來處理風險並識別新風險的可能性
- **風險審查**
  - 評估實施的風險管理策略的績效

### 威脅建模
這是一種風險評估方法，用於通過捕獲、組織和分析影響應用程序安全性的所有信息來分析應用程序的安全性。

1. 確定目標
    - 有助於確定後續步驟需要投入多少努力
2. 應用程序概述
    - **識別組件**、數據流和信任邊界
3. 分解應用程序
    - 找到**更多與威脅相關的詳細信息**
4. 識別威脅
    - 使用第2和3步獲得的信息，識別與您的控制場景和上下文相關的威脅
5. 識別漏洞
    - 使用漏洞類別**識別與所發現威脅相關的弱點**

## <u>安全政策 (Security Policies)</u>
1. **政策** - 關於保護資訊的高層次陳述；保護 CIA 三原則的業務規則；安全政策可以應用於用戶、系統、合作夥伴、網絡和提供商。
    - **常見安全政策範例：**
      - 密碼政策 (Password Policy)
        - 符合密碼複雜度要求。
        - 例如：最少 8 個字符長度，大小寫和字母數字混合。
      - 無線安全政策 (Wireless Security Policy)
      - AUP - 可接受使用政策 (Acceptable Use-Policy)
        - 如何合適地使用公司資產
        - 例如：公司電腦的 "應做和不應做"。
      - 數據保留政策 (Data Retention Policy)
        - 例如：保留數據 X 時間。
      - 訪問控制政策 (Access Control Policies)
        - 例如：訪問服務器；防火牆
2. **程序** - 實現目標的一組詳細步驟；實施指南 
3. **指南** - 針對給定情況的行動建議；推薦，非強制性 

## 安全政策 - 示例
* **訪問控制政策 (Access Control Policy)**
  - 這確定了被保護的資源以及控制訪問它們的規則。

* **遠程訪問政策 (Remote Access Policy)**
  - 這確定了誰可以進行遠程訪問，並確定了訪問媒介和遠程訪問安全控制。

* **防火牆管理政策 (Firewall Management Policy)**
  - 這確定了組織中防火牆的訪問、管理和監控。

* **網絡連接政策 (Network Connection Policy)**
  - 這確定了誰可以在網絡上安裝新資源，批准新設備的安裝，記錄網絡變更等。

* **密碼政策 (Password Policy)**
  - 這確定了在可用資源上使用強密碼保護的指南。

* **用戶帳戶政策 (User Account Policy)**
  - 這確定了帳戶創建流程、權限、權利和用戶帳戶的責任。

* **資訊保護政策 (Information Protection Policy)
  - 這確定了資訊的敏感程度，誰可以訪問，以及如何存儲和傳輸，以及如何從存儲媒體中刪除等。

* **特殊訪問政策 (Special Access Policy)**
  - 這確定了授予系統資源特殊訪問的條款和條件。

* **電子郵件安全政策 (Email Security Policy)**
  - 這項政策旨在規範企業電子郵件的正確使用。

* **可接受使用政策 (Acceptable Use Policy)**
  - 這確定了系統資源的可接受使用。

## 安全政策 - 類型
1. **放任政策 (Promiscuous Policy)** - 這種政策通常對系統資源的使用沒有限制。

2. **寬容政策 (Permissive Policy)** - 這種政策從寬開始，只有已知的危險服務/攻擊或行為被阻止。這類政策必須定期更新以保持有效。

3. **謹慎政策 (Prudent Policy)** - 這種政策在允許已知但必要的危險時提供最大安全性。這類政策將阻止所有服務，只有安全/必要的服務逐個啟用。所有操作都被記錄。

4. **偏執政策 (Paranoid Policy)** - 這種政策禁止一切。不允許使用互聯網連接或嚴格限制互聯網使用。

## 安全政策 - 創建步驟
1. 進行風險評估
2. 使用安全標準和框架作為指導
3. 徵求管理層和員工意見
4. 實施政策。對不遵守的行為進行處罰
5. 向整個組織發布最終草案
6. 讓所有員工閱讀/簽署他們理解的政策
7. 使用工具來幫助實施政策
8. 員工培訓
9. 定期審查和更新

## <u>事件管理流程 (Incident Management Process) </u>
*事件是可能導致組織業務、服務或功能損失或中斷的事件。*

***事件管理（Incident management）**是描述組織確定、分析並糾正風險的活動，以防止未來再次發生的術語。*

1. **準備（Preparation）：** 選擇人員，分配規則，確定處理事件的工具。
2. **檢測與分析（Detection & Analysis）：** 確定事件已發生（IDS, SIEM, AV, 有人報告等）。
3. **分類和優先排序（Classification and Prioritization）：**
4. **通知（Notification）：** 識別輕微和重大事件；如何通知事件。
5. **隔離（Containment）：** 限制損害；隔離主機；聯繫系統所有者。
6. **取證調查（Forensic Investigation）：** 使用取證工具調查事件的根本原因；系統日誌、實時內存、網絡設備日誌、應用日誌等；
7. **根除和恢復（Eradicate & Recovery）：** 消除事件原因；如有需要，打補丁。恢復：恢復生產；監控受影響的系統。
8. **事後活動（Post-incident Activities）：** 記錄事件發生的原因及過程；傳授知識。

### 事件應對小組職責 (Incident Response Team Duties)

1. 通過對客戶安全漏洞採取主動方法來管理安全問題
2. 制定或審查必須遵循的流程和程序
3. 管理對事件的應對，確保所有程序正確執行，以最小化和控制損害
4. 確定和分析事件發生期間的情況，包括影響和威脅
5. 為報告安全事件和問題提供單一聯繫點
6. 審查法律和監管要求的變化，以確保所有流程和程序有效
7. 審查現有控制措施，並推薦防止未來事件發生的步驟和技術
8. 與地方執法機構、政府機構、主要合作夥伴和供應商建立關係

### SIEM -安全資訊和事件管理 (SIEM - Security Information and Event Management)
<p align="center">
<img width="90%" src="https://secureops.com/wp-content/uploads/2020/01/components-of-siem.jpg" />
</p>

*從網絡中收集數據點，包括來自每個主機的日誌文件、流量捕獲、SNMP 消息等。SIEM 可以將所有數據收集到一個集中位置，並將其相關聯以分析，以實時查找安全和性能問題以及負面趨勢。*

* **聚合（Aggregation）：** 從不同來源收集數據並將數據組織成單一格式。SIEM 系統中的任何收集數據的設備都稱為收集器或聚合器。

* **關聯（Correlation）：** 查看來自不同來源的數據，並可以判定在您的網絡上發生的事件。（根據 NIDS/NIPS 的放置方式，可能是內聯或外聯）。
	* **警報（Alerts）** - 如果出現問題，用於通知。
	* **觸發（Triggering）** - 超過閾值。

* **標準化（Normalization）：** 實際上將創建多個表/組織數據，使數據變得更有效，並允許我們的分析和報告工具更好地運行。

* **WORM - Write Once Read Many：** 其概念是日誌文件非常寶貴，很多時候您可能希望以存檔方式查看它們，因此可以使用光盤驅動器等 WORM 驅動器將它們存儲起來。

#### 常見 SIEM Tools: 

* **[Splunk](https://www.splunk.com/)**
	![splunk](https://www.splunk.com/content/dam/splunk2/images/screenshots/platform-journey/conflaunch/SS-UI-Light-Mode-frame.png)

<br>

* **[ArcSight](https://www.microfocus.com/en-us/products/siem-security-information-event-management/overview)**
	![arcsight](https://i.ytimg.com/vi/N7J0EwdbKF0/maxresdefault.jpg)

<br>

* **[ELK - Elastic Search, Log Stash and Kibana](https://www.elastic.co/what-is/elk-stack) (Open Source)**
	![elk](https://i.imgur.com/lydtCwn.png)

## <u>身份和訪問管理</u>
> **身份識別、身份驗證、授權** 和 **記賬** 一起協同工作，以安全地管理資產。

### 1. **身份識別（Identification）**
*憑證上的信息用於識別用戶。*

- **例子**：
  - 你的名字、用戶名、ID 號、員工號、社會安全號等。

### 2. **身份驗證（Authentication）**
*“證明你是合法用戶"。- 應始終使用多因素身份驗證！*

* **身份驗證因素：**
	* 你**知道**的東西（例如 - 密碼）
	* 你**擁有**的東西（例如 - 智能卡）
	* 你**是**什麼（例如 - 指紋）
	* 你**做**的事情（例如 - 安卓圖案；手寫簽名）
	* 你**在哪裡**（例如 - 地理位置）
> 🛑 **多因素身份驗證** *通常使用兩個示例（例如 - 你**知道的東西(1)** 和 你**擁有的東西(2)**，永遠不要在同一類別中）*

### 3. 授權概念

*你被允許訪問什麼 - 我們使用訪問控制模型，我們實現什麼以及如何實現取決於組織以及我們的安全目標。*
* **權限（Permissions）**：
	* 應用於資源
* **權利** / **特權（Rights/Privileges）**：
	* 在系統級別分配
* **授權策略**：
	* 最小特權
	* 職責分離

### 4. 記賬（Accounting）
*將操作追溯到主體身份：*
- 證明特定操作是由誰/什麼執行的（不可抵賴性）；日誌記錄

### 存取控制模型

<p align="center">
<img width="80%" src="https://security-architect.com/wp-content/uploads/FGA.png" />
</p>

* **強制性存取控制 (MAC, Mandatory Access Control)**：
	* 每個對象都會被分配一個**標籤**
		- 保密、機密、絕密等
	* 管理員決定誰可以訪問哪個安全等級；用戶無法更改這些設置
	* 用於舊系統（例如，絕密政府信息）
* **自主存取控制 (DAC, Discretionary Access Control)**：
	* 用於大多數操作系統
	* 數據擁有者定義訪問權限
	* 非常靈活的存取控制；安全性非常薄弱
* **基於角色的存取控制 (RBAC, Role-based Access Control)**：
	* 訪問資源是根據您在組織/職能中的角色所定義的一組規則（經理、主管等）
	* 管理員根據用戶的角色提供訪問權限
		- 權限是隱式獲得而非顯式獲得
	* 在 Windows 中，使用**組**提供基於角色的存取控制
		- 例如：管理組 --> 權限和許可權，
		- 銷售組 --> 權限和許可權


> ⚠️ **訪問權限由 ACL (Access Control List, 存取控制列表) 定義。**
> ⚠️ **隱式拒絕** 除非特別允許，否則阻止訪問。


## 數據損失預防 (DLP, Data Loss Prevention)
數據損失預防（DLP）是指**檢測和防止數據泄露、數據外泄或對敏感數據的非計劃性破壞**的實踐。組織使用 DLP 來保護和保障其數據並遵守法規。

* DLP 一詞指的是防止組織數據損失和數據外泄的措施。

#### 組織通常使用 DLP 來：

- 保護個人身份信息（PII）並遵守相關法規
- 保護對組織至關重要的知識產權
- 在大型組織中實現數據可見性
- 保護移動勞動力，並在 Bring Your Own Device（BYOD）環境中實施安全措施
- 保護遠程雲系統上的數據

<p align="center">
<img width="90%" src="https://miro.medium.com/max/720/1*FG9LR51eySVRQJUjhVv-9A.png" />
</p>

## 數據備份
數據備份在維護業務連續性方面發揮著關鍵作用，幫助組織從 IT 災難、安全漏洞、應用程序失敗、人為錯誤等中恢復。

所有法規遵從性要求，如 COBIT、SSAE、SOCII、PCI-DSS、HIPPA、SOX、FINRA、FISMA、GDPR 等，都要求企業在指定期限內保留關鍵數據的數據備份。

### 備份策略
1. 識別關鍵業務數據
2. 選擇備份媒介
3. 選擇備份技術
4. 選擇合適的 RAID 等級
5. 選擇適當的備份方法

### 3種備份方法
#### 1. 冷備份 🔵

<img width="40%" src="https://gist.githubusercontent.com/Samsar4/62886aac358c3d484a0ec17e8eb11266/raw/29c5e018095b135baec32aaece84a900a43b23ca/cc-cold.png"/>

- **空站點，無硬件，無數據，無人員**
- **需要幾周才能上線**
- 基本辦公空間（如建築、椅子、空調等）
- 沒有運營設備
- 最便宜的恢復站點

#### 2. 暖備份 🟡

<img width="40%" src="https://gist.githubusercontent.com/Samsar4/62886aac358c3d484a0ec17e8eb11266/raw/29c5e018095b135baec32aaece84a900a43b23ca/cc-warm.png"/>

- **介於冷備份和熱備份之間 - 剛好可以運行（有機架空間的大房間，您帶來硬件）**
- 硬件已經準備好，等待您帶來軟件和數據
- **需要幾天才能上線**
- 有運營設備，但數據很少或根本沒有

#### 3. 熱備份 🔴

<img width="40%" src="https://gist.githubusercontent.com/Samsar4/62886aac358c3d484a0ec17e8eb11266/raw/29c5e018095b135baec32aaece84a900a43b23ca/cc-hot.png"/>

- **生產系統的精確副本**
- 應用程序和軟件不斷更新
- 按下開關，一切都在運行
- **需要幾個小時才能上線**
- 實時同步
- 幾乎所有數據都已準備好，通常只需快速更新
- 成本非常高


## <u>滲透測試 - 基礎知識</u>
> **這個主題將在[第14章 - 滲透測試](https://github.com/Samsar4/CEH-v10-Study-Guide/blob/master/modules/14-Pentesting.md)中詳細介紹。**

*滲透測試，口語上稱為 pen test、pentest 或道德黑客，是對計算機系統進行授權的模擬網絡攻擊，以評估系統的安全性。*

> ⚠️ **不要與漏洞評估混淆。**

- 清晰定義的全面安全控制測試
- 階段
  - **準備** - 確定合同和團隊
  - **評估** - 所有黑客階段（侦察，掃描，攻擊等）
  - **後評估** - 報告和結論
- 類型
  - **黑盒** - 在對系統或網絡一無所知的情況下進行。
  - **白盒** - 當攻擊者擁有由所有者/目標提供的系統的完整知識。
  - **灰盒** - 當攻擊者對系統和/或網絡有一定了解

## <u>法律類別</u>

- **刑事** - 保護公共安全的法律，通常附有監禁時間。
- **民事** - 私人權利和救濟。
- **普通** - 基於社會習俗的法律。

## 法律和標准：

### **OSSTM 合規性**
**"開源安全測試方法手冊 (Open Source Security Testing Methodology Manual)"** 由 ISECOM 維護，定義了三種類型的合規性。

- **立法** - 處理政府法規（如 SOX 和 HIPAA）。
- **合同** - 處理行業/團體要求（如 PCI DSS）。
- **基於標准** - 處理由特定團體/組織成員必須遵循的實踐（如 ITIL，ISO 和 OSSTMM 本身）。

- **OSSTM 控制**
  - **OSSTM 類別 A - 交互控制**
    - *身份驗證* - 根據憑證提供身份識別和授權。
    - *賠償* - 提供合同保護，防止損失或損害。
    - *征服* - 確保交互按資產所有者定義的流程進行。
    - *連續性* - 當資產遭受破壞或故障時，保持與資產的交互。
    - *恢復力* - 保護資產免受破壞和故障。

- **OSSTM 類別 B - 過程控制**
    - *不可否認性* - 防止參與者否認其行為
    - *保密性* - 確保只有參與者知道資產
    - *隱私* - 確保只有參與者可以訪問資產
    - *完整性* - 確保只有參與者在資產和過程發生變化時知道
    - *警報* - 當交互發生時通知參與者

### **PCI-DSS**
**"支付卡行業數據安全標準 (Payment Card Industry Data Security Standard)"** 適用於處理信用卡、ATM 卡和其他 POS 卡的組織的標準。

### **ISO 27001**
本國際標準旨在為建立、實施、維護和不斷改進信息安全管理系統提供要求。

### **ISO 27002 和 17799**
基於 BS799，但重點關注安全目標，並根據行業最佳實踐提供安全控制。

### **HIPAA**
**"健康保險搬遷和問責法 (Health Insurance Portability and Accountability Act)"** 一項法律，為保護病人醫療記錄和在醫生、醫院和保險公司之間共享的健康信息制定隱私標準。

### **SOX**
**"Sarbanes-Oxley 法案"** 要求上市公司接受獨立審計並適當披露財務信息的法律。

### DMCA
**"數字千禧年版權法案 (The Digital Millennium Copyright Act)"** 是一項 1998 年美國版權法，該法實施了世界知識產權組織的兩項 1996 年條約。它將生產和傳播技術、設備或服務視為犯罪，這些技術、設備或服務旨在繞過控制版權作品的訪問措施。

### **FISMA**
**"2002 年聯邦信息安全現代化法案 (Federal Information Security Modernization Ac Of 2002)"** 一項法律，於 2004 年更新，以確定國土安全部在實施信息安全政策方面的權限。*(適用於政府機構)*

### **NIST-800-53**
為聯邦信息系統編制的安全和隱私控制目錄，旨在幫助實施 FISMA。
  
### **FITARA**
**"聯邦信息技術采購改革法案 (Federal Information Technology Acquisition Reform Act)"** 一項 2013 年的法案，旨在改變確定美國政府如何購買技術的框架。

### **COBIT**
**"信息和相關技術控制目標 (Control Object for Information and Related Technology)"** IT 治理框架和工具集，由 ISACA 和 ITGI 創建。

### **GLBA**
**"美國格拉姆-里奇-布莱利法案 (U.S Gramm-Leach-Bliley Act)"** 一項法律，旨在保護金融機構收集的個人信息的保密性和完整性。

### **CSIRT**
**"計算機安全事故響應小組 (Computer Security Incident Response Team)"** CSIRT 在報告計算機安全事故時提供單一聯繫點。

### **ITIL**
**"信息技術基礎架構圖書館 (Information Technology Infrastructure Library)"** - 一個在 20 世紀 80 年代開發的運營框架，將 IT 管理程序標準化。

# <u>基本知識</u>

## <u> OSI 模型和 TCP 模型</u>
- **我們剛剛研究的 OSI 模型** 只是一個參考/邏輯模型。它被設計為通過將通信過程劃分為更小且更簡單的組件來描述通信系統的功能。

- **TCP/IP 模型** 是 OSI 模型的簡化版本。它包含四個層次，而 OSI 模型中有七個層次。

| 層次 | 設備類型 | OSI 層 | TCP/IP 模型 | TCP/IP 新 (實際) | 協議 | PDU
--|--|--|--|--|--|--
7 | 網關 | **應用層 (Application)** | 應用層 | 應用層 | HTTP, FTP, POP, SMTP, DNS, RIP | 數據
6 | -       | **表示層 (Presentation)**| 應用層 | 應用層 | HTTP, FTP, POP, SMTP, DNS, RIP, MIME | 數據
5 | -       | **會話層 (Session)**     | 應用層 | 應用層 | HTTP, FTP, POP, SMTP, DNS, RIP, SCP | 數據
4 | -       | **傳輸層 (Transport)**   | 傳輸層  | 傳輸層 | TCP/UDP | 段
3 | 路由器  | **網絡層 (Network)**     | 互聯網   | 網絡層 | IP, ARP, ICMP, IGMP | 封包
2 | 交換機/橋 | **數據鏈路層 (Data Link)** | 鏈路   | 數據鏈路層 | 以太網, 令牌環 | Frames
1| 集線器/中繼器 | **物理層 (Physical)**  | 鏈路   | 物理層 | 以太網, 令牌環 | Bits

### <u>TCP 握手 (TCP Handshake)</u>

<h4 align="center">三次握手 (The Three-way handshake)</h4>
<p align="center">
<img width="77%" src="https://wiki.mikrotik.com/images/f/fc/Image2001.gif">
</p>

#### ✅ TCP 連接建立過程
1. **主機 A** 向主機 B 發送具有建議的初始序列號的 **SYN** (synchronize) 數據包。
2. **主機 B** 收到 **SYN** 消息後，返回一個在 [TCP 頭](https://www.gatevidyalay.com/transmission-control-protocol-tcp-header/) 中設置了 SYN 和 ACK 標誌（**SYN-ACK**）的數據包。
3. **主機 A** 收到 **SYN-ACK**，然後發送 **ACK**（確認）數據包。
4. **主機 B** 收到 **ACK**，此時連接被 **建立**。

#### ❌ TCP 連接終止
1. **主機 A** 發送一個 **FIN**（完成）標誌，表示它已完成數據發送。
2. 收到 **FIN** 的 **主機 B** 不終止連接，而是進入“被動關閉”（CLOSE_WAIT）狀態，並將 **FIN** 的 **ACK** 發送回主機 A。
3. **主機 A** 進入（TIME_WAIT）狀態，並將 **ACK** 發送回主機 B。
4. **主機 B** 從主機 A 收到 **ACK**，然後 **關閉連接**。

⚠️ *序列號在新通信中增加。例如計算機 A 和 B。A 會增加 B 的序列號。A 永遠不會增加自己的序列號。*

### <u>TCP 標誌 (TCP Flags)</u>

| 標誌 (Flag) | 名稱 (Name)       | 功能 (Function)                                               |
| ---------- | ---------------- | ------------------------------------------------------------ |
| SYN        | 同步 (Synchronize)    | 在初始通信中設置。協商參數和序列號 |
| ACK        | 確認 (Acknowledgment) | 作為對 SYN 標誌的確認設置。始終在初始 SYN 之後設置 |
| RST        | 重置 (Reset)          | 強制終止連接（雙向）                                       |
| FIN        | 完成 (Finish)         | 有序關閉通信                                                |
| PSH        | 推送 (Push)           | 強制無需緩衝即可交付數據                                    |
| URG        | 緊急 (Urgent)         |內部的數據被當作帶外數據發送。例如取消消息 |

### <u>端口號 (Port Numbers)</u>

- **互聯網分配數字管理局** (IANA, Internet Assigned Numbers Authority) - 維護服務名稱和傳輸協議端口號註冊表，該註冊表列出了所有端口號保留

- 範圍

  - **眾所周知的端口** (Well-known ports) - 0 - 1023

  - **已註冊端口** (Registered ports) - 1024 - 49,151

  - **動態端口** (Dynamic ports) - 49,152 - 65,535
  
    | 端口號 (Port Number) | 協議 (Protocol) | 傳輸協議 (Transport Protocol) |
    | ------------------- | -------------- | -------------------------- |
    | 20/21               | FTP            | TCP                        |
    | 22                  | SSH            | TCP                        |
    | 23                  | Telnet         | TCP                        |
    | 25                  | SMTP           | TCP                        |
    | 53                  | DNS            | TCP/UDP                    |
    | 67                  | DHCP           | UDP                        |
    | 69                  | TFTP           | UDP                        |
    | 80                  | HTTP           | TCP                        |
    | 110                 | POP3           | TCP                        |
    | 135                 | RPC            | TCP                        |
    | 137-139             | NetBIOS        | TCP/UDP                    |
    | 143                 | IMAP           | TCP                        |
    | 161/162             | SNMP           | UDP                        |
    | 389                 | LDAP           | TCP/UDP                    |
    | 443                 | HTTPS          | TCP                        |
    | 445                 | SMB            | TCP                        |
    | 514                 | SYSLOG         | UDP                        |


---
目前翻譯至原文747行