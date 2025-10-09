---
class: cse
title: 05 Describe the following Linux commands
course: Embedded System Programming
chapter:
  - "ch6: WWW, Kernel, ASP"
semester: 6th
date: 2025-09-13
status: pending 🛑
tags:
  - board_2021
  - board_2022
---
Describe the following Linux commands: #board_2021 #board_2022 

- `mkdir` #board_2021 #board_2022 
- `touch` #board_2021 #board_2022 
- `cat` #board_2022 
- `ping` #board_2021 #board_2022 
- `CP` #board_2022 
- `head` #board_2021 
- `rm` #board_2021 

---

**Here are the explanations of the listed Linux commands:**

- **`mkdir` (Make Directory)** – The `mkdir` command is used to create new directories in the Linux file system. Directories act like folders that help organize files. You can create a single directory or multiple directories at once. For example, `mkdir project` creates a directory named _project_ in the current location, while `mkdir project1 project2` creates two directories together.
    
- **`touch`** – This command is often used to create an empty file, but it also updates the access and modification timestamps of an existing file without changing its content. For example, `touch notes.txt` creates an empty file named _notes.txt_. If _notes.txt_ already exists, it simply updates its last modified time.
    
- **`cat` (Concatenate)** – The `cat` command is one of the most commonly used commands for viewing, creating, and combining files. For example, `cat file.txt` displays the content of _file.txt_. You can also use it to create files (`cat > newfile.txt`) or to merge multiple files into one (`cat file1 file2 > merged.txt`).
    
- **`ping`** – The `ping` command checks the connection between your system and another host (like a server or website). It sends small packets of data and measures how long it takes for the response to return. This helps diagnose network issues and test internet speed or availability. For example, `ping google.com` sends continuous requests to Google’s server and shows the response time.
    
- **`cp` (Copy)** – This command copies files and directories from one location to another. You can also use options like `-r` to copy directories recursively. For example, `cp file1.txt backup/` copies the file _file1.txt_ into the _backup_ directory. To copy entire folders, `cp -r project/ backup/` copies all files inside _project_ to _backup_.
    
- **`head`** – The `head` command displays the first 10 lines of a file by default, which is useful for quickly previewing large files. You can customize the number of lines with the `-n` option. For example, `head log.txt` shows the first 10 lines of _log.txt_, while `head -n 5 log.txt` shows only the first 5 lines.
    
- **`rm` (Remove)** – The `rm` command deletes files or directories. For safety, Linux does not move files to a recycle bin — once deleted, they are permanently gone. For example, `rm old.txt` removes _old.txt_, and `rm -r folder` deletes the folder and all its contents. If you want confirmation before deletion, you can use `rm -i filename`.