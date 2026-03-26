# Steganography: Hiding Data Inside Images
隱寫術：在影像中隱藏資料

---------

<h2>Outline 簡介</h2>

This project explores the concept of steganography, focusing on how sensitive data can be hidden within seemingly harmless files such as images.

本專題探討隱寫術的概念，重點在於如何將敏感資料隱藏於看似無害的檔案 (如圖片) 中。

Using the Steghide tool, we demonstrate how to embed and extract hidden data within image files through the Least Significant Bit (LSB) technique.

透過 Steghide 工具，本專題示範如何利用最低有效位 (LSB) 技術，在圖片中嵌入與提取隱藏資料。

The project highlights both offensive and defensive perspectives, showing how attackers may conceal data and how analysts can detect and recover it.

本專題同時涵蓋攻防兩面，展示攻擊者如何隱藏資料，以及分析人員如何偵測與還原這些資訊。

---------
<h2>Key Learning Outcomes 主要學習成果</h2>


* Understand the concept and purpose of steganography.<br/>
  理解隱寫術的概念與應用目的
  
* Differentiate between steganography and cryptography.<br/>
  能區分隱寫術與密碼學的差異
  
* Learn how data can be hidden within digital images using LSB techniques.<br/>
  學習如何利用 LSB 技術將資料隱藏於數位影像中
  
* Perform data embedding and extraction using Steghide.<br/>
  使用 Steghide 進行資料嵌入與提取

* Analyze file characteristics (e.g., size differences) to detect hidden data.<br/>
  透過檔案特徵（如大小差異）判斷是否存在隱藏資料

* Develop awareness of steganography in real-world cyber threats.<br/>
  建立對隱寫術在實際資安威脅中的認知


---------

<h2>Tools and Concepts Covered 涵蓋工具與概念</h2>

<div align="center">
</p>

| Category 分類                 | Tools / Concepts 工具 / 概念                                               |
| --------------------------- | --------------------------------------------------------------------------- |
| Data Concealment <br/>資料隱匿  | Steganography, LSB technique <br/>隱寫術、最低有效位                      |
| File Analysis <br/>檔案分析     | File size comparison, metadata inspection <br/>檔案大小比較、中繼資料分析 |
| Forensics <br/>數位取證         | Data extraction, hidden content recovery <br/>資料提取、隱藏內容還原      |
| Tools <br/>工具               | Steghide, diffchecker                                                    |
| Security Concepts <br/>資安概念 | Data obfuscation, covert communication <br/>資料混淆、隱密通訊           |



</div>
<br/>



---------


<h2>Materials and Methods 材料與方法</h2>

[Environment]
* Hyper-V virtualization platform (虛擬化平台)</b>
* Kali Linux virtual machine (Kali OS 虛擬機)</b>



[Tasks]
* Prepare Image and Secret Data File (準備圖片與隱藏資料檔案)</b>
* Install and Configure Steghide (安裝並設定 Steghide)</b>
* Embed Hidden Data into Image (將資料嵌入圖片中)</b>
* Compare Original and Stego Image (比較原始圖片與隱寫圖片)</b>
* Inspect File Differences and Indicators (檢查檔案差異與可疑指標)</b>
* Extract Hidden Data from Image (從圖片中提取隱藏資料)</b>
* Validate Extracted Content (驗證提取資料內容)</b>





---------

<h2>Practice 實踐</h2>

