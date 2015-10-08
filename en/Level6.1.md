# K-mer counting


~~~~~~~
#!/usr/bin/perl

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

$N=1;

foreach $key (keys(%gene))
{
        $seq=$gene{$key};
        for($i=0; $i<=length($seq)-$N; $i++)
        {
                $sub=substr($seq,$i,$N);
                print "$sub\n";
        }
        $seq=reverse($seq);
        $seq=~s/A/X/g; $seq=~s/T/A/g; $seq=~s/X/T/g;
        $seq=~s/C/X/g; $seq=~s/G/C/g; $seq=~s/X/G/g;

        for($i=0; $i<=length($seq)-$N; $i++)
        {
                $sub=substr($seq,$i,$N);
                print "$sub\n";
        }
}
~~~~~~~

~~~~~~~
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


print(gene)

f=open('num','r')
lines=f.readlines()

for x in lines:
        y=int(x)
        print y+1
~~~~~~~

