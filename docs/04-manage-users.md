ADD AND MANAGE USERS WITH LINUX COMMANDS

In this activity, I simulate adding a new employee to a Linux system, managing their group memberships, assigning file ownership, and finally removing them when they leave the company.

The example employee username is **`researcher9`**.

---

## 1. Add a New User

To add a new user to the system:

```bash
sudo useradd researcher9
```
<img width="869" height="31" alt="image" src="https://github.com/user-attachments/assets/a43db6c4-10cf-41c9-b23c-2d270fedb97b" />

Then, assigned to the **`research_team`** group as their primary group:

```bash
sudo usermod -g research_team researcher9
```
<img width="940" height="29" alt="image" src="https://github.com/user-attachments/assets/86abed29-e43c-480c-8050-7e9a0bc51037" />

* `useradd` → creates a new user.
* `usermod -g` → sets the user’s default (primary) group.

---

## 2. Assign File Ownership

Suppose the employee needs ownership of the file `project_r.txt` located in `/home/researcher2/projects/`.

```bash
sudo chown researcher9 /home/researcher2/projects/project_r.txt
```
<img width="940" height="58" alt="image" src="https://github.com/user-attachments/assets/27cc0e27-6d23-4024-a332-1d8cb52b2599" />

* `chown` → changes the ownership of files or directories.

---

## 3. Add the User to a Secondary Group

Later, the employee joins the **Sales department** and must also be part of the `sales_team` group, while keeping their primary group as `research_team`.

```bash
sudo usermod -a -G sales_team researcher9
```
<img width="940" height="28" alt="image" src="https://github.com/user-attachments/assets/100a9eb8-1162-44cd-b86a-01f48e1f3e3e" />

* `-G` → adds the user to a supplementary (secondary) group.
* `-a` → appends the user to the group list (without this, existing groups would be overwritten).

📌 *Remember: Linux is case sensitive. Group and user names must match exactly.*

---

## 4. Delete a User

When the employee leaves the company, remove their account:

```bash
sudo userdel researcher9

```
<img width="940" height="73" alt="image" src="https://github.com/user-attachments/assets/47baef65-b79d-4bc9-b956-096be6225bd5" />

After deleting the user, also remove the group created automatically with the same name:

```bash
sudo groupdel researcher9
```
<img width="940" height="70" alt="image" src="https://github.com/user-attachments/assets/d388ea76-852b-4c4f-bad7-c71f3070d781" />

* `userdel` → deletes a user account.
* `groupdel` → deletes a group (good practice to clean empty groups).

---

✅ **Key Takeaways**

* `useradd` creates a new user.
* `usermod` modifies user accounts and group memberships.
* `chown` assigns file ownership.
* `userdel` and `groupdel` remove users and groups.

Managing users is a key administrative task and an important milestone in Linux system management.

---
