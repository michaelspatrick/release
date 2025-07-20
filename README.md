# Plugin Release Script

This is a Bash script to automate versioning, packaging, and GitHub release publishing for WordPress plugins.

## ✨ Features

- 🔍 Auto-detects plugin directory and filename
- 🏷  Automatically bumps version in:
  - `plugin-name.php`
  - `readme.txt` (Stable tag and changelog header)
- 📦 Builds a clean `.zip` file excluding:
  - `.git/`, `.gitignore`
  - `build/`, `release.sh`, `README.md`
  - existing `.zip` file
- 🚀 Creates or replaces GitHub tags and releases
- 🧠 Initializes a Git repository if missing
- 🔗 Prompts to add remote if not set

---

## 📦 How It Works

From your plugin root directory (where `release.sh` lives):

```bash
./release.sh 1.2.3
