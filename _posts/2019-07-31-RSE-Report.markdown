---
layout: post
title:  Trust & Privacy in Smart City IoT Solutions
date:   2019-07-31 16:40:16
description: Report for Trust & Privacy in Smart City IoT Solutions Project
---


# 科技部與英國愛丁堡皇家科學院人員交流合作計畫方案
# MOST-RSE Joint Project for Personnel-Exchange

# Trust & Privacy in Smart City IoT Solutions

## 1.合作研究規劃

### 1.1. 中文摘要/Abstract

本計畫的主要目標在研究物聯網系統在智慧城市的應用下，對資料與應用的信任與隱私的研究。在智慧城市的應用中，系統不間斷地公開場域中搜集各項資料，城市的居民開始對資料的擁有權，使用權，以及隱私權提出質疑。這些資料雖是公開搜集，但是，卻有可能侵害公民的隱私權。因此，本計畫的目的在現有物聯網中介軟體(WuKong以及IoTalk)中增加對資料信任與隱私權的保護，讓資料的使用不會侵害公民的隱私權，設置危害到公民的生命財產的安全。本計劃將結合本國在物聯網中介軟體與蘇格蘭亞伯丁大學在資料隱私以及倫理(Ethic)上的研究團隊，發展在適合在智慧城市使用的物聯網中介平台。資料的信任與隱私對物聯網智慧城市是否可以順利推動是一個決定性的因素。在無法取得社會共識下，推動這類的系統將會面臨相當大的阻力。此一計畫便是使用社會與科技結合的研究方式，研究公民對資料隱私與信任的質疑，提出能夠取得公民信任的資料搜集與使用模式，並在物聯網中介軟體中提供可以實踐的工具，讓系統開發者可以順利開發符合規範且可以被驗證的應用系統。

In this joint project we plan to adopt a socio-technical approach that
will consider a range of issues that are of interest to both Taiwanese
and Scottish researchers, namely: the appropriate governance
arrangements to cover IoT deployments (e.g. smart cities); an
understanding of the attitudes of citizens and communities to privacy
and risk in an IoT context; software (middleware) mechanisms that
enable users to make informed decisions about the trustworthiness of
devices and the information they produce. We characterise these as the
people strand and software strand of our proposed joint activities.

This project has been designed to align closely with the work of the
Intelligent IoT Middleware project at National Taiwan University and
the TrustLens project at the University of Aberdeen (funded by the
UK’s Engineering & Physical Sciences Research Council,
2016-2019). TrustLens is exploring what it means to realize IoT
solutions that are transparent, accountable, and which empower
end-users. 

### 1.2. 本計畫之背景與目的，以及研究方法、進行步驟及執行進度。

應用在智慧城市的物聯網系統可以協助政府與所在地的住民與使用者，提供即時的資訊，以更有效率地分配各項有形與無形的社會資源，並提供更安全與永續的生活環境。但是，在這樣的目標必須要在能適當保護收集的各項資料的隱私以及確保資料使用的倫理受到充分的尊重。

美國芝加哥市的智慧城市計畫 <a href="https://arrayofthings.github.io/"
target="blank">The Array of Things</a>，在 Michigan Ave. 裝設了大量
的感測器(如下圖所示)，量測行人的數量，空氣品質以及各種天氣資訊，以讓各
種資源的分配更加智慧化，例如：經由蒐集行人以及車輛的數量，可以更準確的
計算紅綠燈的停留長度，在保障行人與行車安全的前提下，有效地提昇道路的使
用率。但是，這項計畫在尚未取得住民對資料使用方式地信任前，便開使蒐集資
料，導致居民的恐慌，造成計畫必須在向居民說明資料的隱私性後方能繼續進行
(<a
href="http://chicagoinno.streetwise.co/2014/06/23/lets-all-stop-freaking-out-about-the-michigan-ave-data-sensors-please"
target="blank">2</a>, <a
href="http://www.chicagotribune.com/bluesky/originals/ct-expert-array-of-things-privacy-policy-bsi-20160621-story.html"
target="blank">3</a>, and <a href="http://www.chicagotribune.com/bluesky/originals/ct-array-of-things-privacy-policy-bsi-20160610-story.html" target="blank">4</a>)。 

<div class="img_row">
    <img class="col three" src="{{ site.baseurl }}/assets/img/RSE/ArrayofThings.jpg" alt="" title="Array of Things"/>
