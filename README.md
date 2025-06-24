
# 🎯 Phishing Simulation: Credential Harvesting Attack (SET Toolkit)

## 📌 Overview

This project demonstrates a **realistic phishing simulation** using the **Social Engineering Toolkit (SET)** on Kali Linux. The goal was to assess user awareness, test email security posture, and gather insights to improve organizational security training.

---

## 🛠️ Tools & Technologies

- **Kali Linux**
- **SET (Social Engineering Toolkit)**
- **Credential Harvester Attack Module**
- **Apache/Localhost Web Server**

---

## 🎯 Objective

Simulate a credential harvesting phishing attack to:

- Evaluate employee vulnerability to social engineering attacks
- Understand common behavioral patterns in email interactions
- Generate actionable recommendations for cybersecurity training

---

## 🧪 Attack Methodology

### ✅ Attack Type:
**Credential Harvesting via Cloned Website**

### ✅ Setup Process:

1. **Launched SET via terminal**
   ```bash
   sudo setoolkit
   ```

2. **Attack Vector Selected:**
   - `Social Engineering Attacks` > `Website Attack Vectors` > `Credential Harvester Attack Method`

3. **Cloned Target Website:**
   - Chosen Template: `Google Login Page`
   - URL Cloned: `http://www.google.com`
   - SET automatically hosted the phishing page on `http://172.20.10.7`

4. **Crafted and Sent Phishing Email:**
   - Email disguised as a security alert prompting the user to log in to their Google account

---

## 💥 Simulation Result

- **Victim Interaction:**
  - User clicked the phishing link
  - Entered credentials into the spoofed Google login page

- **Captured Parameters:**
  ```txt
  USERNAME: Email-BlackDaniels@gmail.com
  PASSWORD: gooooodtttddx
  ```

- **Hit Details:**
  - IP: `172.20.10.7`
  - Request: `GET / HTTP/1.1` - Status 200
  - Timestamp: `24/Jun/2025 14:16:59`

> 🛑 _All credentials used were part of a controlled environment with mock data._

---

## 📈 Analysis

| Aspect                 | Result                          |
|------------------------|---------------------------------|
| Email Opened           | ✅                              |
| Link Clicked           | ✅                              |
| Credentials Submitted  | ✅                              |
| Suspicion Detected     | ❌                              |
| Simulation Success     | ✅ 100% effectiveness            |

### 🔍 Key Observations:

- The phishing site appeared convincing and bypassed basic user suspicion.
- The employee did not verify the domain or check for HTTPS.
- Browser security indicators were either ignored or unnoticed.

---

## 📚 Recommendations

To strengthen phishing defense across the organization:

1. **Employee Training**
   - Regular cybersecurity awareness workshops
   - Real-life phishing email examples and detection strategies

2. **Simulated Campaigns**
   - Schedule recurring phishing simulations using tools like Gophish or SET

3. **Technical Controls**
   - Implement SPF, DKIM, and DMARC
   - Enforce Multi-Factor Authentication (MFA)
   - Browser-based phishing warnings and link filtering

4. **Incident Reporting**
   - Create a simple reporting channel for suspicious emails
   - Encourage staff to report before clicking

---

## ✅ Conclusion

This simulation successfully demonstrated how a seemingly legitimate phishing page can deceive an unsuspecting user. The insights gathered will inform ongoing efforts in strengthening employee security posture and resilience against social engineering threats.

> ⚠️ _This project is strictly for educational and ethical penetration testing purposes only._

---

## 👨‍💻 Author

**Thywill Essel**  
Cybersecurity Student | Ethical Hacking Enthusiast  
GitHub: [@Thywill03](https://github.com/Thywill03)

---
