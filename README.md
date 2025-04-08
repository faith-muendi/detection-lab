# 🔍 Detection Lab - Identifying Suspicious SSH Logins

This project is part of my cybersecurity learning journey. The goal was to manually inspect Linux log files to identify any signs of suspicious login attempts — no scripts or coding used. Just me, the terminal, and some powerful built-in Linux tools.

---

## 🧠 What I Did
I examined the `/var/log/auth.log` file in a Linux system to find patterns that looked like brute-force or unauthorized SSH login attempts. I searched for repeated failed logins, successful logins from unknown IPs, and any other signs of suspicious activity.

---

## 🛠️ Tools Used

- **Linux Terminal**
- `cat` – for reading log files
- `grep` – for filtering specific login events
- `journalctl` – to view journal entries related to SSH
- `less` – to scroll through logs interactively
- `sort` and `uniq` – for summarizing frequent IPs or usernames

These were all command-line tools pre-installed on Linux, and I learned to combine them to spot malicious activity.

---

## 💡 What I Found

Using the commands, I noticed several failed SSH login attempts from unknown IPs. Some IPs appeared repeatedly, which suggested a possible brute-force attack. I documented all the suspicious entries in a text file (`log-output.txt`) for reference.

---

## 📦 Files in This Repo

- `log-output.txt` — Saved log entries showing failed/suspicious SSH logins
- `README.md` — You're reading it now :)

---

## 🔧 Skills Practiced

- Linux command-line navigation
- Manual log analysis
- Identifying signs of brute-force SSH attacks
- Recognizing patterns in logs using basic filtering

---

## 👩🏽‍💻 Why I Did This

As someone learning cybersecurity from scratch, I wanted to understand how security analysts detect unauthorized access. This hands-on exercise helped me build a strong foundation before moving into automated detection tools or SIEM platforms.

---

## ✅ Next Steps

- Try the same detection in Windows Event Logs
- Automate this process with Python or Bash in a future script
- Document a similar lab using SIEM tools like Splunk or Wazuh
