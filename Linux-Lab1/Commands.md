### 1. User Identity
- whoami - Displays the currently logged-in user.
- id     - Displays user ID (UID), group ID (GID), and group memberships. Allows you to check what permissions that user has

### 2. Current Location
- pwd -Prints the current working directory.

### 3. Listing Files and Directories
- ls      - Lists files and directories.
- ls -l   - Long listing with permissions, owner, size, and timestamps.
- ls -a   - Shows hidden files.
- ls -la  - Commonly used combination.

### 4. Navigating the Filesystem
- cd /         - Move to root directory.
- cd ~         - Move to home directory.
- cd ..        - Move one directory up.
- cd /var/log  - Navigate directly to a directory.

### 5. Important Linux Directories
- /           -> Root filesystem
- /home       -> User home directories
- /etc        -> Configuration files
- /var/log    -> System logs
- /bin        -> Essential commands
- /tmp        -> Temporary files

### 6. Creating Files and Directories
- mkdir day1-practice - create a directory
- cd day1-practice    - enter the directory which is created
- touch file1.txt     - create a file in the newly created directory

### 7. Viewing File Contents
- cat file1.txt      - view contents in the newly created file
- less /etc/passwd   - Safely views large files with scrolling.
- head /etc/passwd   - Displays first 10 lines of a file.
- tail /etc/passwd   - Displays last 10 lines of a file.

### 8. Copying, Moving, and Deleting Files
- cp file1.txt file2.txt     - Copies a file.
- mv file2.txt renamed.txt   - Renames a file.
- rm renamed.txt             - Deletes a file.
- rm -r day1-practice        - Deletes a directory recursively .

### 9. Help and Documentation
- man ls     - Opens the manual page for a command.
- ls --help  - Displays quick help options.

### 10. Terminal Utilities
- clear      - Clears the terminal screen.
- history    - Displays command history.
- Ctrl + C   - Stops a running command.
