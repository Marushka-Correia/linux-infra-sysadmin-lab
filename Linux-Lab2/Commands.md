### Day 2 – Linux File Permissions

I learnt that every file or folder has **three types of users**:

1. Owner – usually the person who created the file
2. Group – a team of users
3. Others – everyone else

Each of them can have these permissions:
- r -> which stands for read
- w -> write where you can either delete or edit the file
- x → execute where you can either execute the file or enter a folder/file
---

## 1) Create a a folder and a file to text commands

mkdir day2
cd day2
touch note.txt

### Commands 
A) CHECK FILE PERMISSIONS
### 1)  ls -l
output -> -rw-r--r--  sysadmin sysadmin  file1.txt

this means that
1) 1st rw -> means the owner has read and write access.
2) 2nd r -> means group has only read access
3) 3rd r-> means others have only read access.

B) ADDING/ DELETING FILE PERMISSIONS
### 2) Remove all permissions:

chmod 000 note.txt

This command means that all file permissions have been removed. and if the user tries to enter into the file/folder he will get a permission denied error message in his terminal.

### 3) chmod 644 note.txt
This command will provide read and write access to the owner, read access to group and read access to others. rw-r--r--

This was how i understood the numbers in the commands
4	read
2	write
1	execute

If you add them:

6 = read + write (4+2)

5 = read + execute (4+1)

7 = read + write + execute (4+1+2)

Always remember: 
### A directory needs execute (x) permission to enter it ####

### 4) Change owner (this is an admin task):

- sudo chown admin note.txt
