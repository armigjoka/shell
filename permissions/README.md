README.md

Shell Permissions

What is the Shell?

Shell is an environment in which we can run our commands, programs, and shell scripts.

Shell permissions

Every file and directory in your UNIX/Linux system has following 3 permissions defined for all the 3 owners discussed above.

a)Read: This permission give you the authority to open and read a file. Read permission on a directory gives you the ability to lists its content.

b)Write: The write permission gives you the authority to modify the contents of a file. The write permission on a directory gives you the authority to add, remove and rename files stored in the directory. Consider a scenario where you have to write permission on file but do not have write permission on the directory where the file is stored. You will be able to modify the file contents. But you will not be able to rename, move or remove the file from the directory.

c)Execute: In Windows, an executable program usually has an extension “.exe” and which
you can easily run. In Unix/Linux, you cannot run a program unless the execute permision is set. If the execute permission is not set, you might still be able to see/modify the program code(provided read & write permissions are set), but not run it.

File permission commands:
1. chmod
2. su
3. sudo
4. chown
5. chgrp

The following are simple shell permissions commands & also some combined commands that can give faster results for the tasks in hand.


0-iam_betty (consists of the command su that is used to switch users )

1-who_am_i (whoami prints the effective username of the current user when invoked.)

2-groups (consists of command groups Groups command prints the names of the primary and any supplementary groups for each given username, or the current process if no names are given.)

3-new_owner (consists of command chown command that allows you to change the user and/or group ownership of a given file, directory, or symbolic link.)

4-empty (consists of command touch that creates a new empty file)

5-execute (consists of command chmod u+x filename to make file executable for the user.)

6-multiple_permissions (consists of command chmod u+x,g+x,o+r this command is used to give different rights to the file owner to the group and to others according all requirements)

7-everybody (consists of command chmod a+x in this case it is used to give executable rights to the file owner,group & also others.)

8-James_Bond (consists of command chmod 007 the comand here is used to give all rights to others and 0 rights to the file owner or groups.)

9-John_Doe (setting the file mode as required with the command chmod 753.)

10-mirror_permissions (consists of command chmod --reference= is used to change the mode of the file and make it the same as another chosen file.

11-directories_permissions (consists of commandschmod a+X * that adds execute permission to all subdirectories of the current directory for the owner, the group owner and all other users. )

12-directory_permissions (consists of commands mkdir -m 751 creating a directory with set permissions as required)

13-change_group (consists of command chgrp it is used to change group.)

14-change_owner_and_group (consists of command chown * that is used here to change ownership of the all files in a subdirectory)

15-symbolic_link_permissions (consists of command chown -h used in case files contain symbolic links) .

16-if_only (consists of command chown --from= that changes file ownership from one specific file owner to another .