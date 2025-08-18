# Marriott International Data Breach (2018)

## 📅 Date of Incident  
- **Initial Compromise:** 2014 (undetected)  
- **Discovery Date:** September 8, 2018  
- **Public Disclosure:** November 30, 2018  

---

## 📄 Summary  
The **Marriott International data breach** was one of the most severe corporate cybersecurity failures in history, exposing **339 million guest records** from the Starwood Hotels reservation system. This **Advanced Persistent Threat (APT)** attack went undetected for **four years**, even through Marriott's 2016 acquisition of Starwood.  

Attackers exfiltrated highly sensitive data including **5.25 million unencrypted passport numbers** and **9.1 million weakly protected payment cards**, triggering landmark **GDPR enforcement** and costing the company over **$1 billion** in fines, settlements, and remediation.

---

## 📌 Key Facts  
- **Type of Attack:** State-sponsored cyber espionage (APT)  
- **Primary Attack Vector:** Remote Access Trojan (RAT) + credential harvesting  
- **Key Exploits:**  
  - Flat network architecture with no segmentation  
  - Absence of multi-factor authentication  
  - Misrepresentation of SHA-1 "encryption" on payment cards  
- **Affected Data:**  
  - 339 million guest records (PII, travel history)  
  - 5.25 million unencrypted passport numbers  
  - 9.1 million weakly protected payment cards  
- **Regulatory Impact:**  
  - **£18.4 million** GDPR fine (UK ICO)  
  - **$52 million** FTC + state settlement  
  - 20-year FTC consent order  

---

## 🔍 Technical Overview  
1. **Initial Compromise (2014)**  
   - Attackers gained access via RAT or unpatched servers (likely Windows Server/RDP vulnerabilities).  
2. **Persistence & Expansion**  
   - Used tools like **Mimikatz** for credential harvesting and privilege escalation.  
   - Exploited flat network design to move laterally into Starwood’s reservation database.  
3. **Data Exfiltration (2014–2018)**  
   - Systematically copied and encrypted guest records to avoid detection.  
4. **Discovery (2018)**  
   - IBM Guardium anomaly detection flagged a suspicious SQL query that revealed the breach.  

---

## ⚠ Impact  
- **Regulatory Precedent:** First major GDPR enforcement case impacting a U.S. corporation.  
- **Financial Consequences:** Over **$1 billion** in fines, legal fees, and remediation costs.  
- **Reputational Damage:** 5% stock drop and severe erosion of customer trust.  
- **Operational Disruption:**  
  - Free passport replacement program for affected guests.  
  - 20-year mandatory security oversight imposed by U.S. regulators.  

---

## 🛡 Recommendations  
- **M&A Cybersecurity:** Require comprehensive cybersecurity due diligence during acquisitions.  
- **Zero Trust Implementation:** Enforce network micro-segmentation and least-privilege access.  
- **Data Governance:**  
  - Classify and encrypt sensitive data using strong encryption (AES-256).  
  - Implement strict data retention and deletion policies.  
- **Threat Detection & Response:**  
  - 24/7 SOC monitoring with **EDR** and **UEBA** solutions.  
  - Conduct quarterly **red team exercises** to test resilience.  

---

## 📂 Files in This Folder  
- **[Marriott-2018-Data-Breach.pdf](./Marriott-2018-Data-Breach.pdf)** — Full forensic analysis, regulatory findings, and remediation roadmap.  

---

## 🔐 Disclaimer  
This report is for **educational and research purposes only**.  
It provides cybersecurity professionals with critical insights into **large-scale APT attacks** and highlights the importance of **enterprise risk management**.