</div>
<div class="col three caption">
	Array of Things
</div>


此一實例說明，即時在公眾地區域蒐集資料，資料的使用權與安全性仍有續多必須考量地面向，例如：參與計畫的利害關係人(stakeholders)是否取得資料使用，儲存與再利用的權利與義務的充分共識，被觀測的行人是否得到充分的資訊，資料如何不會被第三者取得，進行商業使用時，相關利害關係人是否都公平地分配等問題。台灣目前有許多城市開始規劃智慧城市的計畫<a href="http://www.chinatimes.com/realtimenews/20160620005956-260410" target="blank">5</a>，希望藉由台灣本地豐沛的資通訊硬體資源建構一個更智慧且永續經營的城市。但是，目前各個城市的規劃方向仍缺乏與公民建立資料收集的共識，可以預見其他智慧城市遭遇到的資料使用與隱私性的爭議將無法避免。這些議題除了如何取得社會共識與保護隱私外，在資通訊技術上也必須發展適合的工具與技術，建立資訊流動的模型，提供資料使用的分析方法，確保資料使用確實符合相關共識的要求。

本計劃的目的在與亞伯丁大學(University of Aberdeen)合作研究，智慧城市系統中如何建立資料的信任與隱私模型，並在中介軟體提供有效地方式收集與處理資料，以達成此類模型的規範並最佳化系統的效能與使用性。

計畫申請團隊已經在物聯網中介軟體有深入的研究，以下說明計畫團隊在物聯網中介軟體的成果。

悟空(WuKong)是一個包含應用系統開發，虛擬執行環境以及動態應用程式安裝與管理的中介軟體。

**流程導向應用系統開發**：悟空中介軟體提供流程導向開發(Flow-Base Programming, FBP)環境，建立物聯網應用系統。此一開發環境的主要目的是提供不同領域（智慧城市，農業等）的專家，以資料流動的模型，建構類似使用試算表的方式，建構物聯網的應用程式。在悟空的開發環境中，使用者可以使用圖像化的建立應用程式，下圖所示為目前的程式開發環境。 

<div class="img_row">
    <img class="col three" src="{{ site.baseurl }}/assets/img/RSE/WuKongUI.png" alt="" title="User interface for WuKong development environment"/>
</div>
<div class="col three caption">
	User interface for WuKong development environment.
</div>


