# Part 1: File System Navigation and Core Linux Commands
## 2a pwd — Display the present working directory
**ans** /Users/hafsatuhassanasodangi 

## b ls — List directory contents
**ans** 5102			Downloads		NetBeansProjects
Applications		Library			Pictures
Desktop			Movies			Public
Documents		Music			databaseConnection.sql

##  c. cd — Change the current directory
**ans** cd music (to change from the current directory to music directory)
hafsatuhassanasodangi@Hafsatuhassanas-MacBook-Air Music %

## d. mkdir — Create a new directory
**ans** mkdir directory_name 

## e. mdir — Remove an empty directory
**ans** sage: rmdir directory_name

## 3. Create the following directory structure in your home directory:
/home/yourusername/lab_files
ans: mkdir -p ~/lab_files

## 3.1. Inside lab_files, create two subdirectories named dir1 and dir2
**ans** lab_files % mkdir dir1 dir2

## 3.2a. Copy file1.txt from dir1 to dir2
**ans** lab_files % cd dir1 (to change from current directory which is lab_files to dir1)
- touch dir1/file1.txt (to create a file1.txt to dir1)
- dir1 % ls (to check if the file1.txt has been created)

## 3.2b. Copy file1.txt from dir1 to dir2
**ans** cp file1.txt ../dir2 

## 3.2c Rename file2.txt in dir1 to newfile.txt
**ans** touch file2.txt dir1 (to create a file2.txt to dir1) 
- mv file2.txt newfile.txt

## 3.2d Delete file3.txt from dir2
**ans** cd ../ (to go back to parent folder which lab_files since we are in dir1) 
- cd dir2 (to change directory to dir2)
- touch file3.txt dir2 (to create a file3.txt to dir2)
- rm file3.txt (to remove the file3.txt we just created)

## 3.2e Display the updated directory structure using appropriate commands
**ans** brew install tree (this is to download and install the package tree)
- tree 
.
├── dir1
│   ├── file1.txt
│   └── newfile.txt
└── dir2
    └── file1.txt

3 directories, 3 files

# Part 2:Text Editing, File Manipulation, and Shell Utilities

## 1. Using a text editor of your choice (nano, vi, or vim), create a new file named notes.txt inside the lab_files directory.
**ans** nano notes.txt

## 2. In notes.txt, write a brief reflection describing your experience using the Linux commands introduced so far.
**ans** nano notes.txt (you then go into created file to add anything)

## 3. Append an additional line containing further observations or comments.
**ans** echo "put additional line in here">> notes.txt

## 4. Display the contents of notes.txt using a command-line utility.
**ans** cat notes.txt


So far, my experience with Linux commands have been a little rough. i am still trying to understand how to move around. it is interesting though and i look forward to being very good at it.
it is important to type the correct folder name when reffering to a folder.

## 5. Create a backup copy of notes.txt named notes_backup.txt
**ans** cp notes.txt notes_backup.txt

## 6a. Create a new empty file using the touch command
**ans** touch newfile.txt

## b. Define a shell alias that lists files in alphabetical order
**ans** alias lsal='ls -1'

## c. Remove the alias using the appropriate command
**ans** unalias lsal

## d. Use the man command to view documentation for any Linux command of your choice
**ans** man ls (this lists the directory contents. press q to exit manual)

## e. Update and upgrade your Linux system using the apt package manager
**ans** brew update
- brew upgrade (using Homebrew since i am on macOs)

## f. Use the echo command to display the value of a system environment variable
**ans** echo $HOME
- /Users/hafsatuhassanasodangi

## g. View a file using the cat command
**ans** cat notes.txt (to view the contents of the file notes.txt that we created)

