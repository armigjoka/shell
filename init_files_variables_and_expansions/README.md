README.md

Shell, init files, variables and expansions
Expansion

Each time we type a command line and press the enter key, bash performs several processes upon the text before it carries out our command.

Different types of expansions

1. brace expansion

2. tilde expansion

3. parameter and variable expansion

4. command substitution

5. arithmetic expansion

6. word splitting

7. filename expansion


Shell initialization files

A shell initialization file is a shell script that runs automatically each time the shell executes.

Shell init files are classified as below:


System-wide configuration files

/etc/profile

/etc/bashrc

Individual user configuration files


~/.bash_profile

~/.bash_login

~/.profile

~/.bashrc

~/.bash_logout

Variables

Types of variables

Global variables

Local variables

Table of commands applied:

Questions	  Commands used

0-alias		  alias ls="rm *" using an alias to attrribute ls rm* funcions

1-hello_you	  echo "hello $USER" command used to display script

2-path		  PATH=$PATH:/action Adding action to the path

3-paths		  `echo $PATH

4-global_variables	printenv command used to display environment variables

5-local_variables	set command used to display local variables

6-create_local_variable	BEST='School' script used to create a local variable

7-create_global_variable	      export BEST="School" command used to create global variable

8-true_knowledge		      echo $((128 + $TRUEKNOWLEDGE)) the commands are used to display arithmetic expansion

9-divide_and_rule		      echo $((POWER/DIVIDE)) commands used to display arithmetic expansions

10-love_exponent_breath		      echo $((BREATH**LOVE)) arithmetic expnsions

11-binary_to_decimal		      echo $((2#$BINARY)) arithmetic expansion used to convert numbers from binary to decimal

12-combinations			      `echo {a..z}{a..z}

13-print_float			      printf '%.2f\n' $NUM script that prints a number with two decimal places, followed by a new line

14-decimal_to_hexadecimal	      printf '%x\n' $DECIMAL commands used to convert a script from decimal to hexadecimal

15-rot13			      tr 'n-za-mN-ZA-M' 'a-zA-Z' commands used to decode from rot13

16-odd				      `paste - -

17-water_and_stir		      `printf '%o\n' (( 5#(echo $WATER