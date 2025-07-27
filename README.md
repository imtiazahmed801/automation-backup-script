# 🗂️ Automated Backup Script in Python

This project is a simple Python script that automates daily backups of a specified folder to a target backup directory using the `shutil` and `schedule` libraries. Each backup is stored in a folder named with the current date.

## 📁 Features

- ✅ Daily automated backup at a scheduled time
- ✅ Backs up an entire folder recursively
- ✅ Avoids overwriting existing backups
- ✅ Easy to configure paths and schedule

## 🛠️ Requirements

- Python 3.x
- `schedule` library (`pip install schedule`)

## 💡 How It Works

1. The script defines a `source_dir` to back up and a `destination_dir` to store the backups.
2. It creates a new dated backup folder inside the destination directory.
3. It runs daily at the specified time using the `schedule` library.
4. If the backup for the day already exists, it skips to avoid overwriting.

## 🖥️ Usage

1. **Clone or download** this repository.
2. Modify the script with your own source and destination paths:
   ```python
   source_dir = "/path/to/source"
   destination_dir = "/path/to/backup"