畫面的左邊為可用的服務資源，包含各項感測(Sensing)，計算 (computing)與制動(Actuation)等服務，例如：溫度感測，人員感測，煙霧的感測，數值比較運算，燈光，馬達控制等元件。畫面的右邊為資料流的定義，設計者利用已經定義的服務元件，經由有向線段的連結建構一個勿聯網應用系統，而每一個有向線段代表將資料由來源端(source)傳遞資料至接收端(destination)。目前已經提供超過100個服務元件提供物聯網應用使用。與傳統與其他物聯網流程導向程式開發不同的是，悟空的開發提供服務導向(Service Oriented)的開發方式，開發者僅定義服務之間的資料傳遞模型，不需要定義任何與硬體以及資料傳遞方式的設定。例如：不需要定義該服務將使用哪一種平台（例如：Intel 平台，ARM平台或是 AVR 平台）實作，也不需要定義資料是使用那一種網路協定(例如：WiFi，Bluetooth，或是Serial Port）傳送。硬體相關的設定延遲至應用程式安裝時才對應至可用的硬體平台。

**虛擬執行環境(Virtual Run-time Environment)**：
為了提供在物聯網平台具有可以由遠端無線更新應用程式的能力，悟空中介軟體提供虛擬執行環境(Virtual Runtime Environment)，使得使用者定義的服務不需要針對不同的硬體平台設計或轉譯成不同的原生碼(Native Code)。虛擬執行環境中的主要架構為悟空的Profile Framework [^WuKong], 提供平台描述硬體與軟體屬性的架構。下圖(a)為在資源有限且無作業系統的平台上的悟空虛擬執行環境，包含了通訊模組(communication module)，伺服器模組(Master Protocol)以及 Java 虛擬機(Java Virtual Machine)。在此一環境中，悟空的虛擬執行環境安排所有服務執行的順序 (Schedule)以及資料的傳遞。以 Java 設計的服務元件則在 JVM 上運行。

<div class="img_row">
    <img class="col three" src="{{ site.baseurl }}/assets/img/RSE/WuKong-Runtime.jpg" alt="" title="WuKong Run-Time"/>
</div>
<div class="col three caption">
	WuKong Run-Time
</div>

在資源較為豐富，具有作業系統的物聯網平台上，悟空的虛擬執行環境則以程序(Process)的方式與其他應用程式分享平台的軟硬體資源，如圖(b)所示。

為了提昇虛擬機(Virtual Machine)的執行效率，我們優化了虛擬機中的編譯器，設計一個 Ahead-of-Time (AoT)編譯器，讓執行時間達到接近 300 倍的提昇 [^JVM].

**應用程式安奘與管理**：悟空系統的計算模式以分散式運算為中心，並且讓應用系統可以在異質硬體平台上執行。為達成以上目標，悟空中介軟體設計了閘道器，指揮者，應用程式商店，以及WuDevice。下圖為系統架構示意圖。


<div class="img_row">
    <img class="col three center" src="{{ site.baseurl }}/assets/img/RSE/WuKongOverview_SoftwareArchitecture.jpg" alt="" title="WuKong Softare Architecture"/>
</div>
<div class="col three caption">
WuKong Softare Architecture
</div>

在悟空中介軟體中，WuKong Master (指揮者）負責搜集在環境中有哪些裝置(WuKong Device)參與運作，以及個別裝置的軟硬體特性。在從應用程式取得流程導向的應程式後，WuKong Master 先將服務對應至可以執行的硬體平台上，然後針對平台的軟硬體特性，產生可執行的程式碼，最後再將可執行的程式碼上傳至各個硬體平台。此一架構的優點在於，硬體與服務的連結在安裝的過程中才根據對應的結果，相互連結。這完全歸功於虛擬執行環境提供一個獨立於硬體之外的虛擬執行環境。此一方法，也允許WuKong Master (指揮者）可以動態地將服務由一個平台轉移至另一個平台。因此，當任何一個硬體平台損壞時，WuKong Master (指揮者）可以自行修復受損的系統，不需要使用者或工程師的介入。

計畫團隊的另一個中介軟體為 IoTtalk。IoTtalk系統是一個基於設備功能  (device feature) 特徵概念之物聯網設備平台，當物聯網設備連接至系統時，針對各種感測器，IoTtalk會自動產生或使用應用軟體來處理，因此每一個輸入設備可以相當方便地連接至輸出設備。圖1.1 說明4個物聯網設備D1、D2、D3以及D4，圖之左側代表其輸入功能(IDFs)；而圖之右側則代表其輸出功能(ODFs)。範例中，D1為一具有多種感測器之設備，稱為積木式感測器MorSensor。MorSensor之感測器可以很容易抽換成不同的感測器。如圖1.1左側所示，D1具有包括加速器(Acceleration)以及溫度(Temperature)兩個輸入功能，而智慧手機D2則具有包括加速器(Acceleration)以及麥克風(Microphone)兩個輸入功能。另一方面，如圖1.1右側所示， D2同時具有顯示(Display)之輸出功能；而燈泡(bulb) D3 則具有一個稱為流明(Luminance)之輸出功能。尾巴(Tail)D4則具有一個稱為顫動(Vibration)之輸出功能，這個特殊設備叫做“Transparent Organ”，發表於日內瓦國際發明展並獲得銀牌獎，設備尾巴會根據顫動值強度來進行搖晃。

<div class="img_row">
    <img class="col three" src="{{ site.baseurl }}/assets/img/RSE/IoTTalk.tif" alt="" title="Array of Things"/>
</div>
<div class="col three caption">
圖1.1. 物聯網設備D1, D2, D3, and D4之連線
</div>



圖1.1中線段(1)到(4)分別代表這些物聯網設備間之交流關係，當線段連接一個輸入及輸出功能即表示此輸入與輸出功能存在某種對應關係，而這種對應關係是以Python程式實作而成之網路應用程式。虛線方塊NA1代表這個網路應用程式NA1 實作D1、 D2 與D3間之交流關係(1)與(3)。同樣地，NA2實作D1與D2間之交流關係(2)，而NA3實作D2與D4間之交流關係(4)。舉線段(2)為例，線段(2)連接溫度感測器(Temperature)之輸入功能至顯示(Display)之輸出功能，也就是說，NA2先處理來自D1之溫度值，再將處理結果顯示到智慧手機D2。假如一支網路程式只處理一個獨立的設備功能，那麼我們就可以針對每一個設備功能分別撰寫程式。經由重複使用這些程式模組，即可輕易地建構網路應用程式。舉例而言，在圖1.1中，線段(4)之程式模組如圖1.2所示，網路應用 程式NA3可經由麥克風模組處理D2麥克風(Microphone)之音量，先計算麥克風音量之大小，再將結果傳送至震動（Vibration）模組，震動模組將接收到的值轉化成震動之大小（vibration intensity）。之後NA3再輸出此震動值大小至震動輸出功能（ODF)，進而驅動Ｄ4設備之尾巴震動。 


<div class="img_row">
    <img class="col three" src="{{ site.baseurl }}/assets/img/RSE/NA3.jpg" alt="" title="對應麥克風與震動之NA3軟體模組"/>
</div>
<div class="col three caption">
圖1.2. 對應麥克風與震動之NA3軟體模組
</div>


  
既然輸入功能與輸出功能各自相互獨立，這些軟體模組即可重複使用來建立網路應用，也就能大幅加速物聯網應用開發之時間。圖1.1顯示不同的物聯網設備也可能具有相同之輸入或輸出功能（IDFs/ODFs），例如，D1與D2都具有加速器（Acceleration）這個輸入功能，所以，NA1  就可以重複使用相同模組來實作所需之工作，例如，線段(1)與(3)即代表類似之功能。

根據設備特性，我們發展一套稱為IoTtalk之物聯網設備特性管理系統， IoTtalk 系統架構(如圖1.3)包含網路領域(network domain, 圖1.3 (a)) 與設備領域（device domain, 圖 1.3 (b))兩個領域。其中網路領域由四個系統組成，建立、設定與管理系統（Creation, Configuration and Management system，縮寫CCM; 圖1.3 (c)) 系統性將物聯網設備特性分類，管理並自動設定輸入與輸出功能之連結，儲存所有相關資訊於資料庫系統(DB; 圖1.3 (d))。執行與通訊系統（Execution and Communication system，縮寫EC; 圖1.3 (e)) 由兩個子系統組成， 通訊子模組系統（Communication SubModule system，縮寫CSM;圖1.3 (f))定義HTTP based RESTful API (Application Programming Interface)，提供給設備應用（Device Application，縮寫DA;圖1.3 (g)) 用來傳送或取得輸入/輸出設備資訊。當一個物聯網設備註冊/取消註冊(registers/deregister) 到EC時，DA會經由HTTP API要求CSM 去改變資料庫中之設備狀態，當物聯網設備完成註冊至DA後，即可以經由ＥＣ彼此相互通訊。執行子模組系統（Execution SubModule system，縮寫ESM;圖1.3 (h))代表執行網路應用之以連接相關輸入與輸出功能。圖形介面（GUI）(圖1.3 (i))提供一個友善的網頁使用者介面，可用來快速建立連線以及物聯網間有意義之交流（meaningful interactions），經由此一圖形介面，使用者可以指揮IoTtalk去執行所需求工作 ，用以建立或設定設備特性，功能，以及連線設定。 

