# Mission 3 — Understand the Operating System

## Task / Objective

Explore how macOS manages running programs, memory, devices, files and permissions.

## Work Completed

### Task 3.1 — Explore my operating system

| Information | What I observed |
|---|---|
| Operating system | My Mac was running macOS 27.2. |
| Active account | `whoami` showed the account running my Terminal session. I recorded the name as `[redacted]`. |
| Storage | The data volume had 139 GiB used and 283 GiB available. |
| System activity | `top` showed 652 processes, with 3 running and 649 sleeping. The CPU was 84.38% idle at that moment. |

### Task 3.2 — Understand processes

A process is a running instance of a program. A PID is the number macOS uses to identify a process. I opened Safari and checked Activity Monitor. Safari had PID `66833`, and one of its helper processes had PID `66848`. This showed me that one app can use several processes.

### Task 3.3 — Understand paths and permissions

I ran `pwd` in my repository and again after running `cd terminal-practice`. The second path ended in `/digital-detective-8452/terminal-practice`. I used `cd ..` to return to the repository.

An absolute path starts at `/`. My example is `/Users/[redacted]/Desktop/digital-detective-8452/terminal-practice`. A relative path starts from the current folder. From the repository, `terminal-practice` points to that same folder.

For `notes.txt`, `ls -l` showed `-rw-r--r--@`. The owner's permission letters were `rw-`, so the owner can read and edit the file but has no execute permission. The group and others have read permission only. The `@` shows that the file has extended attributes.

### Task 3.4 — Explain operating system responsibilities

| Responsibility | My explanation and example |
|---|---|
| Process management | macOS tracks running processes and allocates CPU time to them. Safari and its helper each had their own PID. |
| Memory management | macOS manages the RAM programs use. I saw in `top` that macOS had compressed some memory. |
| Device management | macOS handles communication between hardware and apps. When I pressed a key, macOS passed the keyboard input to Terminal. |
| File management | macOS organizes and locates files and folders. I could find `notes.txt` inside `terminal-practice`. |
| User interface / shell | The operating system gives me ways to interact with the computer. I used the shell in Terminal to navigate folders and run commands. |
| Security and permissions | macOS uses file permissions to control access. The owner of `notes.txt` can edit it, while the group and others can only read it. |

## Commands / Tools Used

| Command or tool | Purpose |
|---|---|
| `sw_vers` | Display the macOS version. |
| `whoami` | Identify the active account. |
| `df -h /System/Volumes/Data` | Check the used and available space on the data volume. |
| `top -l 1 -n 0 \| head -n 8` | View a snapshot of process, CPU and memory activity. |
| Activity Monitor | Find the Safari process and read its PID. |
| `pwd` and `cd` | Check my current path and move between folders. |
| `ls -l notes.txt` | View the file's permissions. |

## My Understanding

I learned that an app can use multiple processes and that each process has its own PID. I also learned how the current folder affects relative paths and how to read the owner’s permission letters in a file listing.

## Difficulties Faced

The Terminal commands I tried for finding Safari’s PID did not give me the result I needed.

## How I Resolved Them

I used Activity Monitor to find Safari and its helper process and read their PIDs directly.

## Evidence / Files

- This README records my observations from Terminal and Activity Monitor.
- `../terminal-practice/notes.txt` is the file I inspected for permissions.

## Commit Details

- Commit message: `Document operating system and file management`
- Push status: Verified on GitHub (commit `26ccb9c`).