---

### 🔹 Inside your virtual environment

(so the packages don’t leak into your system Python)

```bash
source venv/bin/activate   # activate your venv
```

Then install packages with:

```bash
pip install <package-name>
```

Example:

```bash
pip install requests
```

---

### 🔹 Freeze dependencies (like `package.json` in Node)

You save installed packages to a file:

```bash
pip freeze > requirements.txt
```

This generates a `requirements.txt` file, e.g.:

```
requests==2.32.3
urllib3==2.2.2
```

---

### 🔹 Reinstall from `requirements.txt` (on another machine/env)

```bash
pip install -r requirements.txt
```

---

### 🔹 Upgrade a package

```bash
pip install --upgrade requests
```

---

⚡ So your workflow is:

1. `python3 -m venv venv`
2. `source venv/bin/activate`
3. `pip install <packages>`
4. `pip freeze > requirements.txt`

---