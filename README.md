## GitHub Actions Demo – Python Addition

This project demonstrates how to automate testing a simple Python addition script using **GitHub Actions**.

---

### 📂 Project Structure

```
.
├── .github/workflows
│   └── first-actions.yaml
├── src
│   └── addition.py
└── README.md
```

---

### What It Does

* `addition.py`: Contains a function to add numbers and has inline test code using `pytest`.
* `first-actions.yaml`: GitHub Actions workflow that sets up Python and runs the script through `pytest`. This GitHub Actions workflow automates the process of testing Python code whenever changes are pushed to a repository. This workflow ensures that your Python code is automatically tested with two different Python versions whenever you push changes. It helps catch bugs early and maintain code quality across environments.

---


### ▶️ GitHub Actions Workflow

This project uses a GitHub Actions CI pipeline that:

1. Triggers on every **push**.
2. Runs on `ubuntu-latest` with Python versions 3.8 and 3.9.
3. Installs dependencies like `pytest`.

4. Runs `pytest` directly on `addition.py`.


| Section                              | Screenshot                    
| ------------------------------------ | ---------------------------------------- |
| Workflow YAML in GitHub UI           | <img width="1470" height="956" alt="Screenshot 2025-07-20 at 12 05 56 PM" src="https://github.com/user-attachments/assets/9f9b2c3f-7f5c-45d7-8254-a53817ac1875" />                        |
| GitHub Actions run result | <img width="1470" height="956" alt="Screenshot 2025-07-20 at 11 39 38 AM" src="https://github.com/user-attachments/assets/24a4d29a-eea6-496e-b966-a329e9f8883b" />  |      


---


