

## ✅ **Basic Installation Commands**

| Command                           | Description                                                        |
| --------------------------------- | ------------------------------------------------------------------ |
| `pip install package`             | Install the latest version of a package.                           |
| `pip install package==1.2.3`      | Install a specific version of a package.                           |
| `pip install "package>=1.0,<2.0"` | Install a version range.                                           |
| `pip install -r requirements.txt` | Install all packages listed in a file.                             |
| `pip install --user package`      | Install in user’s site-packages directory (no admin needed).       |
| `pip install .`                   | Install a package from the current directory (for local projects). |

---

## 🔄 **Upgrade & Uninstall**

| Command                         | Description                              |
| ------------------------------- | ---------------------------------------- |
| `pip install --upgrade package` | Upgrade a package to the latest version. |
| `pip install --upgrade pip`     | Upgrade pip itself.                      |
| `pip uninstall package`         | Uninstall a package.                     |

---

## 📄 **Working with Requirements**

| Command                         | Description                                                     |
| ------------------------------- | --------------------------------------------------------------- |
| `pip freeze > requirements.txt` | Export all current installed packages into a file.              |
| `pip freeze`                    | Show installed packages with exact versions (good for backups). |
| `pip list`                      | Show all installed packages (names + versions).                 |
| `pip list --outdated`           | Show all packages with newer versions available.                |
| `pip list --uptodate`           | Show packages that are up-to-date.                              |

---

## 🔍 **Search, Info, and Help**

| Command                             | Description                                                           |
| ----------------------------------- | --------------------------------------------------------------------- |
| `pip show package`                  | Show metadata: version, location, dependencies, etc.                  |
| `pip help`                          | Show help for all pip commands.                                       |
| `pip help install`                  | Show help for a specific command.                                     |
| *(Deprecated)* `pip search keyword` | Search PyPI for matching packages (use [pypi.org](https://pypi.org)). |

---

## 🌐 **Install from Other Sources**

| Command                                              | Description                                  |
| ---------------------------------------------------- | -------------------------------------------- |
| `pip install git+https://github.com/user/repo.git`   | Install package directly from a GitHub repo. |
| `pip install https://example.com/somepackage.tar.gz` | Install from a URL or `.tar.gz` file.        |
| `pip install somepackage.whl`                        | Install a local `.whl` (wheel) file.         |

---

## 🧪 **Virtual Environment Related (important after reset)**

> Though not pip itself, these help pip work in isolated environments:

| Command                                                                               | Description                                      |
| ------------------------------------------------------------------------------------- | ------------------------------------------------ |
| `python -m venv envname`                                                              | Create a virtual environment.                    |
| `source envname/bin/activate` (Linux/macOS)<br>`.\envname\Scripts\activate` (Windows) | Activate the environment.                        |
| `deactivate`                                                                          | Exit the virtual environment.                    |
| `pip install -r requirements.txt`                                                     | Install environment packages in the virtual env. |

---

## 🛠️ **Diagnostics, Cache & Repair**

| Command           | Description                                            |
| ----------------- | ------------------------------------------------------ |
| `pip check`       | Check for broken or conflicting dependencies.          |
| `pip cache dir`   | Show pip's cache directory.                            |
| `pip cache list`  | Show cached packages.                                  |
| `pip cache purge` | Clear pip's cache.                                     |
| `pip debug`       | Show environment and configuration info for debugging. |

---

## 💡 Extra Tips

* ✅ Always use `python -m pip` instead of just `pip` if you have multiple Python versions:

  ```bash
  python3.10 -m pip install package
  ```

* 📂 To generate a backup of all installed packages **with versions**:

  ```bash
  pip freeze > requirements.txt
  ```

* 🔄 To restore them after reset:

  ```bash
  pip install -r requirements.txt
  ```

---
