# 🕵️‍♂️ PHISHING EMAIL FORENSICS | HEADER HUNT 🔍

> "Every email has a backstory — hidden in its headers. I just learned to read them."

## 🎯 Mission Brief

This task is a deep dive into dissecting the anatomy of a **suspicious email** — exposing hidden metadata, tracing IPs, decoding sender behavior, and detecting **phishing attempts** using **email header forensics**.

---

## 🧠 Core Objective

- Uncover potential phishing indicators from a suspicious email sample
- Leverage free tools and manual analysis to validate authenticity
- Generate a detailed threat report based on findings

---

## 🛠️ Arsenal (Tools Used)

| Tool | Purpose |
|------|---------|
| 📧 Raw Email (.eml/.txt) | Suspicious sample |
| 🛠️ [Google Header Analyzer](https://toolbox.googleapps.com/apps/messageheader/) | Decode metadata |
| 🛠️ [MXToolbox](https://mxtoolbox.com/EmailHeaders.aspx) | Trace relay servers |
| 🌐 Whois/IP Tracker | Investigate sender origin |
| 🧠 Manual inspection | Spot spoofing & inconsistencies |

---

## 🔬 Tactics Deployed

1. **Decoded** the header from the email client
2. **Traced IP hops** using `Received:` lines
3. **Analyzed sender's domain**, Return-Path, Reply-To
4. **Checked** SPF, DKIM, DMARC authenticity
5. **Scanned links/domains** for typosquatting or malicious behavior
6. **Ranked** the threat level from LOW to CRITICAL

---

## ⚠️ Red Flags Caught

| Indicator | Details |
|----------|---------|
| 🟥 SPF Check Failed | Sender's IP not listed in domain's SPF |
| 🟥 DKIM Signature Invalid | Mail content may have been altered |
| 🟥 DMARC Reject | Domain policy disallows this message |
| 🟨 Spoofed Email | Display name mismatch |
| 🟨 Suspicious Links | Obfuscated shortened URLs |
| 🟧 Unusual Send Time | Matches global spam wave timings |
| 🟩 No Attachment | Clean, but could be a phishing link trap |

---