<div class="img_row">
    <img class="col three" src="{{ site.baseurl }}/assets/img/RSE/IoTTalkArch.jpg" alt="" title="IoTtalk 系統架構"/>
</div>
<div class="col three caption">
圖1.3. IoTtalk 系統架構
</div>


在設備領域（device domain）中，DA (圖1.3 (g))被安裝於行動設備（例如，智慧手機），物聯網設備應用（IoT Device Application，縮寫IDA;圖1.3 (j))會間接經由DA連接至IoTtalk系統。在行動設備中，DA 由兩個軟體部分組成。設備應用至網路（Device Application to the Network，縮寫DAN;圖1.3 (k))經由Wi-Fi, 3G, or LTE.與IoTtalk進行通訊，用來執行IDA 註冊（registration）與資料交換。設備應用至物聯網設備（Device Application to IoT Device，縮寫DAI;圖1.3 (l))依據IDA 所指定之訊息格式與物聯網設備進行通訊，通常是經由藍芽（Bluetooth）、 Wi-Fi、ZigBee等無線網路所傳送之字串。物聯網設備必須先註冊到CSM，才能被IoTtalk所操作。IoTtalk註冊之概念遵循行動通訊之註冊流程. 行動通訊中註冊包括認證（authentication）、加密設定（initialization of encryption）、以及手機位置更新。註冊後，行動設備即可連接到網路並開始進行資料連線。目前IoTtalk之版本並未採用應用層之認證與加密，由於物聯網設備相對簡單之特性，IoTtalk之註冊流程僅包含連接（attachment）與資料連線設定。


