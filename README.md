# 🔐 Chrome Password Extractor

This Python-based tool is an executable file capable of extracting saved passwords stored in the **Google Chrome browser** on a Windows system. It securely retrieves login credentials (usernames and passwords) and exports them into a structured **CSV file** for analysis, backup, or auditing purposes.

---

## 📁 Output

- The tool generates an output file named: `output.csv`
- This file contains two columns:
  - **Website/ID**
  - **Password**

---

## ⚙️ How It Works

Chrome stores saved passwords in a local SQLite database (`Login Data`) and encrypts them using the Windows Data Protection API (DPAPI). This tool:
1. Accesses Chrome's local password storage.
2. Decrypts the encrypted passwords using system credentials.
3. Exports the data into a readable `.csv` file.

---

## 🧰 Built With

- **Python 3.x**
- **sqlite3** – to interact with Chrome’s internal database.
- **cryptography / win32crypt** – to decrypt stored passwords.
- **csv** – for exporting data.

---

## 📦 How to Use

> ⚠️ This tool is for **educational and authorized auditing purposes** only. Use it responsibly.

1. Clone or download the repository.
2. Install the required libraries:
   ```bash
   pip install cryptography pywin32
