# Level 1 - Rules of the Game


We will first learn how to write simple programs to print
short messages on the screen. We will start with python 
and then proceed to GO and PERL.


## Python

The python code is shown below. If you are using the online
tool at http://coding4medicine.com/code, you do not need
to include the first line (#!/usr/bin/env python) of the
code below. If you are testing it in a linux computer,
write the code in file (e.g. 'hello.py') using the
nano editor, save it and then run it by typing './hello.py'
from the command line.

~~~~~~~~
#!/usr/bin/env python

#
# The command 'print' is used to print a line.
#

print "Welcome to the class"

~~~~~~~~

Let me explain how the above code works. In python, the first line of the code 
starts with the '#!' sign, followed by a command that finds the location of the python 
executable in the computer.  This is the convention used by all scripting languages in
unix/linux including python, and you can simply copy the line in your new code.

The script runs by starting from the first line and continuing
line by line until reaching the end of the script. From second line
onward, if any sentence contains the character '#', all texts right of 
that character are ignored. 

The computer ignores all empty lines, and therefore, the first statement, 
where it is asked to do something, is the fifth line.  The word 'print' 
is a python instruction that tells the computer to print the following text.
If the above scrpit is run by typing -

~~~~~~~~
./hello.py
~~~~~~~~

the computer will print the message in the screen. Python adds a newline
after completing every 'print' command.


In python, the text following 'print' command can also be broken into multiple
words separated by commas.

~~~~~~~~
#!/usr/bin/env python

print "Hello, ", "my name ", "is Alice"

~~~~~~~~




## GO


The GO program is shown below -

~~~~~~~~
package main
import "fmt"
func main() {
    fmt.Println("Hallo, ich heiße  Alice")
}
~~~~~~~~


To run  -

~~~~~~~~
go run hello.go
~~~~~~~~


Skeleton  -

~~~~~~~~
package main
import "fmt"
func main() {

}
~~~~~~~~

## PERL

The PERL code is shown below. You can write it in any file (e.g. 'hello.perl')
by using the nano editor.

~~~~~~~~
#!/usr/bin/perl

# This is a simple program

print "Hello, my name is Alice\n";
~~~~~~~~

Let me explain how the above code works. In PERL, the first line of the code 
starts with the '#!' sign, followed by the full location of the PERL executable 
in the computer.  This is the convention used by all scripting languages in
unix/linux including python and you can simply copy the line in your new code.

The script runs by starting from the first line and continuing
line by line until reaching the end of the script. From second line
onward, if any sentence contains the character '#', all texts right of 
that character are ignored. 

The computer ignores all empty lines, and therefore, the first statement, 
where it is asked to do something, is the fifth line.  The word 'print' 
is a PERL instruction that tells the computer to print the following text.
If the above script is written in 'hello.perl', run by first turning 
it into an executable file -

~~~~~~~~
chmod +x hello.perl
~~~~~~~~

and then by typing -

~~~~~~~~
./hello.perl
~~~~~~~~

You will see the computer print the message "Hello, my name is Alice" on the screen.

In PERL, the text following the 'print' command can also be broken into multiple
words separated by commas. For example, the following program will print
identical text on the screen as the previous one.

~~~~~~~~
#!/usr/bin/perl

print "Hello, ", "my name ", "is Alice\n";

~~~~~~~~


