# password-strength-checker
A lightweight Python tool to evaluate password strength using common best-practice heuristics and entropy estimates. Works as a CLI utility and an importable library—perfect for quick audits, signup validation, or CI hooks.

📦 Installation
```
git clone https://github.com/<your-username>/password-strength-checker.git
cd password-strength-checker
# optional: create venv
python -m venv .venv && source .venv/bin/activate  # (Windows: .venv\Scripts\activate)
pip install -r requirements.txt  # empty or only for optional breach check
```
🚀 CLI Usage
```
python -m pwcheck "P@ssw0rd!"
```
🔒 Security Notes

- Never log or store real user passwords.

= For breach checks, use k-Anonymity (HIBP range API) and hash locally.

- Encourage passphrases (e.g., 4–5 random words) with separators and case/symbol variety.
