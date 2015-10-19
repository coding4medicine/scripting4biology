# Arrays

## PERL


~~~~~~~~
#!/usr/bin/perl

@A=(10, 20, 30, 40, 3);
print $A[2],"\n";
@A=();

print $A[2],"\n";
~~~~~~~~


## python

~~~~~~~~
#!/usr/bin/env python

A=[10,20,30,40,3]
print A[2]

A=[]
print len(A)
print A[2]
~~~~~~~~

## GO

~~~~~~~~
package main
import "fmt"

func main() {
  A:= [5]int{10,20,30,40,3}
  fmt.Println(A[2])
}
~~~~~~~~
