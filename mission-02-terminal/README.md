# Mission 2 — Terminal and File Management

## Task / Objective

Practise navigating folders and managing files using Terminal, and understand command options and pipes.

## Task 2.1 — Basic Terminal Operations

| Command | What it does | What I observed |
|---|---|---|
| `pwd` | Displays the current folder’s full path. | The path ended with digital-detective-8452, confirming I was inside my project folder. |
| `ls` | Lists visible files and folders. | I saw my main README.md, mission folders and evidence folder. |
| `ls -l` | Lists files and folders with additional details. | I saw permissions, owner, size and modification time alongside each item’s name.|
| `cd ..` | Moves to the parent folder. | I moved from my project folder to the Desktop. |
| `cd digital-detective-8452` | Enters the project folder. | I returned to my assignment folder. |
| `mkdir terminal-practice` | Creates a new folder. | A folder named terminal-practice was created. |
| `cd terminal-practice` | Enters the practice folder. | My current path ended with terminal-practice. |
| `touch notes.txt` | Creates an empty file if it does not exist. | An empty notes.txt file was created. |
| `cp notes.txt notes-copy.txt` | Copies a file. | Both the original file and its copy existed. |
| `mv notes-copy.txt notes-backup.txt` | Renames or moves a file. | The copy was renamed to notes-backup.txt. |
| `cat notes.txt` | Displays a file’s contents. | No text appeared because the file was empty. |
## Task 2.2 — Safe File Changes

- Replacing contents with `>` removes the previous contents and writes new text.
- Appending with `>>` adds text at the end while keeping existing contents.
- Copying creates another file and keeps the original. Moving changes a file’s location or name.
- `pwd` shows which folder I am currently working in.
- `ls` helps me check which files and folders exist in that location.

### My Observation
when i used ">>" for writing a new line the previous line is not deleted the new line is continued but if i use ">" it is replaced


## Task 2.3 — Flags and Pipes

| Command | Purpose |
|---|---|
| `ls` | Lists visible files and folders. |
| `ls -l` | Shows a detailed listing. |
| `ls -la` | Shows a detailed listing including hidden entries. |
| `ls -lah` | Also displays file sizes in human-readable units. |
| `ls -l \| head -n 3` | Displays only the first three lines of the detailed listing. |

### My Observations
- 'ls' only lists the files and folders
- 'ls -l' it does what ls does but also tell the permissions,owner,group,file size in bytes,when it was last modified and its name
- 'ls -la' it does the same thing as ls -l and it also hidden files including . and ..
- 'ls -lha' it does same thing as ls -la but it tells the file size in human readable units such as M or K when appropriate
- The "ls -l" gives output to "head -n 3" as input using pipe("|") symbol. It gives the first three lines of the output

## Task 2.4 — Package Managers

A package manager helps install, update and remove software. It can also manage dependencies—the other software a program needs to work. Homebrew is a package manager commonly used on macOS.

### My Observation
homebrew was installed in my macbook its version is Homebrew 7.0.12 i got it from hombrew --version command. Brew list displays all installed software packages (both command-line formulae and GUI casks) managed by Homebrew

## My Understanding

Terminal commands let me navigate folders and manage files. Flags change a command’s behaviour: for example, `-l` adds details and `-a` includes hidden entries. A pipe sends one command’s output into another command. The `>` operator replaces a file’s contents, while `>>` adds text to the end.

## Difficulties Faced

I did not initially understand why `staff` appeared in the detailed file listing.

## How I Resolved Them

I asked for an explanation and learned that `staff` is a standard macOS group associated with the file. The listing shows both the file’s owner and its group.

## Evidence / Files

- README.md — Contains my command table, observations and explanations.
- ../terminal-practice/ — Contains the text files and backups created during practice.

## Commit Details

Planned commit message: Complete Terminal and file management mission
