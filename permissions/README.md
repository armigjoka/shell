README.md

What is the Shell?

Shell is an environment in which we can run our commands, programs, and shell scripts.Shell permissions

Every file and directory in your UNIX/Linux system has following 3 permissions defined for all the 3 owners discussed above.

Read: This permission give you the authority to open and read a file. Read permission on a directory gives you the ability to lists its content.

Write: The write permission gives you the authority to modify the contents of a file. The write permission on a directory gives you the authority to add, remove and rename files stored in the directory. Consider a scenario where you have to write permission on file but do not have write permission on the directory where the file is stored. You will be able to modify the file contents. But you will not be able to rename, move or remove the file from the directory.

Execute: In Windows, an executable program usually has an extension “.exe” and which you can easily run. In Unix/Linux, you cannot run a program unless the execute permission is set. If the execute permission is not set, you might still be able to see/modify the program code(provided read & write permissions are set), but not run it.

File permission commands:
1. chmod
2. su
3. sudo
4. chown
5. chgrp

Scripts for executing various shell permissions

0-iam_betty Switches the current user to the user betty.

1-who_am_i Prints the effective username of the current user.

2-groups Prints all the groups the current user is part of.

3-new_owner Changes the owner of the file hello to the user betty.

4-empty Creates an empty file called hello.

5-execute Adds execute permission to the owner of the file hello.

6-multiple_permissions Adds execute permission to the owner and the group owner, and read permission to other users, to the file hello.

7-everybody Adds execution permission to the owner, the group owner and the other users, to the file hello

8-James_Bond Sets the mode to 007 for the file hello.

9-John_Doe sets the mode of the file hello to -rwxr-x-wx

10-mirror_permissions Sets the mode of the file hello the same as olleh’s mode.

11-directories_permissions Adds execute permission to all subdirectories of the current directory for the owner, the group owner and all other users without changing regular files.

12-directory_permissions Creates a directory called my_dir with permissions 751 in the working directory.

13-change_group Changes the group owner to school for the file hello

14-change_owner_and_group Changes the owner to vincent and the group owner to staff for all the files and directories in the working directory.

16-if_only Changes the owner of the file hello to vincent only if it is owned by the user guillaume.