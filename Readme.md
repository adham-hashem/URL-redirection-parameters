# 🔁 URL Redirection Parameters List

This repository contains a comprehensive `.txt` list of **common URL redirection parameters** used in web applications. These parameters are often used to redirect users after authentication, form submission, or navigation — but if improperly validated, they can be exploited for **open redirect vulnerabilities**.

---

## 📂 File Structure

- `redirect-parameters.txt`: A flat list of redirection-related URL parameters, each formatted as:
?parameter=[redirect]

---

## 🛡 Use Cases

This list is ideal for:

- 🔍 **Bug Bounty hunters** — Automate fuzzing or manually test for open redirects.
- 🧪 **Security researchers** — Identify potentially unsafe redirect endpoints.
- 🛠 **Developers** — Audit your app for dangerous redirect parameter handling.
- 🤖 **Automation tools** — Feed into scanners, payload injectors, or web crawlers.

---

## 💣 Examples of Open Redirect Exploits

An attacker may craft URLs like: https://example.com/login?redirect=https://evil.com
If the server doesn't validate the redirect destination, users may be silently redirected to malicious sites.

---

## ✅ Best Practices

- Always **validate** redirect targets against a whitelist.
- Use **relative URLs** instead of absolute.
- Avoid reflecting user input into redirects without checks.

---

## 📜 License

This project is released under the [MIT License](LICENSE).

---

## 🙌 Contribute

Feel free to open a PR to expand the list or improve the formatting. Stay safe and hack responsibly!