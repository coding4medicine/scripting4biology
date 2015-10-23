# Level 8 - Packages



## PERL

~~~~~~~~
#!/usr/bin/perl

use Useful;

open(IN,"gene");
$_=<IN>;

$x=Useful::translate($_);

print $x,"\n";
~~~~~~~~


## Python

~~~~~~~~
#!/usr/bin/env python

import Useful
~~~~~~~~


## GO

~~~~~~~~
package main

import ("fmt"
             "Useful")

func main() {

}
~~~~~~~~


