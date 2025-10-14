# Phishing Simulation & Email Analysis

# Objective
Simulate and analyze a credential-harvesting phishing email in a **safe, controlled environment** and document visible indicators of impersonation and malicious intent.

# Tools Used
- Email accounts (attacker test + target test) — Gmail  
- PhishTool (rendering & metadata)  
- Inbox message source (Gmail “Original Message” view)  
- URL reputation scanners (optional)

# Environment / Safety Note
All actions were performed on test accounts I control. No real users or organizations were targeted. Do **not** click any suspicious links.

---

# Steps Performed
1. Created a phishing-style email design and sent it from a test Gmail account to a test target inbox.  
2. Captured inbox view showing subject, display name, sender address, email body and suspicious link.  
3. Uploaded the message to PhishTool to render metadata and message details.  
4. Captured the Gmail “Original Message” view showing SPF/DKIM/DMARC results and Message-ID.  
5. Documented findings and recommendations based on visible artifacts.

---

## Key Observations (from screenshots)
- **Subject:** `Important: Password Expiration Notice!` (social engineering urgency).  
- **Display name:** `bank commonwealth bank` — attempts to impersonate a bank.  
- **Sender email:** `bankcommonwealthb@gmail.com` — a personal Gmail address (mismatch with display name).  
- **Suspicious link (rendered in email body):** `https://commonwealth-bank-dot-com/secure` — look-alike domain formatting, high risk for credential harvesting.  
- **Authentication metadata (Gmail “Original Message”):** SPF / DKIM / DMARC show **PASS** for `gmail.com` with originating IP `209.85.220.65` (Google SMTP) — indicates email was sent via Gmail, not from the bank’s domain.  
- **PhishTool rendered view:** clearly displays the suspicious link, sender address and originating IP. This confirms impersonation tactics and the link that would likely be used for credential capture.

---

# Findings & Recommendations

<img width="1164" height="618" alt="image" src="https://github.com/user-attachments/assets/4c092fc1-e75a-4757-848d-369184ba28a2" />

---

# Evidence (include these in `screenshots/` and reference in the repo)
-  Inbox view showing subject, display name, sender email and email body with highlighted suspicious link.
  <img width="1733" height="775" alt="Screenshot 2025-10-14 163100" src="https://github.com/user-attachments/assets/d866553f-1d44-4d53-a452-4388ed275a5c" />

- Gmail "Original Message" view showing Message-ID, Timestamp, SPF/DKIM/DMARC PASS and originating IP (209.85.220.65).
  <img width="2383" height="1066" alt="Screenshot 2025-10-14 163202" src="https://github.com/user-attachments/assets/ba2a86ef-08c6-4fb8-a587-559b7326a15e" />

- PhishTool rendered view showing sender, display name, originating IP and the suspicious URL.
  <img width="2735" height="1484" alt="Screenshot 2025-10-14 182733" src="https://github.com/user-attachments/assets/2bc874e3-6806-4cc2-bbd9-321ead04c557" />


---

# Limitations
- Analysis is based on rendered email content and visible metadata only. Full SMTP Received chain or full raw headers were not analysed beyond what the Gmail original message view and PhishTool provided.  
- This is a lab/test simulation — do not reuse these techniques against real people or organizations.



