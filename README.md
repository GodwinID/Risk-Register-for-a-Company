# 🔐 CloudNova Inc. — Information Security Risk Register
Create a Risk Register for a Mock Company

> A practical risk management lab exercise for a 10-employee cloud startup, covering 15 identified risks scored by **Likelihood × Impact**, a visual heat map, residual risk tracking, and an executive risk summary report.

---

## 📋 Overview

This repository contains a complete information security risk register for **CloudNova Inc.**, a fictional 10-employee cloud startup. It was built to simulate the workflow of a Risk Analyst identifying, scoring, and prioritizing cybersecurity risks in a small but real-world cloud environment.

---

## 📁 Repository Contents

| File | Description |
|------|-------------|
| [cloudnova_risk_register.xlsx](https://github.com/user-attachments/files/26393358/cloudnova_risk_register.xlsx) | Full risk register workbook (3 tabs: Risk Register, Heat Map, Dashboard) |
| [cloudnova_risk_summary.docx](https://github.com/user-attachments/files/26393366/cloudnova_risk_summary.docx) | Executive risk summary report — top 3 risks, scores, and recommended actions |

---

## 📊 Workbook — Tab Breakdown

### 1. Risk Register
15 risks identified and fully documented across key threat categories:

| Category | Example Risks |
|----------|--------------|
| Data Security | Data breach, misconfigured S3 bucket |
| Access Control | Credential reuse, excessive privilege, insider threat |
| Endpoint / Malware | Ransomware, phishing, security awareness gaps |
| Application Security | Insecure APIs, unpatched vulnerabilities, supply chain |
| Operational | No IR plan, untested backups, regulatory non-compliance |

**Each row includes:**
- Risk ID & Category
- Threat description & source
- Likelihood (1–5) × Impact (1–5) = **Inherent Risk Score**
- Risk Rating (High / Medium / Low) — color-coded 🔴🟡🟢
- Mitigation measures & control status
- Control Owner
- **Residual Risk Score & Rating** (after mitigation)
- Review Date

### 2. Risk Heat Map
A 5×5 Likelihood × Impact matrix with:
- Each cell color-coded red / amber / green by risk score
- Risk IDs plotted in the appropriate cell
- Full legend for score bands

### 3. Dashboard
Summary view showing:
- Count and percentage of High / Medium / Low risks (inherent and residual)
- Average inherent and residual scores per rating tier
- Totals row with overall average maturity

---

## 📄 Risk Summary Report

The Word document covers:
1. **Purpose & Scope** — context for the assessment
2. **Risk Landscape Snapshot** — distribution across High / Medium / Low
3. **Top 3 Priority Risks** — deep dive on Data Breach, Phishing, Misconfigured S3
4. **Overall Recommendations** — prioritized action table with owner and due date
5. **Conclusion** — executive summary and next steps

---

## 📈 Risk Distribution Summary

| Rating | Inherent Count | % |
|--------|----------------|---|
| 🔴 High | 7 | 47% |
| 🟡 Medium | 5 | 33% |
| 🟢 Low | 3 | 20% |

**After mitigations applied — Residual Distribution:**

| Rating | Residual Count | % |
|--------|----------------|---|
| 🔴 High | 0 | 0% |
| 🟡 Medium | 11 | 73% |
| 🟢 Low | 4 | 27% |

---

## 🚨 Top 3 Risks

| Rank | Risk | Score | Rating |
|------|------|-------|--------|
| 1 | Data Breach (customer PII) | 25 | 🔴 HIGH |
| 2 | Phishing Attack | 20 | 🔴 HIGH |
| 3 | Misconfigured S3 Bucket | 20 | 🔴 HIGH |

---

## 🗺️ Remediation Roadmap

```
Immediate  →  S3 Block Public Access + RDS encryption at rest
Week 1     →  Enforce MFA on all accounts + DMARC/DKIM/SPF
Month 1    →  Vulnerability scanning SLA + Incident Response Plan
Month 2    →  SSO + password manager + security awareness training
Month 3    →  PAM / just-in-time access + vendor risk program
Ongoing    →  Quarterly risk register review + phishing simulations
```

---

## 🧮 Risk Scoring Model

```
Risk Score = Likelihood (1–5) × Impact (1–5)

Low:    Score 1–8    🟢
Medium: Score 9–14   🟡
High:   Score 15–25  🔴
```

| Score | Likelihood | Impact |
|-------|-----------|--------|
| 5 | Almost Certain | Critical |
| 4 | Likely | Major |
| 3 | Possible | Moderate |
| 2 | Unlikely | Minor |
| 1 | Rare | Negligible |

---

## 🧰 How to Use This Project

1. **Download** the [cloudnova_risk_register.xlsx](https://github.com/user-attachments/files/26393389/cloudnova_risk_register.xlsx) file and open in Excel or Google Sheets
2. **Add or modify** risks in the Risk Register tab — scores and ratings update with the color coding
3. **Update residual scores** as you implement controls
4. **Check the Heat Map** to visualize where risks cluster
5. **Use the summary doc** as a template for board or investor risk reporting

---

## 📚 References

- [NIST SP 800-30 Rev. 1 — Risk Assessment Guide](https://csrc.nist.gov/publications/detail/sp/800-30/rev-1/final)
- [NIST SP 800-53 Rev. 5 — Security Controls](https://csrc.nist.gov/publications/detail/sp/800-53/rev-5/final)
- [ISO/IEC 27005:2022 — Information Security Risk Management](https://www.iso.org/standard/80585.html)
- [MITRE ATT&CK Enterprise Matrix](https://attack.mitre.org/)
- [CIS Controls v8](https://www.cisecurity.org/controls/v8)
- [OWASP Top 10](https://owasp.org/www-project-top-ten/)

---

## ⚠️ Disclaimer

This project is a **lab exercise** using a fictional company. It is intended for educational and training purposes only. Always consult a qualified risk or security professional for real-world implementations.

---

*Built by Godwin Iduye  |  © 2025*