#### 資料的信任與隱私

資料的信任定義資料的擁有權以及使用權，在物聯網的系統中，資料的擁有權定義是那一個系害關係人擁有資料，並決定資料被如何使用。以智慧城市為例，感測器在公眾場所例如車站，街道上蒐集到人員移動，聲音，影像資料等，都有可能經由資料連結，推算出某一個個體的位置，移動性甚至是日常的生活型態。但是，這些資料在被搜集後，是屬於公民的個人資料，亦或是公眾可共享的資料尚未有定論。運算資料後所產生的商業利益或公眾利益，例如，提供商業團體進行使用者行為分析，提供更準確的商業廣告投放，而增加商業的營收與獲利，此一獲利是否應該回饋至公民個體，或是公眾。資料隱私的議題在於提供資料給第三者時，對於資料揭露程度的規範。以街道的攝影機為例，如果僅揭露車輛種類（例如：大型車，小型車）進行車輛流量分析，則不會揭露個人的身份與動態。但是，若同時揭露車牌號碼，即時不揭露車輛所有人，以可以推算某一車輛在個別地區出現的頻率，時間等資訊，而侵害車輛所有人的隱私。

此一計畫便是使用社會與科技結合的研究方式，研究公民對資料隱私與信任的質疑，提出能夠取得公民信任的資料搜集與使用模式，並在物聯網中介軟體中提供可以實踐的工具，讓系統開發者可以順利開發符合規範且可以被驗證的應用系統。本計劃將結合台方在中介軟體 (<a href="https://newslabntu.github.io/wukong4iox/" target="blank">WuKong</a> 以及 IoTTalk)的研究與亞伯丁大學在資料隱私研究計畫 <a href="https://trustlens.wordpress.com" target="blank">TrustLens</a> 的成果，發展相關的規範，並實踐在中介軟體中。

[WuKong]: Kwei-Jay Lin, Neils Reijers, Yu-Chung Wang, Chi-Sheng Shih and Jane Y Hsu. Building smart m2m applications using the WuKong profile framework. In Green Computing and Communications (GreenCom), 2013 IEEE and Internet of Things (iThings/CPSCom), IEEE International Conference on and IEEE Cyber, Physical and Social Computing, pages 1175–1180, 2013.

[JVM]: Niels Reijers and Chi-Sheng Shih, Ahead-of-Time Compilation of Stack-Based JVM Bytecode on Resource-Constrained Devices, International Conference on Embedded Wireless Systems and Networks, 2017, Uppsala, Sweden.

## 2. 研究團隊：
### 2.1. 臺方參與研究人員（包括在此計畫內之工作角色及其重要性）

