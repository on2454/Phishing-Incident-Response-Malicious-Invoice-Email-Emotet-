# 🚨 Phishing Incident Response – Malicious Invoice Email (Emotet)

**Author:** Oni Victor
**Role:** SOC Analyst (Tier 1)
**Project Type:** Incident Response | Email Security | Phishing Analysis

---

## 📌 Project Overview

This project documents a **SOC Tier 1 phishing incident response** involving a financially themed email sent to an Accounting department user. The email impersonated a legitimate finance organization and attempted to deliver **Emotet malware** via a compressed invoice attachment.

The objective of this project is to demonstrate **operational SOC skills**, including email header analysis, authentication validation, malicious URL identification, malware intelligence verification, and incident classification.

---

## 🎯 Scope of Analysis

The investigation focused on the following areas:

* Email header analysis (SPF and DMARC failures)
* Sender and domain impersonation detection
* Malicious link identification (look-alike login portal)
* Attachment and malware intelligence analysis
* Indicator of Compromise (IoC) extraction
* Incident classification and response actions

---

## 🔍 Key Findings

* The email failed **SPF** and **DMARC** authentication checks, indicating sender spoofing
* Look-alike domains and character substitution were used to impersonate a finance company
* The attachment (`invoice_9A8B.zip`) was confirmed as **Emotet malware** via VirusTotal
* The incident was classified as a **True Positive phishing attack**

---

## 🦠 Malware Identified

* **Malware Family:** Emotet
* **Type:** Trojan / Downloader
* **Delivery Method:** Phishing email attachment (ZIP)

---

## 🚫 Indicators of Compromise (IoCs)

### IP Address

```
198.51.100.10
```

### Domains

```
portal.finance-corp-login.com
mail-server.company-r-us.xyz
```

### File Hash (SHA256)

```
a8f5d021f1f807f7c50a1532f11f8e170a7b4de8a0f0a20f92b676f2d8a45B9C
```

---

## ✅ Incident Classification

* **Result:** True Positive
* **Severity:** High
* **Threat Type:** Phishing / Malware Delivery

---

## 🛠️ SOC Response Actions

* Email quarantined across affected mailboxes
* Malicious IPs, domains, and file hash recommended for blocking
* User confirmed no interaction with attachment
* Escalation path defined if execution had occurred

---

## 📂 Repository Contents

```
├── README.md
├── report/
│   └── Phishing_Incident_Report_Emotet.pdf
├── iocs/
│   └── iocs.txt
```

---

## 🧠 Skills Demonstrated

* Phishing detection and triage
* Email header analysis (SPF, DMARC)
* Malware intelligence analysis
* Incident documentation
* SOC Tier 1 operational workflow

---

## 🏁 Conclusion

This project reflects a realistic SOC Tier 1 phishing investigation and demonstrates the ability to analyze, classify, and respond to email-based threats using industry-standard techniques.

---

⭐ *This repository is intended for learning, portfolio demonstration, and SOC analyst skill validation.*
