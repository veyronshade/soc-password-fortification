# 🔐 SOC Password Fortification Tool

A command-line security utility built with pure Python fundamentals that audits password strength and generates fortress-level alternatives.

## 🎯 The Problem
Most password tools are either too basic (just random characters) or too weak (allow common patterns like "password123"). Users need a tool that:
- Analyzes existing passwords for real vulnerabilities
- Generates strong passwords that are still memorable
- Uses cybersecurity terminology (relevant for SOC Analysts)

## 👨‍💻 Why SOC Analysts Need This

In a SOC environment, password policy violations are a daily alert category. 
Analysts investigate:

- **Weak passwords** in credential dumps (Have I Been Pwned, breach data)
- **Password reuse** across multiple accounts
- **Default credentials** on internal systems (admin/admin, root/password)

This tool automates the **first triage step**: score the password, flag weaknesses, 
and generate a compliant replacement. A Tier 1 analyst can run this against 
exported credentials instead of checking manually.

**Real-world parallel:** Splunk alerts for "weak password detected" → analyst runs 
this script → scores and documents → escalates if critical.

## ✅ What This Tool Does
| Feature | Description |
|---------|-------------|
| **Security Audit** | Checks length, character types, and weak patterns |
| **Scoring System** | 0–100 score with ratings: CRITICAL / MODERATE / FORTIFIED |
| **Pattern Detection** | Detects common weak strings like "123", "password", "qwerty" |
| **Fortress Generator** | Creates 20–25 character passwords using cyber-words with random case scrambling |
| **Entropy Injection** | Adds random digits and symbols, then shuffles everything |

## 🛠️ Built With
- **Python 3** — No external libraries
- **Concepts Used:** Variables, Input/Output, Type Conversion, f-Strings, Lists, Nested Lists, For Loops, Nested Loops, Random Module, Conditional Logic

## ✍️ Author
Precious Ajibola — transitioning from Civil Engineering to Cybersecurity

[LinkedIn](www.linkedin.com/in/precious-ajibola-b086ab173) | [GitHub](https://github.com/veyronshade) | [TryHackMe Profile](https://tryhackme.com/p/VeyronShade)

## 🚀 How to Run
```bash
git clone https://github.com/veyronshade/soc-password-fortification.git
cd soc-password-fortification
python3 fortify_password.py
```
