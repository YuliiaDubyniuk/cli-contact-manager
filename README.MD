# 📒 CLI Contact Book Manager

A command-line based contact book application built with Python. This tool allows you to store, retrieve, update, and delete contact information including phone numbers and birthdays. It also supports birthday reminders for the upcoming 7 days.

---

## ✅ Features

- Add new contacts with phone numbers
- Edit and remove phone numbers
- Add and view birthdays
- Delete entire contact entries
- Show all saved contacts
- Find upcoming birthdays within the next 7 days
- Persistent storage using `pickle`
- Input validation and user-friendly error messages
- Easy-to-use CLI interface

---

## 🚀 How to Use

### 🔧 Run from Python Script

1. Clone or download the repository.
2. Open your terminal and navigate to the project folder.
3. Run the script:
   ```bash
   python contacts_manager.py
   ```
4. Optional: Specify a custom file for saving contacts:
   ```bash
   python contacts_manager.py --file path/to/your/contactbook.pkl
   ```

### 💻 Run as Executable

The project is built using `pyinstaller`, so you can run the standalone executable:

```bash
cli_contact_manager.exe
```

You can optionally provide a custom file path where contacts will be stored:

```bash
cli_contact_manager.exe --file path\to\your\contactbook.pkl
```

Alternatively, you can simply double-click the executable `cli_contact_manager.py`.

> ⚠️ **Default Save Location:**  
> If no file is specified, contacts will be saved to  
> **`<your home directory>\contactbook.pkl`**

---

## ⚙️ Requirements

Python 3.10+

(Optional for building executable) PyInstaller

---

## 💬 Available Commands

| Command                                 | Description                                                                 |
| --------------------------------------- | --------------------------------------------------------------------------- |
| `hello`                                 | Greets the user.                                                            |
| `add <name> <phone>`                    | Adds a phone number to a contact (creates the contact if not exist).        |
| `change <name> <old_phone> <new_phone>` | Updates a contact's phone number.                                           |
| `remove <name> [phone]`                 | Removes a phone number or deletes the entire contact if phone is not given. |
| `phone <name>`                          | Shows phone numbers for a given contact.                                    |
| `add-birthday <name> <DD.MM.YYYY>`      | Adds a birthday to the contact.                                             |
| `show-birthday <name>`                  | Displays the birthday of a contact.                                         |
| `birthdays`                             | Shows contacts with birthdays in the next 7 days.                           |
| `all`                                   | Lists all contacts with details.                                            |
| `exit` / `close`                        | Saves and exits the program.                                                |
