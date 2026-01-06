# 🚀 Intelligent IT Support Automation (n8n)

## 👋 Overview

This repository showcases a **realistic, production-oriented automation workflow for internal IT support**, built with **n8n** and enhanced with **AI-based classification and technical diagnosis**.

The goal is to demonstrate how repetitive IT tickets (login issues, password resets, MFA problems, access requests, etc.) can be **automatically triaged, filtered, resolved, or escalated**, while keeping human intervention only where it truly adds value.

This project is designed as a **portfolio-ready proof of concept**, with a clear and credible path toward real production integration (e.g. Active Directory, IAM, ITSM tools).

---

## 🧩 What problems this solves

### 1️⃣ Ticket overload in IT support teams
IT departments often receive **hundreds of repetitive tickets per day**, such as:
- “I can’t log in”
- “I forgot my password”
- “VPN not working”
- “Access request”

This workflow reduces noise by:
- Automatically classifying requests
- Filtering low-quality or irrelevant submissions
- Resolving common issues without human involvement

➡️ **Result:** fewer tickets, faster resolution, less burnout.

---

### 2️⃣ Poor quality requests that waste IT time
Many tickets lack:
- Sufficient technical detail
- Clear problem descriptions
- Actionable information

This workflow:
- Detects insufficient or meaningless requests
- Informs the user why the request was rejected
- Prevents ticket creation when there is nothing to act on

➡️ **Result:** cleaner queues and better user behaviour over time.

---

### 3️⃣ Misclassification of issues
In real environments:
- Users describe symptoms inaccurately
- A “login issue” may actually be a hardware problem
- “Account locked” may just mean “screen locked”

This workflow:
- Uses AI for an initial hypothesis
- Applies **technical diagnosis rules** to refine or correct the category
- Explicitly reclassifies issues when better information is available

➡️ **Result:** tickets reach the *right team* with the *right category*.

---

### 4️⃣ Over-automation risks
Blind automation in IT can be dangerous (security, access control, accounts).

This workflow avoids that by:
- Using confidence thresholds
- Forcing manual review for risky or ambiguous cases
- Never inventing system or security states

➡️ **Result:** automation is applied **only where it is safe**.

---

### 5️⃣ Lack of transparency in automated systems
Many automated systems behave like black boxes.

This workflow:
- Keeps track of original vs final classification
- Clearly indicates when an issue was auto-resolved vs escalated
- Generates traceable tickets and notifications

➡️ **Result:** automation that can be explained, audited, and trusted.

---

## ✨ Key Features

- AI-based initial issue classification
- Confidence scoring and gibberish detection
- Technical diagnosis for login-related issues
- Explicit category override based on technical findings
- Smart ticket creation logic (no useless or duplicate tickets)
- Automatic vs manual routing
- Demo mode for safe simulation
- Clear separation of responsibilities per node

---

## 🏗️ High-level Architecture

1. **Input collection** (external form / webhook)
2. **AI classification** (category + confidence)
3. **Input validation**
   - Discard invalid or meaningless requests
4. **Technical diagnosis**
   - Refines or corrects classification
5. **Category override (if needed)**
6. **Ticket creation (simulated)**
7. **Routing**
   - Automatic resolution
   - Manual IT escalation
8. **User and IT notifications**

---

## 🧪 Demo vs Production

This workflow runs in **demo mode**:
- Ticket creation is simulated
- Actions like “account unlocked” are illustrative
- No real AD / IAM systems are modified

The architecture is intentionally designed so that:
- HTTP nodes can replace simulated actions
- Real identity systems (AD, Azure AD, Okta, etc.) can be integrated
- ITSM platforms (ServiceNow, Jira, etc.) can be plugged in

---

## 💡 Why this project matters

This project demonstrates:
- Practical automation design
- Responsible use of AI in operations
- Realistic handling of edge cases
- Clear separation between AI, logic, and execution
- Production-oriented thinking (not just happy-path demos)

It reflects how **modern internal service automation is actually built** in real organisations.

---

## 🛠️ Tools & Concepts

- n8n
- AI-assisted text classification
- Rule-based technical diagnosis
- Workflow orchestration
- Conditional routing
- Automation safety patterns
- Demo-to-production design

---

## 📌 Status

- ✅ Functional demo
- ✅ Architecture validated
- ✅ Portfolio-ready
- 🔜 Production integrations (AD / IAM / ITSM)

---

## 👤 Author

Designed and implemented as a demonstration of **intelligent workflow automation for internal IT support**, with a strong focus on clarity, safety, and real-world applicability.
=======
# ai-powered-it-service-desk
AI Powered IT Service Desk
