# Module 6 - Complex Programs

## Computing GC-content

~~~~~~~~
#!/usr/bin/perl

#
#
#

open(IN,$ARGV[0]);
while(<IN>)
{
        if($_=~/^>(\S+)/)
        {
                $name=$1;
                print "WARNING: duplicate name $name\n" if($gene{$name} ne "");
        }
        else
        {
                $line=$1 if($_=~/(\S+)/);
                $gene{$name} .=$line;
        }
}
close(IN);


foreach $key (keys(%gene))
{
        $seq=$gene{$key};
        $seq=~s/N//g;
        $L=length($seq);
        $seq=~s/[AT]//g;
        $r=length($seq)/$L; print "$r\n";
}

~~~~~~~



~~~~~~~~
#!/usr/bin/python3

import sys, re

f=open(sys.argv[-1],'r')
lines=f.readlines()

hre=re.compile('>(\S+)')
lre=re.compile('^(\S+)$')

gene={}

for line in lines:
        outh = hre.search(line)
        if outh:
                id=outh.group(1)
        else:
                outl=lre.search(line)
                if(id in gene.keys()):
                        gene[id] += outl.group(1)
                else:
                        gene[id]  =outl.group(1)


~~~~~~~~


