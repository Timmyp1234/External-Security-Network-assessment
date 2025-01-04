# **Project: External Network Security Assessment for Company X**

### **Summary**
In **May 2024**, Company X engaged a security firm to perform an **External Network Security Assessment**. This assessment identified vulnerabilities in the company's external infrastructure, mimicking a potential attacker's approach to identify potential entry points.

---

## **High-Level Overview**

### **Objective**
To identify vulnerabilities in the external infrastructure and provide mitigation strategies to strengthen the overall security posture.

### **Scope**
The assessment covered external systems accessible via the internet without internal access or prior knowledge, emulating an external adversary.

### **Methodology**
1. **Information Gathering:** Collection of relevant data for scoped systems.
2. **Vulnerability Scanning:** Automated and manual identification of weaknesses.
3. **Analysis:** Risk rating using likelihood and consequence.

### **Tools Used**
- **Burp Suite Pro**
- **Nmap**
- **SSLScan**
- **OpenVAS**
- **Nessus**

---

## **Key Findings**
- **Total Vulnerabilities Identified:** 16
  - **High Risk:** 7
  - **Moderate Risk:** 9
  - **Low Risk:** 0
  - **Critical Risk:** 0

### **Sample High-Risk Vulnerabilities**
1. **Web Server Transmits Cleartext Credentials**  
   *Description:* Passwords transmitted over HTTP instead of HTTPS.  
   *Remediation:* Enforce HTTPS and implement Multi-Factor Authentication.  

2. **OpenSSH Multiple Vulnerabilities**  
   *Description:* Use of outdated OpenSSH versions allowing potential remote code execution.  
   *Remediation:* Upgrade to OpenSSH version 9.7 or later.  

3. **CGI Generic SQL Injection (Blind)**  
   *Description:* Vulnerable CGI scripts allow unauthorised access to databases.  
   *Remediation:* Secure all CGI scripts with proper input validation.  

### **Overall Recommendations**
- Implement regular patch management for software and systems.
- Strengthen TLS/SSL configurations to mitigate cryptographic vulnerabilities.
- Enforce HTTP Strict Transport Security (HSTS) and disable outdated protocols like TLS 1.0 and 1.1.
- Secure application configurations to avoid information disclosure.

---

## **Risk Management Approach**

### **Risk Ratings**
- **Likelihood:** Assessed based on factors such as exploit availability, skill requirements, and access level.
- **Consequence:** Measured against service impact, stakeholder trust, and potential financial loss.

| Likelihood       | Consequence       | Risk Rating |
|-------------------|-------------------|-------------|
| **Almost Certain** | Catastrophic      | Critical     |
| **Likely**        | Major             | High         |
| **Possible**      | Moderate          | Medium       |
| **Rare**          | Insignificant     | Low          |

### **Mitigation Plan**
1. Prioritise patching of high-risk vulnerabilities.
2. Review and secure exposed network services.
3. Perform regular vulnerability scans and security audits.

---
## **Lessons Learned**
- **Proactive Patching is Crucial:** Many vulnerabilities arose from outdated software. Regular updates and patching cycles are essential to maintaining a secure environment.  
- **Effective Risk Prioritisation:** Categorising vulnerabilities based on impact and likelihood ensures the most critical issues are addressed first.  
- **Holistic Security Planning:** Evaluating systems as a whole rather than in isolation provides a clearer view of potential attack vectors.  
- **Training and Awareness:** Even with technical mitigations in place, the importance of user training cannot be overstated. Misconfigured systems can be avoided through better operational awareness.

---

## **What Went Well**
- **Comprehensive Assessment:** The engagement successfully identified vulnerabilities across the scope, including several that could have led to severe risks if exploited.  
- **Team Collaboration:** The external assessment team worked closely with Company X, ensuring seamless communication and timely issue reporting.  
- **Quick Response to Findings:** Company X’s IT team promptly patched several high-risk vulnerabilities during the engagement, showcasing their commitment to improving security.  
- **Accurate Tool Usage:** Leveraging industry-standard tools provided detailed insights and ensured accurate vulnerability identification.  

