# 🔐 Password Leak Checker using "Have I Been Pwned" API

This Python script checks if your password has ever appeared in a data breach using the [HaveIBeenPwned API](https://haveibeenpwned.com/API/v3#PwnedPasswords).

## 🚀 How It Works

- Your password is hashed using SHA-1.
- Only the **first 5 characters** of the hash are sent to the API (to maintain privacy).
- The API responds with a list of matching hash suffixes and breach counts.
- If your hash suffix is in that list, your password has been compromised.

✅ **No full password or full hash is ever sent over the internet.**

## 🛠 Requirements

- Python 3.x
- `requests` library

## 💻 How to Run

```bash
python main.py password123 mysecurepassword helloWorld@123

