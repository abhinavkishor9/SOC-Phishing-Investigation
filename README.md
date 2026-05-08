

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

### Technical Findings
* **Suspicious sender domain identified**: Initial detection in the 'Email Security' tool flagged a deceptive domain and link within the communication.

* **Email bypassed filtering controls**: The phishing attempt successfully reached the internal user inbox despite existing organizational security layers.

* **Potential credential harvesting indicators observed**: Analysis of the email content revealed markers specifically associated with credential-harvesting phishing attempts.

* **User delivery confirmed through SIEM event review**: Investigation of SIEM Event ID 257 and rule SOC282 verified that the email was successfully delivered to the recipient.

* **Log correlation and timestamp verification**: Email security logs and delivery reports were correlated with the alert timestamp of May 13, 2024, at 09:22 AM.

* **Impact assessment performed**: Conducted post-delivery checks to determine if the user interacted with the malicious URL or opened any files.

  
### 🔍 Indicators of Compromise (IOCs)

| IOC Type | Value |
| :--- | :--- |
| **Threat Type** | Phishing |
| **Delivery Status** | Delivered |
| **Sender Reputation** | Suspicious |
| **User Exposure** | High |


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

## Analyst Decision

* **Incident requires escalation**: The case has been prepared for escalation to ensure a deeper investigation into potential compromise.

* **Successful delivery confirmed**: Investigation verified that the deceptive email reached the user inbox, significantly increasing the risk profile.

* **Potential user interaction risk**: High risk levels for user compromise and credential theft necessitate further review of user activity.


* **True Positive classification**: The incident is officially closed as a True Positive, confirming that a legitimate threat bypassed initial security controls.

  

  ## 📋 Logs Reviewed
* **Email security logs**: Analyzed to identify the detection of suspicious domains and links.

* **Delivery reports**: Reviewed to confirm the email was successfully delivered to the user inbox.

* **SIEM event logs**: Evaluated Event ID 257 to validate the rule trigger and alert details.

* **User activity logs**: Checked to determine if there was any interaction with malicious files or URLs.
  
---

## 📂 Repository Contents

**This project is organized into specific branches to separate the stages of the investigation and the types of evidence collected**:

* **main**: The landing page containing the Executive Summary, the technical README.md, and the Threat Infographic.

* **iocs**: Dedicated repository for technical threat intelligence. Contains extracted Indicators of Compromise, including malicious URLs, suspicious sender domains, and IP addresses identified during the triage.

* **screenshots**: Contains visual evidence from the SIEM (Security Information and Event Management) platform, including log entries for Event ID 257 and rule SOC282.

* **final-report**: Houses the formal Incident Investigation PDF, providing the complete deep-dive analysis, root cause documentation, and long-term remediation strategies.
  
<img width="1000" height="900" alt="ChatGPT Image May 7, 2026, 10_32_53 AM (1)" src="https://github.com/user-attachments/assets/0c39977a-b60e-4823-9d47-5c2ab6baf510" />




