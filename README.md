# Password Manager (Python, tkinter, SQLite)

A desktop app that generates strong passwords and saves and looks up website logins locally.

Originally built in 2023. This repository is a clean copy that leaves out the local database file.

## Features

- Generate a strong random password (letters, digits and symbols)
- Save a website, email and password to a local SQLite database
- Search saved logins by website
- Input checks with message boxes for empty fields and missing entries

## Project structure

| File | Role |
| --- | --- |
| `main.py` | Starts the app |
| `frontend.py` | tkinter GUI (`PasswordManagerGUI`) |
| `backend.py` | SQLite storage and password generation (`PasswordManagerBE`) |

## How to run

```bash
python main.py
```

Only the Python standard library is used. The app creates `password_data.db` on first run; it is listed in `.gitignore`, so saved passwords never reach GitHub. Put a `logo.png` next to the scripts to show a logo (optional).

## Note

Passwords are stored as plain text in the local database. This is a learning project, not a production password vault.
