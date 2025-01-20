# 📜 Doc Seed Parser v2.2

## 🔍 Description
This program searches for **phrases and private keys** inside various document formats (`doc`, `docx`, `xls`, `pdf`) and images (extracting **QR codes**). After detecting a phrase, it **generates multiple cryptocurrency addresses** and logs them in a dedicated folder.

---

## 🚀 Installation Guide

### 1️⃣ Install Python
Download and install **Python** (version **3.8 or higher**) from the official website:  
🔗 [Python Download](https://www.python.org/)

During installation:
- ✅ **Check** "Install Launcher for all users"
- ✅ **Check** "Add Python3.8 to PATH"
- ✅ **Select** "Disable Path length limit" at the end of the installation.

### 2️⃣ Install Build Tools  
Download and install **Visual C++ Build Tools**:  
🔗 [Visual C++ Build Tools](https://visualstudio.microsoft.com/visual-cpp-build-tools/)  

📷 Screenshot Guide:  
![Install Guide](https://prnt.sc/XUQAJLvWtrU-)

### 3️⃣ Install Required Libraries
Run the following command to install dependencies:
```sh
pip install -r requirements.txt
```

---

## ⚙️ Configuration

All settings are stored inside **`doc_seed_parser_v2.2.py`**.

### 🔹 **Specify the path to logs**
```python
SOURCE_DIR = 'd:/__dd2/'
```
📌 **Windows users**: Use `/` instead of `\` in paths.

### 🔹 **Enable/Disable Ethereum private key parsing**
```python
PARCE_ETH = False
```
If enabled (`True`), **set up exclusion files and folders** to prevent collecting excessive data.

### 🔹 **Blacklist unwanted folders**
```python
BAD_DIRS = ['ololololz']
```
Files inside these folders will **not** be scanned.

### 🔹 **Blacklist unwanted files**
```python
BAD_FILES = ['ololololo']
```
These filenames will be **ignored**.

### 🔹 **Define seed phrase lengths**
```python
WORDS_CHAIN_SIZES = {12, 15, 18, 24}
```
It is recommended to keep **all supported values**.

### 🔹 **Filter out duplicate phrases**
```python
EXWORDS = 2
```
Phrases with **more than 2 repeated words** will be skipped.

---

## ▶️ Running the Script

To run the script **easily**, use `Run.bat`:
1. Open `Run.bat` in a text editor.
2. Locate the following line:
   ```bat
   cd C:\Users\administrator\Desktop\seed_parser_v2.2
   ```
3. Replace the path with the **folder containing the script**.
4. **Double-click** `Run.bat` to execute the script.

---

✅ **Done!** The program will now search for phrases and generate addresses automatically. 🚀  
