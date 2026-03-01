# Security Policy

## Supported Versions

We actively maintain security support for:

- Main branch (`main`)
- Latest stable releases in tags

Security fixes will be backported to supported tags when applicable.

---

## Reporting a Vulnerability

If you find a security vulnerability in this repository, please report it **privately** so that we can address it before public disclosure.

### Steps to report:

1. Create a confidential issue (if available)  
   OR  
2. Telegram:

```

https://t.me/RuslanSenatorov
https://www.youtube.com/SENATOROV

````

Please include:

- Description of the issue  
- Minimal reproducible code/sample  
- Impact assessment  
- Steps to reproduce

We will respond within 72 hours.

---

## Vulnerability Response Process

1. Acknowledge receipt within 72 hours.  
2. Triage and risk assessment.  
3. Assign severity based on CVSS criteria.  
4. Communicate acknowledgement to reporter.  
5. Fix in a dedicated branch.  
6. Release patched version with advisory.

---

## Security Best Practices

When contributing code, follow these recommendations:

### 🔹 Dependency Safety

- Avoid unvalidated third-party code  
- Keep dependencies minimal  
- Use static analysis tools

Example:

```bash
pip install safety bandit
safety check
bandit -r .
````

---

### 🔹 Input Validation

All user-facing code should validate input shapes and types.

Example:

```python
def minimize(f, grad, x0):
    assert callable(f)
    assert callable(grad)
    assert isinstance(x0, np.ndarray)
```

---

### 🔹 Sensitive Data

This repository does not handle credentials or sensitive user data.

Do not:

* Hardcode passwords
* Store API tokens in code
* Log secrets

---

### 🔹 Reporting Abuse

For critical security abuse or threats, contact:

```

https://t.me/RuslanSenatorov
https://www.youtube.com/SENATOROV

```

---

## Expected Response Time

* **Acknowledgement:** within 72 hours
* **Initial fix:** within 14 days
* **Advisory / release:** as soon as patch is verified

---

Thank you for helping keep this project secure.
