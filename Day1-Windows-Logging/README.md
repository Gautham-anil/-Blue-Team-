# 🛡️ Blue Team Learning - Day 1: Windows Logging Basics

## 📅 Date: June 24, 2025  
## 🎯 Goal:
Understand how Windows logs work, where to find them, and what common Event IDs tell us about user and system activity.

---

## 📌 Key Concepts

### 🔍 What are Windows Event Logs?
Windows Event Logs are records of system, application, and security activities. They help defenders analyze user behavior and detect suspicious events.

### 📁 Types of Logs:
| Log Type       | Description                          | Path in Event Viewer                    |
|----------------|--------------------------------------|------------------------------------------|
| System         | OS & hardware activity               | Windows Logs → System                    |
| Application    | App errors and behavior              | Windows Logs → Application               |
| Security       | Logons, logoffs, account usage       | Windows Logs → Security                  |
| Setup          | OS install and update logs           | Windows Logs → Setup                     |
| Forwarded Logs | Centralized logs from other systems  | Forwarded Events                         |

---

## 🧪 Event Viewer – How to Use:
1. Open Run (`Win + R`) → `eventvwr`
2. Go to **Windows Logs** → **Security**
3. Use **Filter Current Log...** (on the right) to search by **Event ID**

---

## 🔑 Important Event IDs

| Event ID | Meaning                        |
|----------|--------------------------------|
| 4624     | Successful user logon          |
| 4625     | Failed login attempt           |
| 4688     | New process created            |
| 1102     | Security log cleared           |
| 6005     | Event log service started      |

📄 [SANS Event ID Cheat Sheet](https://www.sans.org/media/score/checklists/windows-event-id-cheat-sheet.pdf)

---

## 📚 Tasks Completed

- ✅ Explored Windows Event Viewer
- ✅ Filtered logs by login-related Event IDs
- ✅ Read logs and noted user accounts and timestamps
- ✅ Learned about core logs: Security, System, Application

---

## 🎥 Resources Used

- [YouTube: Windows Event Logs Explained](https://www.youtube.com/watch?v=tGeC3xTQ6iE)
- [Microsoft Docs - Windows Event Viewer](https://learn.microsoft.com/en-us/windows/security/threat-protection/auditing/basic-security-auditing)

---

## 🧠 Summary

Today, I explored how to navigate Event Viewer and interpret key Event IDs related to logins, logouts, system activity, and more. These logs form the foundation for threat detection in any Blue Team environment.

---
