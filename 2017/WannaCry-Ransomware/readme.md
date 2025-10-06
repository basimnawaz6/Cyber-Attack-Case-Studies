# WannaCry Ransomware Attack (2017)

## 📅 Date of Incident
May 12, 2017

## 📄 Summary
The **WannaCry ransomware outbreak** was one of the most destructive cyberattacks in history, infecting **300,000+ computers** across **150 countries** within days.  
It leveraged a leaked NSA exploit known as **EternalBlue** (CVE-2017-0144) to automatically spread to vulnerable Windows systems using the **SMBv1 protocol**.  
Once inside, WannaCry encrypted user files, appending `.WCRY` to filenames, and demanded ransom payments in **Bitcoin**.

---

## 📌 Key Facts
- **Type of Attack:** Ransomware Cryptoworm
- **Exploit Used:** EternalBlue (CVE-2017-0144) + DoublePulsar backdoor
- **Primary Attack Vector:** Unpatched Windows SMBv1 vulnerability
- **Key Victims:**  
  - UK National Health Service (NHS) — 19,000+ appointments canceled  
  - FedEx (USA)  
  - Telefónica (Spain)  
  - Renault (France)  
  - Deutsche Bahn (Germany)
- **Estimated Global Loss:** $4–8 billion
- **Ransom Collected:** ~ $130,000

---

## 🔍 Technical Overview
1. **Initial Exploitation**  
   Exploited SMBv1 vulnerability to gain remote code execution on unpatched machines.
2. **Propagation**  
   Self-propagated without user interaction by scanning for other vulnerable systems on TCP port 445.
3. **Payload Execution**  
   Deployed ransomware component to encrypt files and display a ransom note demanding Bitcoin.
4. **Kill Switch**  
   Security researcher Marcus Hutchins accidentally stopped the first wave by registering a hidden “kill switch” domain found in the malware code: before executing, it would query the domain iuqerfsodp9ifjaposdfjhgosurijfaewrwergwea.com

---

## ⚠ Impact
- **Critical Infrastructure Disruption:** Hospitals, logistics, manufacturing, and transport services globally affected.
- **Reputational Damage:** Major organizations faced public scrutiny for not applying the available MS17-010 patch.
- **Compliance Issues:** Triggered legal reviews under HIPAA, GDPR (upcoming), and other data protection regulations.

---

## 🛡 Recommendations
- Implement **automated patch management** for critical vulnerabilities.
- **Disable SMBv1** on all systems.
- Transition to a **Zero Trust architecture** to limit lateral movement.
- Regular **incident response drills** for ransomware and worm-based attacks.

---

## 📂 Files in This Folder
- **[WannaCry-Ransomware.pdf](./WannaCry-Ransomware.pdf)** — Full incident report with detailed technical and business impact analysis.

---

## 🔐 Disclaimer
This report is for **educational and research purposes only**.  
It is intended to help cybersecurity professionals, students, and researchers understand real-world cyber incidents and improve defensive strategies.
