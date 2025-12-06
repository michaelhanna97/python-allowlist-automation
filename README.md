# 🐍 Python Automation – Allow List Update Algorithm

## 📌 Overview
This project demonstrates how Python can be used to securely and automatically update an **allow list** of IP addresses. The script reads an existing file containing approved IPs, removes entries found in a separate `remove_list`, and writes the updated list back to the file. This automation supports system security by ensuring outdated or unauthorized IP addresses are removed efficiently.

The workflow uses Python file handling, list manipulation, loops, conditionals, and string methods to manage and update access control data.

---

## 🗂️ Project File
- **Python-AllowList-Update-Algorithm.pdf**  
  Includes:
  - Reading files in Python using `with open()`
  - Using `.read()` to load file content
  - Converting strings into lists with `.split()`
  - Iterating through lists with `for` loops
  - Removing items using `.remove()`
  - Converting lists back to strings using `.join()`
  - Writing updated content back to a file with `.write()`
  - Explanation of read (`"r"`) and write (`"w"`) modes

---

## 🔍 Algorithm Summary

### ✔ Step 1 — Open and read the allow list  
The script opens the file in **read mode (“r”)** using:

with open(import_file, "r") as file:

ip_addresses = file.read()

This loads the file contents as a **single string**.

### ✔ Step 2 — Convert string to list  
The data is split into a list of individual IP addresses:

ip_addresses = ip_addresses.split()

This allows item-by-item removal.

### ✔ Step 3 — Iterate through the remove list  
A `for` loop cycles through each IP to be removed:

for element in remove_list:

if element in ip_addresses:

ip_addresses.remove(element)


### ✔ Step 4 — Convert updated list back to string  
Used `.join()` to prepare the data for writing:

ip_addresses = " ".join(ip_addresses)


### ✔ Step 5 — Write updated list back to file  
The file is opened in **write mode (“w”)**, replacing old data:

with open(import_file, "w") as file:

file.write(ip_addresses)

This overwrites the allow list with the cleaned version.

---

## 🛠️ Skills Demonstrated
- Python file handling (`open`, read/write modes)  
- Using `.read()`, `.write()`, `.split()`, `.join()`  
- Data cleaning and transformation  
- List iteration and conditional checks  
- Automating repetitive security tasks  
- Understanding of access control concepts  

---

## 🧩 Key Technical Concepts
### 📁 File Handling
- `"r"` → read mode  
- `"w"` → write mode (overwrites file)  
- `with open()` automatically closes the file  

### 🔁 Data Processing  
- `.split()` converts text to a list for easier manipulation  
- `.remove()` deletes specific entries  
- `.join()` rebuilds a clean string for writing  

### 🔐 Security Use Case  
This workflow automates updating an **allow list**, which is often used to control access to servers, applications, or internal systems.

---

## 📌 What This Project Shows Employers
This project demonstrates my ability to:

- Automate security-related tasks using Python  
- Manipulate files, strings, and lists effectively  
- Write clean, structured algorithms  
- Understand access control concepts  
- Document each step of the logic clearly  
- Apply Python to real-world IT and security workflows  

---

## 📌 Roles This Project Aligns With
- **Cybersecurity Analyst (Entry Level)**  
- **SOC Analyst – Tier 1**  
- **IT Support / Desktop Support (with scripting responsibilities)**  
- **Automation Technician (Junior)**  
- **Python Developer (Beginner-level scripting)**  

---

## 📬 Contact
- **GitHub Portfolio:** *https://github.com/michaelhanna97*  
- **LinkedIn:** *your LinkedIn link (optional)*  
