

### Step 1: Create the ignore file

* For Git, the ignore file is named `.gitignore`
* You create this file in your project root folder.

If you are in a terminal/command prompt, you can create it like this:

```bash
touch .gitignore
```

Or just create a new text file named `.gitignore` in your project folder manually.

---

### Step 2: Add files/folders to ignore

Open `.gitignore` in a text editor and add the files or directories you want Git to ignore.

For example:

```
# Ignore Python compiled files
__pycache__/
*.pyc

# Ignore environment variables file
.env

# Ignore folders
node_modules/
build/

# Ignore logs
*.log
```

---

### Explanation:

* `*.pyc` ignores all Python compiled bytecode files.
* `.env` ignores your environment variables file.
* `node_modules/` ignores the whole node\_modules folder.
* Lines starting with `#` are comments.

---

### Step 3: Save the `.gitignore` file.

---

### Bonus: If you want to ignore files in other contexts, examples:

* **For Docker:** create a `.dockerignore` file
* **For npm:** use `.npmignore`

---
