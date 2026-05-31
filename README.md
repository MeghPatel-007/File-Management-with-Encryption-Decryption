# 🗄️ File Manager with Encryption / Decryption
A command-line tool that allows you to create, read, edit, delete, and list files — along with encrypting and decrypting them using an extended Caesar cipher.
Built entirely in C++ using only standard libraries.

---

## 🚀 Features

### 📁 File Management
- Create new text files
- Read file contents
- Append text to existing files
- Delete files
- List files (Windows uses `dir`, Linux uses `ls`)

### 🔐 Encryption & Decryption
- Extended Caesar Cipher implementation
- Key-based dynamic shifting
- Supports:
  - Lowercase letters
  - Uppercase letters
  - Digits
  - Printable ASCII characters (33–126)
- Whitespace remains untouched
- Wrap-around logic for every character range

---

## 🛠️ Tech Stack
- **C++**
- **Standard Library (iostream, fstream, string)**

No frameworks or external dependencies.

---

## 📦 How It Works

### **1. File Operations Menu**
Users can:
- Create File
- Read File
- Edit File
- Delete File
- List Files


### **2. Encryption / Decryption**
The shift value is derived from the key:


Character handling:
- Alphabet → Rotated within alphabet
- Numbers → Rotated within 0–9
- Symbols → Rotated within ASCII 33–126
- Whitespace → Preserved
- Byte-by-byte processing

---

## 📥 How to Run

### Clone the repository
```bash
git clone https://github.com/<your-username>/<your-repo>.git
```

### Compile
```bash
g++ File.cpp -o filemanager
```

### Run
```bash
./filemanager
```

## 📌 Example Usage

Encrypt

```bash
Input  : input.txt
Output : encrypted.txt
Key    : mykey123
```

Decrypt

Use the same key to restore original contents.

## Project Structure

````bash
File.cpp      → Source code
README.md     → Documentation

````