* 施吉昇副教授 (Chi-Sheng Shih, National Taiwan University)：為 WuKong 的技術主持人，將負責研究在 WuKong 軟體平台上的資料隱私性。
* 林一平教授 (Yi-Bing Lin, National Chiao Tung University)：為 IoTtalk 的技術主持人，將負責研究在 IoTTalk 軟體平台上的資料隱私性。
* 曾煜棋教授 (Yu-Chee Tseng, National Chiao Tung University：研究在資料傳遞過程中確保資料的安全性，尤其是在不同的通訊協定與平台。
* 任毅博士 (Ren Yi, National Chiao Tung University):  協同曾煜棋教授 研究在資料傳遞過程中確保資料的安全性，尤其是在不同的通訊協定與平台。

### 2.2. 英方參與研究人員（包括在此計畫內之工作角色及其重要性）

* Dr Caitlin Cottrill, Department of Geography, University of Aberdeen
* Dr David Corsar, Department of Computing Science, University of Aberdeen
* Dr Milan Markovic, Department of Computing Science, University of Aberdeen
* Dr Naomi Jacobs, Department of Computing Science, University of Aberdeen

### 2.3. 雙方團對隊之具體分工項目及內容；如果雙方已有合作經驗，可一併提出。

雙方團隊依照團隊的專長與現有成果分工合作，台灣團隊以發展軟體平台上的實作與效能優化，英方團隊以進行需求分析與規範。因此，雙方可以發揮各自所長。在人員方面可以
* Sharing results on user attitudes to IoT trust and privacy in Scotland with colleagues in Taiwan.
* Sharing experience of IoT deployment in a nursing home in Taiwan.
* Conducting user studies in Taiwan to investigate cross-cultural perspectives on IoT trust and privacy.
* Developing a shared view of priorities for governance of future IoT deployments.

在軟體發展方面可以
* Sharing existing software solutions for IoT/sensor metadata, data provenance and quality developed by Aberdeen researchers.
* Sharing details of the existing privacy and trust mechanisms deployed as part of the WuKong IoT and IoTtalk middleware platform.
* Designing extensions to the WuKong and IoTtalk platform to enhance capabilities such as accountability, transparency, personal data controls.
* Influencing design of the TrustLens trusted IoT software platform.

### 2.4.雙方合作對計畫之加值意義與效果；

此一計畫的執行雙方具有高度的互補性，台灣團隊的專長在於中介軟體以及通訊協定的設計，亞伯丁大學的專長在於資料隱私的研究。

台灣團隊已經在物聯網中介軟體（包含 WuKong 以及 IoTTalk)研究多年，對中介軟體，虛擬執行環境以及應用程式管理在小範圍物聯網應用有充分的經驗，可逐步擴展至智慧城市範疇。對台灣團隊的意義在於藉由此一合作可以取得資料隱私方面的最新技術，並研究此一技術在應用物聯網架構於智慧城市的核心技術。亞伯丁大學團隊則在資料隱私上有多年的研究成果，但是，對於物聯網的應用領域則是在 2016 年開始執行的 TrustLen 計畫中才開始接觸，與本團隊合作可將資料隱私技術建構在已經完整的中介軟體架構之上，研究適用於物聯網應用的資料隱私技術。

## 3. 第二年(2018-2019)互訪活動：
本年度的雙方研究團隊規劃互訪的活動為

|日程  |參加人員  |停留日數  | 訪問目的 |
|:--|:--|:--|:--|
| May, 2018	| Peter Edwards | 4 days |	了解台灣團隊在物聯網中介軟體的發展，並規劃合作方向。| 
| September, 2018 |	Chi-Sheng SHIH and Yu-Chee Tseng | 6 days | 	|
| April, 2019 |	Peter Edwards | |		
August, 2019	| Chi-Sheng SHIH and Yu-Min Hsieh |	5 days |	2019/08/27 - 2019/08/31 |

以下為本年度活動的訪問報告：

### 3.1 2018 年五月 亞伯丁大學 Peter Edwards 教授團隊訪問台灣。 

訪問期間為 2018/5/21 ~ 2018/5/24. 期間安排拜訪 台灣大學施教授團隊，交通大學林一平教授，交通大學曾煜棋教授，以及中央研究院陳柃志研究員團隊。討論合作題目，以及合作方式。

<div class="img_row">
    <img class="col three" src="{{ site.baseurl
    }}/assets/img/RSE/IMG_2582-50.jpeg" alt="" title="Visit NTU CSIE"/>
</div>
<div class="col three caption">
Prof. Peter Edwards visited Dept. of Computer Science and Information
    Engineering, National Taiwan University. (2018.05.21)
</div>

### 3.2 訪問蘇格蘭區研究團隊並舉辦 IoT Workshop
訪問期間：2018/09/08 - 2018/09/14. 訪問期間 舉辦為期兩天的  IoT Workshop. 

<div class="img_row">
    <img class="col three" src="{{ site.baseurl
    }}/assets/img/RSE/IMG_3989-52.jpeg" alt="" title="IoT Workshop at
    University of Aberdeen"/>
</div>
<div class="img_row">
    <img class="col three" src="{{ site.baseurl
    }}/assets/img/RSE/IMG_3985-54.jpeg" alt="" title="IoT Workshop at
    University of Aberdeen"/>
</div>
<div class="col three caption">
NTU Team visited University of Aberdeen and delivered speech at IoT
    Workshop (2018.09.10)
</div>

### 3.3 2019 年四月 亞伯丁大學Peter Edward 教授訪問台灣。

訪問期間：2019/04/12 - 2019/4/20

