# Writing into a file  -

## python

~~~~~~~~
#!/usr/bin/env python

f = open('myfile', 'w')

f.write("hi, my name is john\n")
~~~~~~~~

## GO

~~~~~~~~
package main
import  "os"

func main() {
file,err := os.Create("myfile")
if(err!=nil) {}

file.WriteString("hi, my name is john\n")
}
~~~~~~~~

## PERL

~~~~~~~~
#!/usr/bin/perl

open(OUT,">myfile");
print OUT "My name is john\n";
close(OUT);
~~~~~~~~

