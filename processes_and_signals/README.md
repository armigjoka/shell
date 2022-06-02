README.md

Shell, processes and signals

The commands that are used on process and signal are:

0-what-is-my-pid Script that displays its own PID.

1-list_your_processes Script that displays a list of all currently running process
es, including those which may not have TTY, in a hiearchy order.

2-show_your_bash_pid Script that adds to the previous and displays lines containing the bash word.

3-show_your_bash_pid_made_easy Script that displays only the PID of the processes containing 'bash'

4-to_infinity_and_beyond Script that prints a message indefinitely every 2 seconds.
5-dont_stop_me_now Script that kills previous process.

6-stop_me_if_you_can Script that stops process using pkill command.

7-highlander Script that prints 'To infinity and beyond' indefinitely with a sleep 2 and prints 'I am invincible!!!' when it terminates.

8-beheaded_process Script that deletes highlander.

10-process_and_pid_file Creates the file /var/run/myscript.pid containing its PID, displays a message indefinitely, and does several other thing based on the signal.
11-manage_my_process Script that manages bg process manage_my_process. Either starting, stopping or restarting the other process and creating a file storing its PID.