<p align="center">
<b>Task 1-1: Download File and Verify Integrity Using SHA256<br/> (下載檔案並使用 SHA256 驗證其完整性)</b><br/>
<img src="https://i.imgur.com/PIIR09U.jpeg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<b>Task 1-2: Verify File Reputation via VirusTotal<br/> (使用 VirusTotal 驗證檔案信譽)</b><br/>
<img src="https://i.imgur.com/X2BmHGi.jpeg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
* This step extends the analysis from integrity validation to threat intelligence correlation, providing additional context for risk assessment. <br/>此步驟將分析從完整性驗證延伸至威脅情報關聯，提供額外的風險評估依據 <br/>
<br />
<br />
<b>Task 2: Configure Antivirus Exclusion<br/> (設定防毒排除)</b><br/>
<img src="https://i.imgur.com/14KHT7X.jpeg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<b>Task 3: Prepare Payload Programs<br/> (準備封裝程式)</b><br/>
<img src="https://i.imgur.com/JrwDMX5.jpeg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<b>Task 4: Create a Wrapped file and Configure Execution Behaviour<br/> (建立封裝檔並配置執行行為)</b><br/>
<img src="https://i.imgur.com/6qsorSJ.jpeg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<b>Task 5: Execute the Packed File and Analyse Process Behaviour<br/> (執行封裝檔並分析進程行為)</b><br/>
<img src="https://i.imgur.com/lD3r5lY.jpeg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />



---------

<h2>Results 專題結論</h2>

This project demonstrates how executable wrapping techniques can be used to simulate basic Trojan behavior by packaging multiple programs into a single file and controlling their execution.

本專題展示了如何透過可執行檔封裝技術，將多個程式整合為單一檔案並控制其執行方式，以模擬基本木馬行為。

By embedding legitimate applications and configuring hidden execution, the wrapped file was able to trigger multiple processes, including background execution without direct user visibility.

透過嵌入合法程式並設定隱藏執行，封裝檔成功觸發多個程序，其中包含使用者不可見的背景執行行為。

Process analysis using Task Manager revealed abnormal behavior, such as a single executable spawning multiple processes and initiating hidden activities, which aligns with common characteristics of Trojan-based attacks.

透過工作管理員進行程序分析，觀察到異常行為，例如單一執行檔啟動多個程序並產生隱藏活動，這與典型木馬攻擊特徵一致。

In addition, file integrity verification and hash-based reputation checks were performed prior to execution, reinforcing secure analysis practices and ensuring reliable results.

此外，在執行前進行檔案完整性驗證與雜湊信譽查詢，強化了安全分析流程並確保分析結果的可靠性。

Overall, this project highlights how simple techniques can replicate real-world malware behavior and emphasizes the importance of process monitoring and behavioral analysis in detecting such threats.

總結而言，本專題展示了簡單技術如何重現真實世界的惡意程式行為，並強調透過程序監控與行為分析來偵測此類威脅的重要性。


---------

<h2>Security Insight 安全洞察</h2>

This project highlights the importance of verifying file integrity and assessing potential threats before execution, especially when dealing with externally sourced files.

本專題強調在執行外部來源檔案前，進行完整性驗證與潛在威脅評估的重要性。

By validating the SHA256 hash against a trusted source and cross-checking it with threat intelligence platforms such as VirusTotal, we ensured that the file had not been tampered with and did not match known malicious signatures.

透過比對 SHA256 雜湊值與可信來源，並進一步利用 VirusTotal 等威脅情報平台進行交叉驗證，我們確認該檔案未被竄改，且未匹配已知惡意樣本。

This demonstrates a critical security practice: hash-based validation serves as the first line of defense against supply chain attacks and malicious file distribution.

這展示了一項關鍵資安實務：基於雜湊值的驗證是防禦供應鏈攻擊與惡意檔案散佈的第一道防線。

Additionally, the workflow reinforces that static verification alone is not sufficient. Combining hash validation with reputation-based intelligence platforms improves confidence in file safety and reduces the risk of executing compromised binaries.

此外，本流程也強調僅依賴靜態驗證是不足的。結合雜湊驗證與信譽型威脅情報平台，能有效提升檔案安全性的判斷準確度，降低執行惡意程式的風險。

From a defensive perspective, this approach aligns with secure software handling practices, where every external artifact must be validated before being trusted within an environment.

從防禦角度來看，此方法符合安全軟體處理原則，即所有外部取得的檔案在被信任與使用前，都應進行驗證。

---------

<h2>Reference 參考</h2>

[UniSQ] [CSC6101 - Penetration Testing](https://handbook-guide.unisq.edu.au/course/2026/CSC6101)<br/>
[TryHackMe] [Cyber Kill Chain](https://tryhackme.com/room/cyberkillchainzmt)<br/>
<br/>
