# Reading from a file


## PERL

~~~~~~~~
#!/usr/bin/perl
open(IN,"filename");
$_=<IN>;
while(<IN>)
{
	print $_;
}
close(IN);
~~~~~~~~


## python

~~~~~~~~
#!/usr/bin/env python
f = open('filename', 'r')
line = f.readline()
print line
~~~~~~~~


## GO

~~~~~~~~
package main
import ( "bufio"
         "fmt"
         "os")

func main() {

    file,err := os.Open("b.go")
   if err != nil {}

 scanner :=     bufio.NewScanner(file)
    scanner.Scan()
    fmt.Println(scanner.Text())
}
~~~~~~~~
