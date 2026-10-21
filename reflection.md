# Lab 5: Static Code Analysis — Reflection

## 1. What did you learn?
I learned that static analysis tools identify code quality, style, and security issues without executing the program. Pylint checks code quality, Flake8 checks style, and Bandit identifies common security risks.

## 2. Which issue was most important to fix, and why?
The use of `eval()` was important because it can execute unintended code when given untrusted input. I replaced it with direct salary and tax calculations. I also replaced MD5 with SHA-256 and used `secrets` for token generation.

## 3. How did the fixes improve the program?
The changes improved readability, maintainability, and security. I removed unused code, improved input validation, avoided mutable default arguments, and used safer file handling.

## 4. What were the final tool results?
Pylint scored 10.00/10, Bandit reported no issues, and Flake8 reported no violations for the revised Python file.

## 5. What challenges did you face?
I initially generated a Bandit report for the original file by mistake. I corrected the filename and reran the tools on the updated file to verify the results.

## Conclusion
This lab helped me understand how Pylint, Bandit, and Flake8 can be used to improve Python code quality, maintainability, and security.
