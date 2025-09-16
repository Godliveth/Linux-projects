### FIND FILES WITH LINUX COMMANDS 

In this activity, I used Linux commands to explore the filesystem, navigate directories, and read file contents. These skills are essential for a security analyst when investigating logs and reports.

---

## 1. Get Current Directory Information

### Display Current Directory

```bash
pwd
```
The `pwd` command (print working directory) shows the current directory path.

### List Files and Directories

```bash
ls
```

This displays the names of files and directories in the current working directory.

<img width="940" height="125" alt="image" src="https://github.com/user-attachments/assets/c21b3855-f287-417c-bcb2-e65101989cfa" />

---

## 2. Change Directory and List Subdirectories

### Navigate to `/home/analyst/reports`

```bash
cd /home/analyst/reports
```

### List Contents

```bash
ls
```
<img width="940" height="108" alt="image" src="https://github.com/user-attachments/assets/024aa6b5-7adc-4328-83bf-cce7c86e382c" />


The `cd` command changes the working directory, while `ls` lists its contents.

---

## 3. Locate and Read the Contents of a File

### Navigate to the `users` Subdirectory

```bash
cd /home/analyst/reports/users
```

### List Files

```bash
ls
```

### Display File Contents

```bash
cat Q1_added_users.txt
```

* `cat` displays the full content of a file.
* For large files, you can use `less` to view page by page.
<img width="940" height="313" alt="image" src="https://github.com/user-attachments/assets/ac8f64bf-a96a-4ba3-aac2-307c50345d62" />


## 4. Navigate to a Directory and Locate a File

### Navigate to `/home/analyst/logs`

```bash
cd /home/analyst/logs
```

### List Files

```bash
ls
```

### Display the First 10 Lines of a File

```bash
head server_logs.txt
```
<img width="940" height="393" alt="image" src="https://github.com/user-attachments/assets/f38cd129-01d1-494d-aa12-2cd17d0d6e22" />

The `head` command shows the beginning of a file (10 lines by default).
Similarly, `tail` shows the last 10 lines.

📌 **Observation:** In the first 10 lines of `server_logs.txt`, there were three (3) warning messages.

---

✅ **Key Takeaways**

* `pwd` prints the current directory.
* `cd` navigates between directories.
* `ls` lists contents of directories.
* `cat`, `head`, and `tail` are useful for reading files.

---
