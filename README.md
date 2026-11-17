# SafeBox: Secure Encrypted File Storage & Vault System

SafeBox is a secure file storage platform built on a **Zero-Knowledge Architecture**. Files are encrypted and decrypted on the client side using **AES-256**, ensuring that only the vault owner has access. Even system administrators are strictly restricted from viewing, decrypting, or downloading stored user files.

---

## 👥 Project Information

- **Institution**: American International University-Bangladesh (AIUB)
- **Course**: Software Engineering (Spring 2025–2026)
- **Supervisor**: Anik Kumar Saha

### Team Members
| Student Name | Student ID |
|:---|:---:|
| **Abu Saleh Mohammad Jaeef** | 23-52631-2 |
| **Md. Nafiz Iqbal Rohan** | 23-52646-2 |
| **Md. Al Amin** | 23-52648-2 |
| **Md. Mahmud Hasan** | 22-48894-3 |
| **Md. Tanim Hasan Priyanto** | 24-57041-1 |

---

## 🔒 Key Features

- **Zero-Knowledge AES-256 Encryption**: Client-side encryption ensures plaintext never reaches the server or database.
- **Admin Isolation**: System administrators manage accounts and view system health, but receive `403 Forbidden` if attempting to access user files.
- **Personal Vaults**: Organize files into isolated, password-protected vaults.
- **Permission-Based Sharing**: Share files with specific registered users with `View-Only` or `Download` permissions, with instant revocation.
- **Activity & Audit Logging**: Users can view their personal activity logs, while immutable system-level audit logs track administrative actions.

---

## 📐 System Design & Architecture

All system design diagrams are maintained in the [image/](image/) directory:

- **Use Case Diagram**: Defines actor boundaries and permissions between Standard Users and System Administrators. → [image/image3.png](image/image3.png)
- **Class Diagram**: Outlines domain entities (`User`, `Vault`, `SecureFile`, `SharedAccess`, `AuditLog`) and cryptographic services. → [image/image4.png](image/image4.png)
- **Activity Diagram**: Details client-side key derivation, AES-256 encryption, database storage, and audit logging. → [image/image5.png](image/image5.png)

---

## 🎨 UI Wireframes (Figma)

UI prototypes are maintained in the [image/](image/) directory:

- **Authentication**: [Login & Register](image/image6.png) | [Forgot Password](image/image7.png)
- **Vault & Files**: [User Dashboard](image/image8.png) | [Vault Explorer](image/image9.png) | [Upload Modal](image/image10.png) | [Share Modal](image/image11.png)
- **Logs & Settings**: [User Activity Log](image/image12.png) | [Profile Settings](image/image13.png)
- **Admin Governance**: [Admin Dashboard](image/image14.png) | [User Management](image/image15.png) | [Audit Log](image/image16.png)

---

## 📁 Repository Structure

```text
SE/
│
├── image/                                              # System diagrams & Figma UI mockups
│   ├── image3.png                                      # Use Case Diagram
│   ├── image4.png                                      # Class Diagram
│   ├── image5.png                                      # Activity Diagram (Upload Flow)
│   └── image6.png - image16.png                        # Figma UI Prototypes
│
├── SE - Project Report Template_Spring 25-26.docx      # Full Academic Project Report
└── README.md                                           # Project Documentation
```
