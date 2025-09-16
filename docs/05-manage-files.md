
### MANAGE FILES WITH LINUX COMMANDS 

In this activity, I managed the `/home/analyst` directory and its contents by creating and removing directories, moving and deleting files, and editing a file to track changes.

---

## 1. Create a New Directory

Create a dedicated subdirectory called **logs** to store future log files:

```bash
pwd                # Print current directory
ls                 # List subdirectories
mkdir /home/analyst/logs
ls /home/analyst   # Verify logs directory was created
```
<img width="940" height="220" alt="image" src="https://github.com/user-attachments/assets/4d3c93cc-1c7d-4e53-aaf6-88bf410e5d9a" />

* `pwd` → prints the working directory.
* `ls` → lists files and directories.
* `mkdir` → creates a new directory.

---

## 2. Remove a Directory

Remove the unused `temp` directory from `/home/analyst`:

```bash
rmdir /home/analyst/temp
ls /home/analyst   # Confirm removal
```
<img width="940" height="119" alt="image" src="https://github.com/user-attachments/assets/61db6e4b-8c5b-4812-bf5e-fc870229ad53" />

* `rmdir` → removes empty directories.

---

## 3. Move a File

The file `Q3patches.txt` needs to be moved from the **notes** directory to the **reports** directory:

```bash
cd /home/analyst/notes
mv Q3patches.txt /home/analyst/reports/
ls /home/analyst/reports   # Verify move
```
<img width="940" height="163" alt="image" src="https://github.com/user-attachments/assets/76eac2f1-2bfe-4f05-914b-825cf5c280b1" />

* `cd` → changes directories.
* `mv` → moves or renames files.

---

## 4. Remove a File

Delete the unused file `tempnotes.txt` from the **notes** directory:

```bash
cd /home/analyst/notes
rm tempnotes.txt
ls /home/analyst/notes   # Confirm removal
```
<img width="940" height="116" alt="image" src="https://github.com/user-attachments/assets/e7d8c5e7-75b1-4684-9343-de47be0626fe" />

* `rm` → deletes files.

---

## 5. Create a New File

Create an empty file called `tasks.txt` inside the **notes** directory:

```bash
touch /home/analyst/notes/tasks.txt
ls /home/analyst/notes   # Confirm creation
```
<img width="940" height="124" alt="image" src="https://github.com/user-attachments/assets/335000b4-982b-4994-9230-9f01f5ff4ceb" />

* `touch` → creates a new empty file.

---

## 6. Edit a File

Use the **nano** text editor to add notes into the `tasks.txt` file:

```bash
nano /home/analyst/notes/tasks.txt
```
<img width="940" height="41" alt="image" src="https://github.com/user-attachments/assets/ec3e371b-0599-4d33-b9b7-23d752286def" />

Inside `nano`:
* Type your notes.
* Save with **CTRL+O** and exit with **CTRL+X**.

<img width="891" height="500" alt="image" src="https://github.com/user-attachments/assets/18137994-e0e8-4e91-b8f0-9459e01e43f1" />

After editing, clear the screen and confirm the contents:

```bash
clear
cat /home/analyst/notes/tasks.txt
```
<img width="940" height="150" alt="image" src="https://github.com/user-attachments/assets/c6872eea-9de3-4a70-bdc8-4e4f4787d1b4" />

* `nano` → edits files directly in the terminal.
* `clear` → refreshes the terminal window.
* `cat` → displays the file’s contents.

---

✅ **Key Takeaways**

* `mkdir` and `rmdir` manage directories.
* `mv`, `rm`, and `touch` handle files.
* `nano` allows editing files without leaving the terminal.

This exercise provided hands-on experience in **organizing directories, moving/removing files, and editing configuration or notes with `nano`**—all essential skills for Linux administration.

---

