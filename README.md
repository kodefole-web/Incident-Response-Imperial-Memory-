# Incident-Response-Imperial-Memory-
# 🧠 Imperial Memory – Memory Forensics & Encrypted File Investigation

 📌 Overview
This project focuses on analyzing a memory dump (`Emperor.vmem`) to extract credentials, decrypt an encrypted archive, and recover hidden artifacts. The investigation simulates a real-world DFIR scenario involving encrypted data, decoy files, and memory artifact extraction using the Volatility Framework.

 🔍 Key Skills Demonstrated
- Memory forensics (Volatility)
- OS profile identification & kdbgscan analysis
- Credential extraction via `strings` + `grep`
- Encrypted archive deconstruction (7z)
- MD5 hash identification & validation
- Investigative triage of decoy files
- Linux terminal workflow

 🛠️ Tools Used
- Volatility 2.6 – Extract OS profile, analyze memory, enumerate processes  
- strings + grep – Locate username/password artifacts in memory  
- 7zip – Extract encrypted `.7z` archive  
- Linux Terminal – Full command-line analysis environment  

 🧪 Investigation Summary
- Identified suspicious encrypted file `gift.7z`  
- Located hidden reference to `ew4!suspicious.docx`  
- Analyzed `Emperor.vmem` to determine OS profile (`Win2016x64_14393`)  
- Used `strings | grep` to extract credentials from memory image  
- Decrypted archive & uncovered `secrets.txt`  
- Extracted MD5 hash: 0f235385d25ade312a2d151a2cc43865**

 🔐 MITRE ATT&CK Mapping
- TA0006 – Credential Access**  
- T1003 – OS Credential Dumping**  
  - T1555 – Credentials from Encrypted Files**

 📄 Full Report  
See: (https://github.com/user-attachments/files/23512460/Imperial.Memory.report.docx.pdf)
