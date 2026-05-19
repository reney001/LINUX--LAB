# Linux Lab — File Management

## Part 1 — File Management
- Created devops-project folder structure

![image alt](https://github.com/reney001/LINUX--LAB/blob/e9e53634ef81329081826e9d572af20eee3a65a1/Snipaste_2026-05-18_20-28-27.png)

- Created logs, backups, scripts, configs, temp folders

![image alt](https://github.com/reney001/LINUX--LAB/blob/883df567c9ab3f497301a0315149335f5f2dd7d1/Snipaste_2026-05-18_20-33-09.png)


## Part 2 — File Viewing & Log Investigation
-adding sample content 

![image alt](https://github.com/reney001/LINUX--LAB/blob/f375820b4eb391c6d681a754d0240a9b02da3b62/Snipaste_2026-05-18_20-39-24.png)

- Used grep to find ERROR and WARNING entries
- Used tail -f to monitor logs live

## Part 3 — Permissions & Ownership

### Task 7 — Script Permissions
- Made deploy.sh executable using chmod +x
- Command used: chmod +x scripts/deploy.sh

### Task 8 — Secure Config File
- Secured app.conf so only owner can read and write
- Command used: chmod 600 configs/app.conf

### Task 9 — Permission Explanations

755 — Owner can read, write and execute. Group and others can read and execute only.
Used for folders and scripts.

644 — Owner can read and write. Group and others can read only.
Used for regular files like text and config files.

600 — Owner can read and write only. Nobody else has any access.
Used for sensitive files like passwords, SSH keys and config files.


