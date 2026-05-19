# Linux Lab — File Management

## Part 1 — File Management
- Created devops-project folder structure

![image alt](https://github.com/reney001/LINUX--LAB/blob/e9e53634ef81329081826e9d572af20eee3a65a1/Snipaste_2026-05-18_20-28-27.png)

- Created logs, backups, scripts, configs, temp folders

![image alt](https://github.com/reney001/LINUX--LAB/blob/883df567c9ab3f497301a0315149335f5f2dd7d1/Snipaste_2026-05-18_20-33-09.png)


## Part 2 — File Viewing & Log Investigation
-adding sample content 

![image alt](https://github.com/reney001/LINUX--LAB/blob/f375820b4eb391c6d681a754d0240a9b02da3b62/Snipaste_2026-05-18_20-39-24.png)

-copy backup

![image alt](https://github.com/reney001/LINUX--LAB/blob/b63aac77933779d58b06354808e053dfe5f32141/Snipaste_2026-05-18_20-43-55.png)

- Used grep to find ERROR and WARNING entries
  ![image alt](https://github.com/reney001/LINUX--LAB/blob/0a73bf39a3aa2f514f0834052093afd3fef04054/Snipaste_2026-05-18_20-46-30.png)
  
- Used tail -f to monitor logs live
![image alt](https://github.com/reney001/LINUX--LAB/blob/2b99bb4b634326444e9b4613ebb1eaaa15d638a3/Snipaste_2026-05-18_20-47-19.png)
![image alt](https://github.com/reney001/LINUX--LAB/blob/6892f4ec815de78587ae8c40fd704428cfee0c12/Snipaste_2026-05-18_21-17-21.png)

## Part 3 — Permissions & Ownership

### Task 7 — Script Permissions
- Made deploy.sh executable using chmod +x

  ![image alt](https://github.com/reney001/LINUX--LAB/blob/0194066b7a1d5543958487acb135a387c3896017/Snipaste_2026-05-18_21-23-51.png)

  
- Command used: chmod +x scripts/deploy.sh
### Task 8 — Secure Config File
- Secured app.conf so only owner can read and write

  ![image alt](https://github.com/reney001/LINUX--LAB/blob/198caca0399adb14d18eb0740984b0abe6edb09f/Snipaste_2026-05-18_21-58-05.png)
  ![image alt](https://github.com/reney001/LINUX--LAB/blob/f40505b9180ad908f49fcff359513e955cd7742f/Snipaste_2026-05-18_21-59-53.png)
  ![image alt](https://github.com/reney001/LINUX--LAB/blob/6ef47d3ab4459594877861dbdd4294bafbce976c/Snipaste_2026-05-18_22-01-48.png)
  ![image alt](https://github.com/reney001/LINUX--LAB/blob/996f68143511d97a30e09450832e35ea4ac6769d/Snipaste_2026-05-18_22-03-33.png)
  
- Command used: chmod 600 configs/app.conf
  ![image alt](https://github.com/reney001/LINUX--LAB/blob/a21f5356ca497330771c7cf3f0979528c4bad2b6/Snipaste_2026-05-18_21-36-30.png)

### Task 9 — Permission Explanations

755 — Owner can read, write and execute. Group and others can read and execute only.
Used for folders and scripts.

644 — Owner can read and write. Group and others can read only.
Used for regular files like text and config files.

600 — Owner can read and write only. Nobody else has any access.
Used for sensitive files like passwords, SSH keys and config files.

 Process Management
-Start Background Process

![image alt](https://github.com/reney001/LINUX--LAB/blob/0dc5f1abe4c53c6741f6c8122d0de4d2b304b7be/Snipaste_2026-05-18_22-07-48.png)

identify process 
-finding pid and process name 
![image alt](https://github.com/reney001/LINUX--LAB/blob/6c7f4acdafa7e3353fad9081b40f1a141cbdf463/Snipaste_2026-05-18_22-09-27.png)

terminate process
![image alt](https://github.com/reney001/LINUX--LAB/blob/931d888f4db4ba5ff35e2365adfaa3832bdb14ce/Snipaste_2026-05-18_22-11-15.png)

