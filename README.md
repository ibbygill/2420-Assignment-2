# 2420-Assignment-2

## Overview
This repository contains two scripts. The first script installas the essential software packages and creates symbolic links to the configuration files. The second script is to automate the process of creating a new user on the system. Now I will go in-depth to each of the scripts. 

## Project 1
### Requirements
    The script must be run with sufficient privileges (e.g., as root or with sudo).
### Usage
1. **Clone the Repository:**
```
git clone <repository-url>
cd <repository-directory>
```
2. **Run the Scripts**
```
cd project1
sudo bash ./install
```
This will create run the install packages which will install the user-defined packages inside of the .txt provided.

3. **Run Symlink Script**
```
sudo bash ./symlink
```
- This will create the symbolic links for the `bin` directory to `~/bin`, along with the `config` into the `~/.config` and same with the `bashrc` to your `~/.bashrc`

All of the code is explained inside of the actual scripts if you want to do more research.

## Project 2
### Requirements
    The script must be run with sufficient privileges (e.g., as root or with sudo).
### Usage
1. **Run the New User Script**
```
cd project2
sudo bash ./new-user -u <username> -p <password>
```

I've already hard-coded the specific shell we want to use, in this /bin/bash

2. **Functionality**
- Creates a new user with a group matching their username, sets the specified shell, creates a home directory and copies the contents from /etc/skel and using chpasswd to set the password for the new user. Instead of the existing tools for creating a new user.


## References

https://www.cyberciti.biz/faq/understanding-etcshadow-file/

https://gitlab.com/cit2420/2420-notes-f24/-/blob/main/2420-notes/week-three.md

https://gitlab.com/cit2420/2420-notes-f24/-/blob/main/2420-notes/week-four.md

https://gitlab.com/cit2420/2420-notes-f24/-/blob/main/2420-notes/week-five.md

https://gitlab.com/cit2420/2420-notes-f24/-/blob/main/2420-notes/week-six.md

https://gitlab.com/cit2420/2420-notes-f24/-/blob/main/2420-notes/week-seven.md

https://gitlab.com/cit2420/2420-notes-f24/-/blob/main/2420-notes/week-nine.md

https://www.youtube.com/watch?v=tQ9VDxCmiKk

https://www.geeksforgeeks.org/awk-command-unixlinux-examples/

https://www.golinuxcloud.com/linux-list-users-examples/

https://www.reddit.com/r/linux/comments/1hfjgl/pulling_uidgid_values_from_active_directory/