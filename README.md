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
<b>Task 1: Prepare Image and Secret Data File<br/> (準備圖片與隱藏資料檔案)</b><br/>
<img src="https://i.imgur.com/kJJ4a7t.jpeg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<b>Task 2: Install and Configure Steghide<br/> (安裝並設定 Steghide)</b><br/>
<img src="https://i.imgur.com/bx09NnK.jpeg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<b>Task 3: Embed Hidden Data into Image<br/> (將資料嵌入圖片中)</b><br/>
<img src="https://i.imgur.com/3StX54O.jpeg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<b>Task 4: Compare Original and Stego Image<br/> (比較原始圖片與隱寫圖片)</b><br/>
<img src="https://i.imgur.com/504PWnE.jpeg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<b>Task 5: Inspect File Differences and Indicators<br/> (檢查檔案差異與可疑指標)</b><br/>
<img src="https://i.imgur.com/5V8Z7Vq.jpeg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<b>Task 6: Extract Hidden Data from Image<br/> (從圖片中提取隱藏資料)</b><br/>
<img src="https://i.imgur.com/ULp3vGp.jpeg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<b>Task 7: Validate Extracted Content<br/> (驗證提取資料內容)</b><br/>
<img src="https://i.imgur.com/taPH0DY.jpeg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />


---------

<h2>Results 專題結論</h2>

This project demonstrates how steganography can be used to conceal and recover data within digital images using the Steghide tool.

本專題展示了如何使用 Steghide 工具，將資料隱藏於數位影像中並成功進行還原。

By embedding a text file into an image using the LSB technique, we created a stego file that appeared visually identical to the original while containing hidden content. Through file comparison and metadata inspection, we identified subtle indicators such as file size differences that suggested the presence of concealed data.

透過 LSB 技術將文字檔嵌入圖片中，我們成功建立了一個在視覺上與原圖無差異，但實際包含隱藏資料的隱寫檔案。透過檔案比較與中繼資料分析，我們發現如檔案大小差異等細微跡象，顯示可能存在隱藏資料。

Finally, the hidden data was successfully extracted and validated, confirming the integrity of the steganographic process.

最終成功提取並驗證隱藏資料，證明隱寫與還原流程的完整性與可行性。

This project reinforces the concept that data can be hidden in plain sight and requires specialized techniques for detection and analysis.

本專題強化了一項關鍵概念：資料可以隱藏於表面可見的媒介中，且需透過特定技術才能偵測與分析。


---------

<h2>Security Insight 安全洞察</h2>

This project highlights a critical but often overlooked threat vector: data can be covertly embedded within benign-looking files, bypassing traditional security controls.

本專題揭示一項常被忽略的威脅途徑：資料可被隱藏於看似正常的檔案中，進而繞過傳統安全機制。

Unlike encrypted traffic or obvious malware, steganography operates at the data level, making it significantly harder to detect using standard network or signature-based defenses.

與加密流量或明顯惡意程式不同，隱寫術運作於資料層，使其難以被傳統的網路監控或特徵碼偵測機制發現。

From an attacker’s perspective, steganography can be used for covert communication, data exfiltration, or payload delivery without raising immediate suspicion.

從攻擊者角度來看，隱寫術可用於隱密通訊、資料外洩或惡意載荷傳遞，且不易引起注意。

From a defensive standpoint, this reinforces the need for deeper file inspection, anomaly detection, and contextual analysis, rather than relying solely on surface-level indicators.

從防禦角度而言，這強調了進階檔案檢測、異常行為分析與情境判斷的重要性，而非僅依賴表面特徵。

This project also demonstrates that minor inconsistencies, such as unexpected file size differences, can serve as early indicators of hidden data.

此外，本專題也顯示細微異常（如檔案大小差異）可作為隱藏資料的初步指標。

Overall, this reinforces a key defensive principle:
Not all threats are visible at the network level—some are hidden within the data itself.

總結而言，本專題強化了一項核心防禦觀念：
威脅不一定存在於網路層，有些是隱藏於資料本身之中。

---------

<h2>Reference 參考</h2>

[UniSQ] [CSC6101 - Penetration Testing](https://handbook-guide.unisq.edu.au/course/2026/CSC6101)<br/>
[EC-Council] [Certified Ethical Hacker Practical](https://aspen.eccouncil.org/Home)<br/>
<br/>
