# OWASP Juice Shop – HACK & JUICE project

## Project Overview

This repository contains the documentation and analysis of multiple security challenges solved on **OWASP Juice Shop**.

The goal of this project is to **train, test, and improve hacking skills** by exploiting vulnerabilities aligned with the **OWASP Top 10**.

Each group member was required to solve and document **more than 10 challenges of difficulty level 3 or higher**.

---

## Objectives

- Exploit vulnerabilities across multiple OWASP Top 10 categories  
- Put real attack testing techniques into practice (manual and tool-assisted)
- Create clear and precise documents like a pro
- Be able to **explain** every solved challenge

---

## Repo Structure

All documentation files are located at the **root of the repository** and strictly follow the required naming convention:


categoryName-difficultyLevel-challengeName.md

### Examples:
- `Broken Access Control-3-CSRF.md`
- `Broken Authentication-4-Login Bjoern.md`

Invalid examples:
- `Cross Site Scripting (XSS)-CSP Bypass-4.md`
- `4_User Credentials_Injection.md`

---

## Documentation Methodology

Each .md file documents **one challenge** and contains at least the following sections:

### Methodology
- Step-by-step exploitation process
- Techniques used (OSINT, enumeration, brute force, code analysis, etc.)
- Tools involved (Burp Suite, browser dev tools, SQLMap, scripts, wordlists…)

### Vulnerability
- Vulnerability name (e.g. SQL Injection, XSS, Misconfiguration, CWE)
- Affected component (authentication, database, API, client-side logic…)
- Severity estimation (Low / Medium / High / Critical)

### Risks
- Business impact, data leakage, account takeover, reputational damage…

### Actions
- Mitigation strategies
- Secure coding recommendations
- Best practices and remediation fixes

---

## Managing documentation with Obsidian

All documentation was written using **Obsidian**, which allows for:
- All documents to be in .md format as requested
- Consistent formatting and organization
- A very simple and effective synchronization system with the git repo


