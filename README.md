# ⚡ KARMAS SUITE

**The Ultimate Automated Recon & Exploitation Toolkit**

Karmas Suite is a lightweight, highly modular offensive security framework designed for Linux and Termux/Proot environments. It automates the entire kill chain: from subdomain discovery and directory busting to secret extraction, API token spraying, WAF bypassing, and vulnerability scanning (GraphQL, IDOR, Default Creds).

Built with `curl_cffi` for Chrome TLS impersonation to bypass modern WAFs (Cloudflare, Akamai). 🚀 🦝

---

## 📦 Modules

| Module | Description |
|---|---|
| **`karmasHunter`** | Deep crawler, subdomain enumerator, directory buster, JS bundle parser, `.env` secret extractor, and HTML dashboard generator. |
| **`karmasAuth`** | API token crusher. Tests harvested tokens against endpoints and automatically attempts WAF bypasses (403s) using header manipulation. |
| **`karmasVuln`** | Vulnerability scanner. Automatically tests for GraphQL Introspection leaks, IDOR (Parameter Tampering), and Default Credentials on login forms. |
| **`karmas.py`** | The master control panel. Includes the **AUTO-CHAIN** feature which runs Hunter -> Extracts Secrets -> Feeds them to Auth. |

---

## 🚀 Installation

### Prerequisites (Termux / Proot / Linux)
You need Python 3, pip, and venv.

```bash
apt update
apt install -y python3 python3-pip python3-venv

Actor kArmasec
