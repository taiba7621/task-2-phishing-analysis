# Phishing Email Analysis Report

## Summary
This report analyzes a phishing email claiming to be from PayPal. It uses social engineering techniques to trick users into clicking a fake verification link.

---

## Email Details

- **From**: support@paypall.com
- **Subject**: Important - Your Account is Limited
- **Attachments**: None
- **Suspicious Links**: [Click here to verify] → Redirects to `http://malicious-verify.com`

---

##  Phishing Indicators

| Indicator                | Observed Example                  |
|--------------------------|-----------------------------------|
| Spoofed sender address   | `support@paypall.com`             |
| Suspicious domain        | `paypall.com` instead of `paypal.com` |
| Urgent language          | “Your account is limited”         |
| Header SPF failure       | SPF = fail                        |
| Link mismatch            | Text shows PayPal but redirects to malicious URL |

---

##  Header Analysis (Summary)

- **SPF**: Fail  
- **DKIM**: None  
- **DMARC**: Fail  
- **Received from**: smtp.evil.com (203.0.113.55)

---

##  Conclusion

The email is a **phishing attempt** using urgency, fake branding, and link spoofing. Users should never click suspicious links or download attachments.

---

##  Recommendations

- Always check sender address and link URLs.
- Report phishing emails to your email provider.
- Use email security tools and spam filters.
