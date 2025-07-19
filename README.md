# 🔐 Password Strength Checker

This Python script allows users to test the strength of their passwords based on multiple criteria such as length, character variety, and presence on a banned list. It provides real-time feedback on whether the password is **Strong**, **Moderate**, or **Weak**.

## 🚀 Features

- ✅ Checks for minimum password length (>= 8 characters)
- ✅ Evaluates presence of:
  - Uppercase letters
  - Lowercase letters
  - Numbers
  - Special characters
- ✅ Flags passwords that appear in a list of banned or commonly used passwords
- ✅ Gives strength rating: `Strong`, `Moderate`, or `Weak`
- ❌ Rejects insecure passwords like `"password"`, `"123456"`, etc.

## 🛠️ How It Works

The script calculates a score based on the following rules:

| Criteria              | Score |
|-----------------------|-------|
| Contains a digit      | +1    |
| Contains a lowercase  | +1    |
| Contains an uppercase | +1    |
| Contains a special    | +1    |

- **Strong**: Score ≥ 5
- **Moderate**: Score of 3-5
- **Weak**: Score < 2

If a password is found in a banned list, it is rejected immediately.
