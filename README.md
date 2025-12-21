 Password Strength Checker

This Python script allows users to test the strength of their passwords based on multiple criteria such as length, character variety, and presence on a banned list. It provides real-time feedback on whether the password is **Strong**, **Moderate**, or **Weak**.

 Features

- Checks for minimum password length (>= 8 characters)
- Evaluates presence of:
- Uppercase letters
- Lowercase letters
- Numbers
- Special characters
- Flags passwords that appear in a list of banned or commonly used passwords
- Gives strength rating: `Strong`, `Moderate`, or `Weak`
- Rejects insecure passwords like `"password"`, `"123456"`, etc.

 How It Works

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

If a password is found in a banned list, it is rejected immediately. In my first iteration, the strong score was a 4, moderate was a 3, and weak was a 2. I edited the range to give it a more realistic evaluation for passwords. Also at first I did not have a ban list of common passowrds, and added that once I was done with the main parts of the password checker. To enhance this project even more, I could include a larger list of either common passwords or passwords that have interations of the word "password" in them. As my first project on Github, this was satisfying to complete. Testing changes for activity. 

