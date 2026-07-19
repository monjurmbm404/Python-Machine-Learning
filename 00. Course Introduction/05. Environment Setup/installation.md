# 🛠️ Machine Learning Environment Installation Guide

_A Complete Step-by-Step Installation Guide_

---

# 📖 Introduction

Before building Machine Learning models, you need a properly configured development environment.

In this guide, you will install all the software and tools required throughout this course.

By the end of this guide, you will have a fully functional Machine Learning development environment.

---

# 🎯 What You Will Install

- Python
- Visual Studio Code (VS Code)
- Git
- GitHub Account (Optional but Recommended)
- Python Virtual Environment
- Jupyter Notebook
- Required Machine Learning Libraries

---

# 🖥️ System Requirements

## Minimum Requirements

| Component        | Requirement                    |
| ---------------- | ------------------------------ |
| Operating System | Windows 10/11, Linux, or macOS |
| RAM              | 4 GB                           |
| Storage          | 5 GB Free Space                |
| Processor        | Dual Core                      |
| Internet         | Required for installation      |

---

## Recommended Requirements

| Component | Requirement                  |
| --------- | ---------------------------- |
| RAM       | 8 GB or Higher               |
| Storage   | 20 GB Free Space             |
| Processor | Intel i5 / Ryzen 5 or Better |
| Python    | Latest Stable Version        |

---

# Step 1 — Install Python

## Download Python

Download the latest stable version from the official Python website.

### During Installation

✔️ Check:

```text
☑ Add Python to PATH
```

Then click:

```text
Install Now
```

---

## Verify Installation

Open Command Prompt or Terminal.

```bash
python --version
```

or

```bash
python3 --version
```

Expected output:

```text
Python 3.x.x
```

Also verify pip:

```bash
pip --version
```

---

# Step 2 — Install Visual Studio Code

Download and install **Visual Studio Code**.

During installation, enable:

- Add to PATH
- Register Code as editor
- Open with Code

---

## Install Recommended Extensions

Open VS Code.

Go to:

```text
Extensions (Ctrl + Shift + X)
```

Install:

- Python
- Jupyter
- Pylance
- GitLens (Optional)
- Markdown All in One (Optional)
- Code Spell Checker (Optional)

---

# Step 3 — Install Git

Install Git.

Verify installation:

```bash
git --version
```

Expected output:

```text
git version 2.x.x
```

---

# Step 4 — Configure Git

Set your Git username:

```bash
git config --global user.name "Your Name"
```

Set your email:

```bash
git config --global user.email "you@example.com"
```

Verify configuration:

```bash
git config --list
```

---

# Step 5 — Create a Project Folder

Create a folder for your Machine Learning projects.

Example:

```text
Machine-Learning/
```

Open it in VS Code.

---

# Step 6 — Create a Virtual Environment

Open the terminal inside VS Code.

Create a virtual environment:

```bash
python -m venv .venv
```

A new folder will appear:

```text
.venv/
```

---

# Step 7 — Activate the Virtual Environment

## Windows

```bash
.venv\Scripts\activate
```

---

## Linux / macOS

```bash
source .venv/bin/activate
```

After activation, your terminal should look similar to:

```text
(.venv)
```

---

# Step 8 — Upgrade pip

```bash
python -m pip install --upgrade pip
```

---

# Step 9 — Install Required Libraries

Install all required packages:

```bash
pip install -r requirements.txt
```

This installs libraries such as:

- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter
- SciPy
- Joblib
- tqdm
- and other dependencies

---

# Step 10 — Verify Installed Packages

```bash
pip list
```

You should see the installed libraries listed.

---

# Step 11 — Install Jupyter Kernel

Register your virtual environment as a Jupyter kernel:

```bash
python -m ipykernel install --user --name ml-course --display-name "Python (ML Course)"
```

This allows you to select the correct Python environment inside Jupyter Notebook.

---

# Step 12 — Launch Jupyter Notebook

Start Jupyter Notebook:

```bash
jupyter notebook
```

Your default web browser should open automatically.

---

# Step 13 — Verify the Installation

Create a new notebook and run:

```python
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
import sklearn

print("Environment Setup Successful! 🎉")
```

If no errors appear, your environment is ready.

---

# Step 14 — Open the Project in VS Code

Open VS Code.

Select:

```text
File
    ↓
Open Folder
```

Choose your Machine-Learning project folder.

---

# Step 15 — Select the Python Interpreter

Press:

```text
Ctrl + Shift + P
```

Search for:

```text
Python: Select Interpreter
```

Choose the interpreter inside:

```text
.venv
```

This ensures VS Code uses the correct virtual environment.

---

# 📁 Recommended Project Structure

```text
Machine-Learning/
│
├── .venv/
├── notebooks/
├── datasets/
├── images/
├── src/
├── models/
├── README.md
├── requirements.txt
└── .gitignore
```

---

# 🧪 Environment Verification Checklist

Make sure the following commands work successfully:

```bash
python --version
```

```bash
pip --version
```

```bash
git --version
```

```bash
jupyter notebook
```

```bash
pip list
```

---

# 🚨 Common Problems & Solutions

## Python Not Found

**Error**

```text
python is not recognized...
```

**Solution**

- Ensure Python is installed.
- Reinstall Python and enable **Add Python to PATH**.
- Restart your terminal.

---

## pip Not Found

**Error**

```text
pip is not recognized...
```

**Solution**

```bash
python -m ensurepip --upgrade
```

Then verify:

```bash
pip --version
```

---

## Virtual Environment Not Activating

**Windows PowerShell**

If you encounter execution policy issues, run:

```powershell
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
```

Then activate the environment again.

---

## ModuleNotFoundError

**Error**

```text
ModuleNotFoundError: No module named 'numpy'
```

**Solution**

Activate the virtual environment and reinstall dependencies:

```bash
pip install -r requirements.txt
```

---

# 💡 Best Practices

- Use one virtual environment per project.
- Keep `requirements.txt` updated.
- Use meaningful folder names.
- Commit your code regularly with Git.
- Back up your work to GitHub.
- Avoid installing packages globally unless necessary.
- Verify your environment before starting a new project.

---

# 🎉 Congratulations!

You now have a complete Machine Learning development environment.

You are ready to:

- Write Python code
- Use Jupyter Notebook
- Analyze data with Pandas
- Perform numerical computing with NumPy
- Visualize data with Matplotlib and Seaborn
- Build Machine Learning models with Scikit-learn
- Manage your projects using Git and GitHub

---

# 🚀 Next Step

Run the provided notebook:

```text
setup-notebook.ipynb
```

This notebook will verify your installation by importing all required libraries, checking their versions, creating sample datasets, plotting basic charts, and training your first Machine Learning model.

Happy Coding! 🚀
