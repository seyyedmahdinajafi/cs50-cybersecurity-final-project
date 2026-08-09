# cs50-cybersecurity-final-project
CS50's Introduction to Cybersecurity Final Project — Analysis of a March 2026 Microsoft 365 Device Code Phishing Campaign.
حتماً. این README را مستقیم در فایل `README.md` گیت‌هاب قرار بده. فقط username و لینک YouTube را بعداً جایگزین کن.

# Device Code Phishing: When MFA Is Not Enough

## CS50's Introduction to Cybersecurity — Final Project

This repository contains my final project for **CS50's Introduction to Cybersecurity**.

The project analyzes a large-scale **Microsoft 365 Device Code Phishing campaign** that occurred in March 2026 and examines how attackers abused a legitimate authentication mechanism to obtain authorized access to victims' Microsoft 365 environments.

## Project Overview

Multi-factor authentication (MFA) is an important security control, but not every authentication flow is equally resistant to phishing.

In the incident analyzed in this project, attackers used **Device Code Flow** and social engineering to convince victims to authenticate an attacker-controlled device.

The victim could complete the normal authentication process, including MFA, while unintentionally authorizing the attacker's session.

This demonstrates an important security principle:

> **Successful MFA does not necessarily mean that the entire authentication process was safe.**

## Incident

**Incident:** Microsoft 365 Device Code Phishing Campaign
**Occurrence:** March 2026
**Organizations affected:** 344
**Countries:** United States, Canada, Australia, New Zealand, and Germany

The campaign involved phishing, Device Code Authentication, OAuth tokens, Microsoft 365 resources, and post-compromise activity.

## Topics Covered

This project relates to several topics covered in CS50's Introduction to Cybersecurity, including:

* Phishing
* Social Engineering
* Authentication
* Multi-Factor Authentication
* OAuth
* Access Tokens
* Identity and Access Management (IAM)
* Authorization
* Session Security
* Network Security
* Conditional Access
* Security Monitoring
* Incident Response

## Attack Chain

```text
Phishing Message
        ↓
Malicious Landing Page
        ↓
Attacker-Generated Device Code
        ↓
Legitimate Microsoft Authentication
        ↓
Password + MFA
        ↓
Authorization
        ↓
OAuth Tokens
        ↓
Attacker Access
        ↓
Post-Compromise Activity
```

## Key Security Lesson

The attack demonstrates that security cannot depend on a single control.

A firewall can protect the network perimeter, while identity security protects authentication and authorization.

Similarly, MFA can protect an account from many credential-based attacks, but phishing-resistant authentication and additional identity controls may be necessary to defend against attacks that manipulate the authentication process itself.

## Recommended Mitigations

The project discusses several defensive measures, including:

1. Blocking Device Code Flow when it is unnecessary.
2. Using Conditional Access policies.
3. Restricting access to trusted or compliant devices.
4. Deploying phishing-resistant authentication such as FIDO2 and passkeys.
5. Improving email and URL protection.
6. Monitoring authentication and token activity.
7. Revoking compromised sessions and tokens.
8. Investigating unusual authentication behavior.
9. Maintaining user awareness and security training.
10. Applying defense-in-depth across network and identity security.

## Presentation

The final presentation is available as a PowerPoint file in the `presentation` directory.

* [PowerPoint Presentation](./presentation/Device-Code-Phishing-Final-Project.pptx)
* [PDF Presentation](./presentation/Device-Code-Phishing-Final-Project.pdf)

## Video

The final project presentation is available on YouTube as an **Unlisted** video.

**YouTube:** [Final Project Video](YOUR_YOUTUBE_UNLISTED_LINK)

## Sources

### Microsoft Security

Microsoft Security — *Inside an AI-enabled device code phishing campaign*

[https://www.microsoft.com/en-us/security/blog/2026/04/06/ai-enabled-device-code-phishing-campaign-april-2026/](https://www.microsoft.com/en-us/security/blog/2026/04/06/ai-enabled-device-code-phishing-campaign-april-2026/)

### Huntress

Huntress — *Threat Actors Abuse Railway.com PaaS as Microsoft 365 Token Attack Infrastructure*

[https://www.huntress.com/blog/railway-paas-m365-token-replay-campaign](https://www.huntress.com/blog/railway-paas-m365-token-replay-campaign)

### Huntress

Huntress — *We Need to Talk About Device Code Phishing*

[https://www.huntress.com/blog/tradecraft-tuesday-device-code-phishing-explained](https://www.huntress.com/blog/tradecraft-tuesday-device-code-phishing-explained)

### Microsoft Learn

Microsoft Learn — *Authentication flows in Microsoft Entra ID*

[https://learn.microsoft.com/en-us/entra/identity/conditional-access/concept-authentication-flows](https://learn.microsoft.com/en-us/entra/identity/conditional-access/concept-authentication-flows)

## Author

**Name:** Seyed Mehdi [Last Name]

**edX:** `[YOUR EDX USERNAME]`

**GitHub:** `[YOUR GITHUB USERNAME]`

## Course

**CS50's Introduction to Cybersecurity**

Harvard University / CS50

---

*This repository was created as part of the CS50's Introduction to Cybersecurity Final Project.*
