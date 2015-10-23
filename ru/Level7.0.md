# Level 7 - Functions

## PERL

~~~~~~~~
#!/usr/bin/perl

sub name  {
my($name)=@_;
print "My name is $name\n";
}

name('Alice');
name('John');
~~~~~~~~


## Python

~~~~~~~~
#!/usr/bin/env python

def name(str):
     print "My name is", str
     return

name("Alice")
name("John")
~~~~~~~~

## GO

~~~~~~~~
package main
import "fmt"

func name(x string) {
fmt.Printf("My name is ")
fmt.Printf(x)
fmt.Printf("\n")
}
func main() {
        name("Alice")
        name("John")
}
~~~~~~~~
