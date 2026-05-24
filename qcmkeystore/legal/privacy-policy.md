# Privacy Policy — Qcm Locker

**Last updated: 2026-05-24**

This Privacy Policy explains how QmakerTech ("we", "us", "our") collects, uses, and
protects information when you use **Qcm Locker** (package: `com.qmaker.qcm.keystore`),
an Android application that lets quiz authors create locks, generate PassCodes, and
protect `.qcm` quiz files.

By using Qcm Locker you agree to the practices described in this policy.

---

## 1. Who We Are

Qcm Locker is developed and operated by **QmakerTech**.  
Contact: contact@qmakertech.com

---

## 2. Data We Collect

### 2.1 Google Account Information

Qcm Locker requires a Google account to sign in. When you authenticate we receive
from Google:

| Data | Purpose |
|---|---|
| Display name | Identify your account in the app |
| Email address | Uniquely associate locks and PassCodes with your account |
| Profile photo URL | Display your avatar in the navigation drawer |

We do not receive your Google password.

### 2.2 Lock Data

When you create or edit a lock, the following information is sent to and stored on
QcmKeyStore servers operated by QmakerTech:

| Data | Purpose |
|---|---|
| Lock name | Display and identify the lock |
| Lock password (encrypted) | Protect the content of `.qcm` files |
| Expiration date (optional) | Enforce time-limited access |
| Usage limit (optional) | Limit the total number of allowed uses |
| Multi-owner setting | Control whether a PassCode may be used by multiple devices |
| Creation date | Sort and display locks in the home list |

### 2.3 PassCode Data

When you generate PassCodes, the following is stored on QcmKeyStore servers:

| Data | Purpose |
|---|---|
| PassCode values | Distributed to authorized users to unlock protected quizzes |
| Usage count | Track how many times each code has been used |
| Per-code expiration (optional) | Enforce time-limited codes |
| Per-code usage limit | Limit the number of uses per code |

### 2.4 Quiz File Access

When you tap **Protect a .qcm file**, Qcm Locker reads the source `.qcm` file you
select and writes the protected output file to your device storage. This processing
happens entirely **on your device**. The quiz file content is never uploaded to
QmakerTech servers.

### 2.5 Data We Do Not Collect

Qcm Locker does **not** access or collect:

- Location data
- Camera or microphone
- Contacts or call logs
- Device identifiers beyond what Firebase Authentication requires

---

## 3. How We Use Your Data

| Data | Use |
|---|---|
| Google account info | Authenticate you and associate your locks with your account |
| Lock and PassCode data | Provide the QcmKeyStore service — validate PassCodes when a reader opens a protected file |
| File access | Protect quiz files locally on your device |

We do not sell, rent, or share your personal data with third parties for marketing
purposes.

---

## 4. Third-Party Services

### Google Sign-In / Firebase Authentication

Authentication is handled by **Firebase Authentication**, a Google service. When you
sign in, your data is processed according to:

- [Google Privacy Policy](https://policies.google.com/privacy)
- [Firebase Terms of Service](https://firebase.google.com/terms)

### QcmKeyStore

Lock and PassCode data is stored on **QcmKeyStore**, a backend service operated
exclusively by QmakerTech. No third party has access to this data.

---

## 5. Data Retention

| Data | Retention |
|---|---|
| Google account info | Managed by Google; we retain only what Firebase Authentication provides per session |
| Lock data | Retained until you disable the lock or request deletion |
| PassCode data | Retained until the associated lock is disabled or you request deletion |
| Protected `.qcm` files | Stored only on your device; we have no copy |

---

## 6. Data Security

Lock passwords are stored encrypted on QcmKeyStore servers. Access to the service
requires a valid Google authentication token. We apply industry-standard security
practices to protect data in transit (HTTPS) and at rest.

---

## 7. Your Rights

You have the right to:

- **Access** the data we hold about you.
- **Delete** your locks, PassCodes, and account data at any time by contacting us.
- **Sign out** of Qcm Locker at any time via the navigation drawer.
- **Withdraw consent** by uninstalling the app and requesting data deletion.

To exercise any of these rights, contact us at: **contact@qmakertech.com**

---

## 8. Children

Qcm Locker is not directed at children under 13. We do not knowingly collect personal
data from children. If you believe a child has provided us with personal data, please
contact us and we will delete it promptly.

---

## 9. Changes to This Policy

We may update this Privacy Policy from time to time. When we do, we will update the
"Last updated" date at the top of this page. Continued use of Qcm Locker after changes
constitutes acceptance of the updated policy.

---

## 10. Contact

**QmakerTech**  
Email: qmakertech@gmail.com

---

*This policy applies exclusively to the Qcm Locker Android application
(`com.qmaker.qcm.keystore`). Other QmakerTech applications are governed by their own
privacy policies.*