訪問期間 Prof. Eward 參加 台灣大學醫學院舉辦的 New Progress in the Application of Modern Technology in LTC Industry，並發表演講，並訪問交通大學，以及參觀自動駕駛公車。

4/14: Workshop: New Progress in the Application of Modern Technology in LTC Industry 
現代科技在長照領域應用的新進展 - ERICA 計畫成果發表會（台灣大學醫學院 201 講堂）

<div class="img_row">
    <img class="col three" src="{{ site.baseurl
    }}/assets/img/RSE/CIMG1056-56.jpg" alt="" title="LTC Workshop at NTU"/>
</div>
<div class="img_row">
    <img class="col three" src="{{ site.baseurl
    }}/assets/img/RSE/CIMG1090-58.jpg" alt="" title="LTC Workshop at NTU"/>
</div>
<div class="img_row">
    <img class="col three" src="{{ site.baseurl
    }}/assets/img/RSE/CIMG1125-64.jpg" alt="" title="LTC Workshop at NTU"/>
</div>
<div class="img_row">
    <img class="col three" src="{{ site.baseurl
    }}/assets/img/RSE/CIMG1155-66.jpg" alt="" title="LTC Workshop at NTU"/>
</div>
<div class="col three caption">
Workshop for New Progress in the Application of Modern Technology in LTC Industry (2019.04.14)
</div>


[1]: Array of Things, https://arrayofthings.github.io/
[2]: Let’s all stop freaking out about the Michigan Ave. Data Sensors, please! http://chicagoinno.streetwise.co/2014/06/23/lets-all-stop-freaking-out-about-the-michigan-ave-data-sensors-please
[3]: City needs more details in Array of Things privacy policy, experts day, http://www.chicagotribune.com/bluesky/originals/ct-expert-array-of-things-privacy-policy-bsi-20160621-story.html
[4]: City seeks input on privacy policy for Array of Things sensor network. http://www.chicagotribune.com/bluesky/originals/ct-array-of-things-privacy-policy-bsi-20160610-story.html
[5]: 六都智慧城從桃竹出發 工研院士提建言, http://www.chinatimes.com/realtimenews/20160620005956-260410

### Publications supported by this project 
<ul>
    <li>J.-J. Chou and C.-S. Shih, “Turning Over Detecting Using Super-Resolution Thermal Image,” in The 26th IEEE International Conference on Embedded and Real-Time Computing Systems and Applications, Virtual Conference, 2020</li>
    <li>C.-S. Shih, Y.-T. Wang, and J.-J. Chou, “Multiple-Image Super-Resolution for Networked Extremely Low-Resolution Thermal Sensor Array,” in Proceedings of the 2020 IEEE Second Workshop on Machine Learning on Edge in Sensor Systems, New York, NY, USA, 2020, pp. 1–6.</li>
    <li>J.-J. Chou and C.-S. Shih, “Parameterized Data Reduction Framework of Thermal Sensing for Gait Velocity Measurements,” in The 24th IEEE International Confernece on Embedded and Real-Time Computing Systems and Applications, Hakodate, Japan, 2018, pp. 76–84.</li>
    <li>J.-J. Chou and C.-S. Shih, “IoT Sensing Networks for Gait Velocity Measurement,” International Journal of Applied Mathematics and Computer Science (AMCS), vol. 29, no. 2, pp. 245–259, 2019.</li>
	<li>J.-J. Chou and C.-S. Shih, “Parameterized Data Reduction Framework of Thermal Sensing for Gait Velocity Measurements,” in The 24th IEEE International Confernece on Embedded and Real-Time Computing Systems and Applications, Hakodate, Japan, 2018, pp. 76–84.</li>
	<li>C.-S. Shih, J.-J. Chou, W.-D. Wang, and K.-C. Huang,
	“Measuring Gait Speed Using Temporal and Location-Aware Sensing
	Services in Smart Homes,” in 10th IEEE Conference on
	Service-Oriented Computing and Applications, SOCA, Kanazawa,
	Japan, 2017, pp. 173–180.</li>
	<li>C.-S. Shih et al., “Collaborative Sensing for Privacy Preserving Gait Tracking Using IoT Middleware,” in Proceedings of the International Conference on Research in Adaptive and Convergent Systems, (RACS), Krakow, Poland, 2017, pp. 152–159.</li>
</ul>

<hr>
