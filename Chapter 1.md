# Chapter 1 -- 緒論
## 1.1
### 細胞式系統的歷史
- 1G：使用**分頻多工 (frequency division multiplexing, FDM)** 來進行語音通訊
- 2G：改採用**分時多工 (time division multiplexing, TDM)**
- 3G：為了滿足**整合與因、資料跟多媒體流量需求**，所以有了 3G

### 發展歷史及服務
- 1G：1970 年 - 1985 年 → 無線電
- 2G：1980 年 - 2000 年 → 全球行動通訊系統 (也稱 GSM 系統)
- 3G：
    - 主要特色：
        - 小型裝置
        - 高度全球化設計共通性
        - 全球漫遊能力
        - 與 **IMT-2000** 和固定網路相容
    - 重要元件：
        - 固定環境可達 **2Mbps**
        - 室內 / 戶外環境可達 **384kbps**
        - 車用環境可達 **144 kbps**
- 4G：
    - 主要特色：
        - 高速通訊
        - 通道相關排程
        - 使用移動 IP
        - 更廣的頻段
    - 重要元件：
        - FDD-LTE (FDD = 分頻雙工)：上行速率 **150Mbps**、下行速率 **40Mbps**
        - TD-LTE (TD = 分時雙工)：上行速率 **100Mbps**、下行速率 **50Mbps**
## 1.2
### 細胞式系統的特色
- 網路的特色取決於所應用的類型
    - 家用 vs 業界用
    - 商用 vs 個人環境用
- 在家用中，**集中式存取點 (access point, AP)** 負責與多種家用裝置通訊，並透過區域性的無線模式來控制他們

### 無線科技與其特色
| 技術                | 服務或特色                               | 覆蓋區域                         | 限制                           | 例子                                        |
|---------------------|------------------------------------------|----------------------------------|--------------------------------|---------------------------------------------|
| 細胞式              | 手機進行語音與資料傳送                   | 大都會環境                       | 大量資料的應用 → 可用頻寬低    | 手機、PDA                                   |
| 無線區域網路        | 傳統區域網路加上無線介面                 | 區域環境                         | 有限範圍                       | Motorola 的 ALTAIR <br> Proxim 的 range LAN |
| GPS                 | 三度空間之定位                           | 地表上任何地方                   | 昂貴                           | GNSS                                        |
| 以衛星為主的**PCS** | 主要是**語音傳訊**                       | 地表上任何地方                   | 昂貴                           | 衛星通訊系統                                |
| Ricochet            | 遠端高速、安全存取本機電腦               | 主要城市、機場、大學校園         | 有傳輸限制、環境因素會影響品質 | 微細胞式資料網路 (MCDN)                     |
| 家庭網路            | 連接家中各種設備                         | 家中任何地方                     | 家用範圍                       | 3Com Home Connect Home                      |
| Ad hoc 網路         | 一群人可聚在一起暫時共享資料             | 如同區域網路，只是無固定基礎建設 | 有限範圍                       | 國防應用                                    |
| WPAN (藍芽)         | 所有裝置不必透過纜線即可連結             | 私人 ad hoc 網路                 | 短距離、範圍有限               | 家用裝置                                    |
| 感測網路            | **大量**具有**無線**能力的**微小**感測器 | 小區域                           | 有限範圍                       | 國防與城市應用                              |

- ad hoc 網路：資訊傳遞式透過**同儕模式**，俗稱 **P2P (peer-to-peer) 模式**
- 換手 (handoff) 應盡量減少變動所使用到的無線電資源，為了使換手交換過程的頻率降到最低，應使用**巨細胞 (macrocellular)** 基礎建設及**多階層重疊 (multilevel overlapped)** 機制

## 1.3
### 細胞式系統的基礎
- 一個基地台會服務多個用戶，若覆蓋面積需要增大，就要多蓋一些基地台
- 此外，因為無線服務分配到的**頻寬有限**，為了增加整體系統效能，必須使用一些**多工技術**
- 主要有四種基本的多工技術
    - 分頻多重存取 (frequency division multiple access, FDMA)
    - 分時多重存取 (time division multiple access, TDMA)
    - 分碼多重存取 (code division multiple access, CDMA)
    - 正交分頻多工 (orthogonal frequency division multiplexing, OFDM)
    - 另外，還有一種叫做**空間分隔多重存取 (space division multiple access, SDMA)** 的新技術，使用特殊的**微波天線**

