# 🔐 VAPT Report – Metasploitable 2

**Target:** Metasploitable 2 (192.168.56.102)  
**Attacker:** Kali Linux (192.168.56.101)  
**Environment:** VirtualBox Host-Only Network  
**Date:** April 20, 2026  
**Status:** ✅ 1.0 Final

---

## 🛡️ Executive Summary

Full Vulnerability Assessment and Penetration Testing (VAPT) exercise on Metasploitable 2 following a structured 5-phase black-box methodology. The assessment resulted in complete root-level compromise via 9 different attack vectors.

---

## 🚀 Key Achievements

- ✅ **9 successful exploits** across multiple attack vectors
- ✅ **Root access** via 3 methods – Netcat, Meterpreter, Command Shell
- ✅ **6 passwords cracked** using John the Ripper
- ✅ **Full database extraction** via MySQL and SQL Injection

---

## 🔍 Vulnerability Matrix

| Service | Vulnerability | CVE | Risk |
|---|---|---|---|
| Port 1524 (Bindshell) | Open Root Shell | N/A | 🔴 CRITICAL |
| Port 21 (vsftpd 2.3.4) | Backdoor Command Exec | CVE-2011-2523 | 🔴 CRITICAL |
| Port 6667 (UnrealIRCd) | Backdoor Command Exec | CVE-2010-2075 | 🔴 CRITICAL |
| Port 139/445 (Samba) | Username Map Script | CVE-2007-2447 | 🔴 CRITICAL |
| Port 3306 (MySQL) | No Root Password | N/A | 🟠 HIGH |
| DVWA Web App | SQL Injection | CWE-89 | 🟠 HIGH |
| DVWA Web App | Cross-Site Scripting | CWE-79 | 🟠 HIGH |
| System | Weak Passwords | CWE-521 | 🟠 HIGH |

---

## 🛠️ Tools Used

`Nmap` `Metasploit` `Netcat` `John the Ripper` `MySQL Client` `DVWA` `Kali Linux`

---

## 📄 Full Report

👉 [Download VAPT_Report_Final.pdf](./VAPT_Report_Final.pdf)

---

> ⚠️ *This project was conducted in an isolated lab environment for educational purposes only.*
