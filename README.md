

# SOC Case Study: Deceptive Phishing Investigation

## 📌 Executive Summary

On **May 07, 2026**, a SIEM alert (Rule: SOC282) was triggered regarding a deceptive email detected within the environment. This investigation confirmed the incident as a **True Positive**, as a phishing email containing suspicious links was successfully delivered to an internal user's inbox.



### 📊 Incident Profile

| Category | Details |
| :--- | :--- |
| **Incident Title** | Phishing Alert - Deceptive Mail Detected|
| **Date** | May 07, 2026 |
| **Severity** | Medium |
| **Event ID** | 257 |
| **Status** | True Positive / Closed |

## 🔍 Investigation Overview

### Indicators of Compromise (IOCs)

* **Threat Type**: Deceptive Phishing Email identified in Email Security logs.


* **Delivery Status**: Successfully delivered to the user inbox.


* **Primary Indicator**: Suspicious domain and link detected within the message body.


* **Sender Behavior**: Observed unverified sender patterns and phishing characteristics.

### Action Workflow

* **Validation**: Reviewed SIEM alert details for Event ID 257 and confirmed the detection rule was correctly triggered.


* **Analysis**: Verified email security logs and delivery reports to confirm successful delivery.


* **Impact Assessment**: Evaluated potential user exposure and checked for interactions with malicious content.


* **Final Assessment**: Confirmed the email reached the recipient, increasing the organizational risk profile.



---

## ⚠️ Risk Assessment

The investigation identified the following risk levels associated with this threat:

* **User Compromise**: High.
* **Credential Theft**: High.
* **Malware Risk**: Medium.
* **Organization Impact**: Medium.


 **Root Cause**: A targeted attempt to trick the recipient into interacting with malicious content or revealing sensitive information.



---

## 💡 Recommendations & Lessons Learned

* **Immediate Action**: Block the identified sender and update email filtering mechanisms to prevent similar delivery.
* **User Training**: Implement awareness training to help users identify suspicious emails and deceptive links.
* **Process Improvement**: Ensure prompt investigation of delivered phishing emails to reduce the window of exposure.

---

## 📂 Repository Contents

* **Full Report**: Detailed SOC Incident Investigation PDF.
* **Phishing_Threat_Infographic.png**: Visual breakdown of the threat, risks, and actions taken.

<img width="1000" height="900" alt="ChatGPT Image May 7, 2026, 10_32_53 AM (1)" src="https://github.com/user-attachments/assets/0c39977a-b60e-4823-9d47-5c2ab6baf510" />




