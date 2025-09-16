### FILTER WITH `grep`

In this scenario, I used the `grep` command to extract information from server logs and user data files. We also combine `grep` with other commands (like `ls` and pipes '|') to filter filenames containing specific strings.

---

## 1. Search for Error Messages in a Log File

Navigated to the `/home/analyst/logs` directory and searched the `server_logs.txt` file for lines containing the word **error**:

```bash
cd /home/analyst/logs
grep "error" server_logs.txt
```


<img width="940" height="232" alt="image" src="https://github.com/user-attachments/assets/1fabaca6-5b36-4635-8a38-60beccb17318" />


✅ The `grep` command takes two arguments:

* The **string to search for** (`error`)
* The **file to search through** (`server_logs.txt`)

---

## 2. Find Files Containing Specific Strings

Navigated to the `/home/analyst/reports/users` directory and searched for filenames with particular text:

```bash
cd /home/analyst/reports/users

# List files with "Q1" in their names
ls | grep "Q1"

# List files with "access" in their names
ls | grep "access"
```


<img width="940" height="289" alt="image" src="https://github.com/user-attachments/assets/3de40d61-b072-4d2b-b55e-fa5fc9df0ca7" />


✅ Here, the **pipe character (`|`)** is used to send the output of one command (`ls`) into another (`grep`).

---

## 3. Search More File Contents

Searched inside user files for specific usernames and department information:

```bash
ls /home/analyst/reports/users

# Check deleted users for "jhill"
grep "jhill" Q2_deleted_users.txt

# Check added users for "Human Resources"
grep "Human Resources" Q4_added_users.txt
```


<img width="940" height="294" alt="image" src="https://github.com/user-attachments/assets/a097dc5b-ff6e-4798-9455-5ab67c572723" />


✅ When searching for multi-word strings like `"Human Resources"`, quotation marks are required so `grep` interprets them as one argument.

---

## Key Takeaways

This task gave practical experience in using `grep` to:

* 🔎 Search for specific information inside files.
* 📂 Find files containing specific strings when combined with other commands like `ls` and pipes (`|`).

---
