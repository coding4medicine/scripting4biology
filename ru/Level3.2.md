# Associative arrays

## PERL

~~~~~~~~
#!/usr/bin/perl

$A{"john"}=12;
$A{"mark"}=170;
print %A;
print $A{"john"},"\n";
~~~~~~~~

## Python

~~~~~~~~
#!/usr/bin/env python

A = {'john': 12, 'mark': 170};

print A['john']
print A
~~~~~~~~

## GO

~~~~~~~~
package main
import "fmt"
var A = map[string]int{
        "john": 12,
        "mark":170,
}
func main() {
        fmt.Println(A)
}
~~~~~~~~
