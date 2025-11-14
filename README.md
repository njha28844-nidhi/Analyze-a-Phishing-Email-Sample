# Analyze-a-Phishing-Email-Sample

# Day 2 – Phishing Email Analysis

## 📌 Objective
Analyze a phishing email sample and identify indicators of a phishing attack by reviewing sender information, headers, URLs, attachments, and social engineering patterns.

---

## 📨 Sample Phishing Email Summary
A phishing email pretending to be from “PayPal Security” was analyzed.  
It attempts to trick users into clicking a malicious login link by claiming suspicious activity.

Full email content is available in `email_sample.txt`.

---

## 🚨 Phishing Indicators Identified

### 1️⃣ Suspicious Sender
- Display name: **PayPal Support**
- Sender address: **security@paypa1-verification.com**
- Domain uses **"1" instead of "l"** → clear domain spoofing.

---

### 2️⃣ Email Header Red Flags
- **SPF:** Fail  
- **DKIM:** Fail  
- **DMARC Alignment:** Fail  
- The originating IP does **not** belong to PayPal infrastructure.
- Details available in `header_analysis.txt`.

---

### 3️⃣ Malicious Links
The email text displays:

> https://www.paypal.com/activity

But the actual embedded link redirects to:

> http://verify-login-secure-paypal.xyz/login

This mismatch indicates a phishing URL designed to steal credentials.

---

### 4️⃣ Social Engineering Techniques
The message uses:
- **Urgency:** “Your account will be suspended in 24 hours.”
- **Fear:** Claims unauthorized login attempts.
- **Action pressure:** “Click the link below to secure your account.”
- **Grammar errors** typical of phishing campaigns.

---

### 5️⃣ Suspicious Attachment
Attachment included: **Invoice_87821.html**  
This is commonly used to redirect users to malware or a phishing login page.

---

## 📌 Conclusion
The analyzed email contains multiple indicators of phishing, such as:
- Domain spoofing  
- Failed email authentication checks  
- Malicious redirect URL  
- Social engineering  
- Suspicious attachment  

Users receiving such emails should **not click links or download attachments** and must report to their security team.


---

## ✔️ Submitted for Day 2 Task
This repository contains all required analysis files as per task expectations.
