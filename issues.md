# Lab 5: Static Code Analysis

## Tools Used
- Pylint
- Bandit
- Flake8

## Issues Found and Fixes

| No. | Original Issue | Tool | Fix Applied |
|---|---|---|---|
| 1 | Mutable default argument `transaction_logs=[]` | Pylint | Changed default to `None` and initialized the list inside the function. |
| 2 | Bare `except` with `pass` | Bandit / Flake8 | Removed the exception handler and validated inputs. |
| 3 | Use of `eval()` | Bandit | Replaced dynamic evaluation with direct salary and tax calculations. |
| 4 | Weak MD5 hash | Bandit | Replaced MD5 with SHA-256. |
| 5 | Insecure `random.randint()` for a token | Bandit | Used the `secrets` module. |
| 6 | Shell execution using `os.system()` | Bandit | Replaced with Python's `print()`. |
| 7 | Unsafe file handling | Code review | Used a context manager and UTF-8 encoding. |
| 8 | Unused imports and variables | Flake8 | Removed unused code. |
| 9 | Naming and documentation issues | Pylint | Improved naming, formatting, and docstrings. |

## Final Results

- **Pylint:** 10.00/10
- **Bandit:** No issues identified
- **Flake8:** No violations reported

## Conclusion
The revised program passed all three final static analysis checks, improving code quality, readability, and security.
