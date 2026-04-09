🔐 Hunter – Endpoint DLP Agent (AI Data Leakage Prevention)

Hunter is a host-based Data Loss Prevention (DLP) agent designed to detect and mitigate sensitive data exposure at the endpoint level — particularly in modern workflows involving browsers and AI tools.

This project demonstrates a practical, policy-driven approach to real-time protection against clipboard-based data leaks and screenshot-to-clipboard exfiltration.

🚨 Problem

Modern data leakage often occurs through:

Copy-paste into browsers or AI tools (e.g. ChatGPT)
Screenshots containing sensitive information
Clipboard misuse across applications

Traditional security solutions do not fully address user-driven, real-time data exposure at the endpoint level.

💡 Solution

Hunter monitors endpoint activity and applies real-time protection policies to reduce the risk of sensitive data leakage.

Core capabilities:
🔍 Detects sensitive data patterns (e.g. card-like numbers)
📋 Monitors clipboard activity in real time
🖼 Detects images/screenshots entering clipboard
🧠 Context-aware monitoring (focus on high-risk applications)
🚫 Automatically clears clipboard upon detection
📝 Logs security events for audit and analysis
⚙️ How it works
User copies or generates content (text or screenshot)
Agent monitors clipboard changes
If sensitive pattern or image is detected:
Clipboard is cleared
Warning message is inserted
Event is logged
🧠 Context-Aware Security

Hunter applies stricter rules when high-risk applications are active:

Web browsers
AI tools
External communication platforms

This reflects a policy-driven approach aligned with modern endpoint security practices.

🛡️ Policy Modes
Monitor Mode – logs events only
Strict Mode – blocks sensitive clipboard content
Regulated Mode – enhanced protection for high-risk environments
📸 Demo (Coming Soon)

Example scenarios:

Copy card-like number → ❌ clipboard cleared instantly
Take screenshot → ❌ image removed from clipboard
Event logged → ⚠️ security alert generated
🧪 Current Scope (PoC)

This is a Proof of Concept (PoC) focusing on:

Clipboard monitoring
Screenshot-to-clipboard detection
Pattern-based detection
🚧 Roadmap
OCR for screenshot content analysis
Advanced pattern detection (tokens, credentials)
Improved application classification
Integration with SIEM / logging systems
Centralized policy management
⚠️ Limitations
Does not block screenshot creation at OS level
No OCR (image text recognition) yet
Runs as a user-space agent (not kernel-level)
🛠️ Tech Stack
Python
OS clipboard APIs
Pattern detection logic
Context-aware monitoring
📄 License

This project is licensed under the Mozilla Public License 2.0 (MPL-2.0).

👩‍💻 Author

Viktoriia Pivovar
Aspiring Cybersecurity Analyst | Comptia Security+ | AZ-900 | IT Specialist in Python (ITS-303)
Focused on Endpoint Security, DLP, and SOC

🤝 Contact

Open to collaboration, feedback, and entry-level opportunities in cybersecurity.

⭐ The DLP Endpoint Monitor addresses a real-world security challenge:
protecting sensitive data in an environment of constant data movement and widespread use of AI tools.
