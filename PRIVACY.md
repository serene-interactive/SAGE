# SAGE Agent — Privacy Policy

**Last Updated: June 16, 2026**

SAGE is developed and operated by **Serene Interactive, Global (SiG)** ("we," "us," or "our"). This Privacy Policy explains how SAGE processes and protects your data. SAGE is a Discord-integrated AI assistant designed to prioritize user privacy and minimize data collection.

---

## Core Data Handling Principles

We operate on a **Privacy-by-Design** and **Data Minimization** framework:

1. **Ephemeral by Default:** Standard conversation prompts and responses are processed in-memory (volatile RAM) in real-time. Once the response is sent, the interaction is discarded. We do **not** log, store, or monitor your standard conversations on our servers.
2. **Volatile Session Context:** To maintain dialogue flow, SAGE retains a rolling context window of the last 20 messages. This context is kept entirely in volatile memory and is automatically wiped after 30 minutes of inactivity.
3. **No Model Training:** We do **not** use your prompts, responses, or personal data to train, fine-tune, or improve our AI models.

By default, SAGE operates in a fully ephemeral mode. If you do not explicitly opt in to the Memory feature, no user-associated conversational data is retained after your active session ends.

---

## Opt-In Memory Feature & Discord User ID

SAGE includes an optional **Contextual Memory** feature that allows the bot to remember your preferences and topics across sessions.

- **Identifiers Used:** If you choose to opt in, SAGE uses your unique **Discord User ID** (a pseudonymous snowflake identifier) to associate memory states with your account. We do not collect your real name, email, or IP address.
- **Saved Data:** The memory profile stores only high-level facts, topics, or preferences that you explicitly share (e.g., "prefers Python," "studying computer science"). It does **not** store raw chat transcripts.
- **Storage & Sharing:** This memory database is hosted privately on secure servers managed directly by SiG. This data is never shared with third parties, sold, or used for advertisement profiling.
- **Self-Service Control:** You can view, modify, or delete your memory profile at any time directly within Discord using the `/privacy` commands.

---

## Exception-Based Diagnostics & Safety Logging

To keep the service stable and secure, SAGE uses an **Exception-Based Audit Model** to track critical operational events:

### 1. What We Log (Critical Events)
We only log metadata and stack traces when a system anomaly occurs:
- **System Failures:** API timeouts, backend crashes, and execution errors (to diagnose code bugs).
- **Safety Exception Metadata:** When a prompt triggers safety filters, we log the filter category and timestamp. The original prompt text is **not** logged.
- **User Bug Reports:** If you explicitly use command triggers to report an error, the reported message and associated debug metadata are logged for human review.

### 2. Anonymization of Diagnostic Logs
All diagnostic traces are stripped of user identifiers (such as Discord User IDs and usernames) before writing to disk. They are stored under transient session IDs that do not identify a specific Discord user.

---

## Data Storage and Retention Limits

| Data Type | Stored Information | Retention Period | Storage Location |
| :--- | :--- | :--- | :--- |
| **Active Session** | Last 20 messages (in RAM) | 30 minutes of inactivity | Volatile Memory |
| **Opt-In Memory** | Facts & preferences (linked to Discord ID) | Until deleted by user (Max 30 days) | Private Database |
| **Diagnostic Logs** | Anonymized stack traces & error metadata | 7, 14, or 30 days (based on `/privacy` setting) | Secure Admin Logs |

*Note: You can configure your diagnostic retention period using the `/privacy` command. By default, all logs are permanently deleted after 7 days.*

---

## Global Regulatory Compliance

### 1. European Economic Area (EEA) & GDPR
- **Data Controller:** Serene Interactive, Global (SiG).
- **Legal Basis for Processing:** 
    - *Consent* (Art. 6(1)(a) GDPR) for storing your opt-in Memory profile.
    - *Legitimate Interest* (Art. 6(1)(f) GDPR) for real-time response generation and temporary diagnostic logging to secure service stability.
- **Data Subject Requests (DSRs):** 
    - You have the right to view, download, or delete your data. Because SAGE does not create user profiles unless you opt into the Memory feature, we can only fulfill requests related to your active **Memory profile** (linked to your Discord User ID). 
    - Since **Diagnostic Logs** are fully anonymized and stripped of user IDs, we cannot search for, verify, or delete specific error traces on request.
- **International Transfers:** All data processing occurs on secure servers located in compliant jurisdictions.

### 2. Canada (PIPEDA)
- We do not collect or disclose personal information without consent. 
- We protect your pseudonymous Discord identifier with administrative and technical safeguards matching PIPEDA standards.

### 3. Japan (APPI)
- SAGE respects the principles of the Act on the Protection of Personal Information. 
- We do not use Japanese user data for secondary purposes, and we immediately delete temporary processing traces.

---

## Your Rights and Choices

Using the `/privacy` slash commands in Discord, you can manage your data instantly:
- **`/privacy view`**: View all facts and preferences currently stored in your opt-in Memory profile.
- **`/privacy delete`**: Instantly delete your Memory profile and purge any staged diagnostic records.
- **`/privacy optout`**: Disable the Memory feature entirely (SAGE will operate in a completely stateless mode).

For further assistance, complaints, or custom data inquiries, please email us at [support@sereneinteractive.com](mailto:support@sereneinteractive.com) or contact us via our [ROSY Support Server](https://discord.gg/rosy).

---

*Serene Interactive, Global (SiG)*  
*Email: support@sereneinteractive.com*