#### 分頻多重存取 (frequency division multiple access, FDMA)
- 簡單來說就是將一個頻率分成數個通道，然後基地台將數個通道分給不同使用者，**1G 都是使用這個技術**
<br><img src="Ch 1\1.PNG" width="300px" />
- FDMA 頻寬結構
<br><img src="Ch 1\2.PNG" width="400px" />

#### 分時多重存取 (time division multiple access, TDMA)
- 簡單來說就是將時間分成數個子時間，然後基地台將數個子時間分給不同使用者
<br><img src="Ch 1\3.PNG" width="400px" />
- TDMA 框架結構
<br><img src="Ch 1\4.PNG" width="400px" />

#### 分碼多重存取 (code division multiple access, CDMA)
- <img src="Ch 1\5.PNG" width="400px" />

### 兩個不同的多載波技術 (FDMA vs OFDM)
- <img src="Ch 1\6.PNG" width="400px" />

### 早期無線系統 → 大區域
- <img src="Ch 1\7.PNG" width="400px" />

### 細胞式系統 → 小區域
- <img src="Ch 1\8.PNG" width="400px" />

### 細胞式系統基礎建設架構圖
- <img src="Ch 1\9.PNG" width="400px" /><br>
    - PSTN：公用交通電話網路
    - MSC：Mobile Station Controller → 行動交換中心
    - BSC：Base Station Controller → 基地台控制中心
    - BS：Base Station → 基地台
    - MS：Mobile Station → 行動裝置

### 從 MS (行動裝置) 至 BS (基地台) 的通話建立基本步驟
- <img src="Ch 1\10.PNG" width="400px" /><br>
    1. 建立路徑
    2. 選擇使用通訊技術（FDMA / TDMA / CDMA）
    3. 控制資訊應答
    4. 開始在指派的流量通道上進行通訊

### 從 BS (基地台) 至 MS (行動裝置) 的通話建立基本步驟
- <img src="Ch 1\11.PNG" width="400px" /><br>
    1. **通話等待**
    2. 可建立一條路徑
    3. 選擇使用通訊技術（FDMA / TDMA / CDMA)
    4. 可進行通訊
    5. 開始在指派的流量通道上進行通訊

### 簡化後的無線通訊系統示意圖
- <img src="Ch 1\12.PNG" width="400px" /><br>

## 1.5
### 網路架構與協定
- 協定 = 基本規則，可以讓資訊透過系統化的步驟來相互交換
    - Open Systems Interconnections (OSI)
    - Transmission Control Protocol (TCP)
    - Internet Protocol (IP) 
        - Internet Protocol Version 4 (IPv4)
        - Internet Protocol Version 6 (IPv6) – 正在進行中
        - 無線 IP

## 1.9 無線大都會網路、無線區域網路、無線體域網路及無線個人網路
- 無線區域網路 (wireless local area network, WLAN)
    - 使用 IEEE 802.11 a/b/g/n/ac 等
- 無線個人網路 (wireless personal area networks, WPANs) 
    - 使用 IEEE 802.15.1 (藍芽) 
- 無線體域網路 (wireless body area networks, WBANs)
    - 使用 IEEE 802.15.6
- 無線大都會網路 (Wireless Metropolitan Area Network, WMAN)
    - 使用 IEEE 802.16
    - WiMAX
    - 3G、4G
    - 網狀網路

### 無線區域網路及無線個人網路技術
| 網路型態    | 節點範圍      | 主要用途                             | 建至位置             |
|-------------|---------------|--------------------------------------|----------------------|
| IEEE 802.11 | 30 公尺       | **無線節點**的標準協定               | 任意節點之間的連結   |
| HiperLAN    | 30 公尺       | **高速**的**室內**連線               | 機場                 |
| Ad hoc      | 大於 500 公尺 | **行動、無線，類似有線連線**         | 戰場、災難現場       |
| 感測網路    | 2 公尺        | 廉價、不適合久待的區域               | 核電廠、化工廠、海洋 |
| HomeRF      | 30 公尺       | 共用資源連接裝置                     | 家裡                 |
| Ricochet    | 30 公尺       | 高速的無線網際網路連線               | 機場、辦公室         |
| 藍芽網路    | 10 公尺       | 免於佈建雜亂的線路，適合用在低移動性 | 辦公室               |