#### INSTALL SOFTWARE IN A LINUX DISTRIBUTION

As a security analyst, you often need to install network security tools such as **Suricata** and **tcpdump**. This tutorial walks through installing, uninstalling, and verifying these applications on a Linux system using the `apt` package manager.

---

## 1. Verify APT is Installed

APT is the package manager used for installing and removing software in Debian-based distributions (like Ubuntu and Kali Linux).

```bash
apt
```

If `apt` is installed, you’ll see usage instructions.
<img width="940" height="242" alt="image" src="https://github.com/user-attachments/assets/0d6a533e-9a36-4c0d-9079-338a9a3a82bc" />


---

## 2. Install and Uninstall Suricata

### Install Suricata

Suricata is a network analysis and intrusion detection system. To install it:

```bash
sudo apt install suricata
```
<img width="908" height="488" alt="image" src="https://github.com/user-attachments/assets/bf293b43-7b99-4067-9f2c-acd3d33f5ce4" />

After installation, confirm it works:

```bash
suricata
```

---

### Uninstall Suricata

If you want to remove Suricata:

```bash
sudo apt remove suricata
```

Check again with:

```bash
suricata
```
You should see an error saying the command is not found, which confirms uninstallation.

<img width="928" height="102" alt="image" src="https://github.com/user-attachments/assets/a898f6cd-f00a-4963-abe7-edc03d6810cc" />

---

## 3. Install tcpdump

`tcpdump` is a command-line tool for capturing and analyzing network traffic. Install it with:

```bash
sudo apt install tcpdump
```
<img width="940" height="528" alt="image" src="https://github.com/user-attachments/assets/5daf4f70-90c3-4828-bf42-a0ed39b95eaf" />

Verify installation:

```bash
tcpdump 

```
## 4. List the installed applications
The APT package manager lists the installed applications by running thsi command-line prompt 

```bash
apt list --installed
```
---
<img width="940" height="274" alt="image" src="https://github.com/user-attachments/assets/61a1e678-8679-461f-bf0a-93d4467297b4" />


✅ **Key Takeaways**

* Always verify your package manager (`apt`) is available.
* Suricata can be installed, tested, and uninstalled with `apt`.
* Tcpdump provides powerful command-line packet capture capabilities.

---
