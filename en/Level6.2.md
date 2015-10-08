# Translating nucleotides into proteins

~~~~~~~~
#!/usr/bin/perl


$code{"AAA"}="K"; $code{"AAT"}="N"; $code{"AAC"}="N"; $code{"AAG"}="K";
$code{"TTT"}="F"; $code{"TTA"}="L"; $code{"TTC"}="F"; $code{"TTG"}="L";
$code{"CCC"}="P"; $code{"CCA"}="P"; $code{"CCT"}="P"; $code{"CCG"}="P";
$code{"GGG"}="G"; $code{"GGA"}="G"; $code{"GGT"}="G"; $code{"GGC"}="G";
$code{"ATA"}="I"; $code{"ATT"}="I"; $code{"ATC"}="I"; $code{"ATG"}="M";
$code{"TAA"}="*"; $code{"TAT"}="Y"; $code{"TAC"}="Y"; $code{"TAG"}="*";
$code{"CAA"}="Q"; $code{"CAT"}="H"; $code{"CAC"}="H"; $code{"CAG"}="Q";
$code{"GAA"}="E"; $code{"GAT"}="D"; $code{"GAC"}="D"; $code{"GAG"}="E";
$code{"ACA"}="T"; $code{"ACT"}="T"; $code{"ACC"}="T"; $code{"ACG"}="T";
$code{"TCA"}="S"; $code{"TCT"}="S"; $code{"TCC"}="S"; $code{"TCG"}="S";
$code{"CTA"}="L"; $code{"CTT"}="L"; $code{"CTC"}="L"; $code{"CTG"}="L";
$code{"GTA"}="V"; $code{"GTT"}="V"; $code{"GTC"}="V"; $code{"GTG"}="V";
$code{"AGA"}="R"; $code{"AGT"}="S"; $code{"AGC"}="S"; $code{"AGG"}="R";
$code{"TGA"}="*"; $code{"TGT"}="C"; $code{"TGC"}="C"; $code{"TGG"}="W";
$code{"CGA"}="R"; $code{"CGT"}="R"; $code{"CGC"}="R"; $code{"CGG"}="R";
$code{"GCA"}="A"; $code{"GCT"}="A"; $code{"GCC"}="A"; $code{"GCG"}="A";

open(IN,"gene");
$line=<IN>;

$count=0;

while($count<=100000)
{
        $section= substr $line, $count, 3;
        print $code{$section};
        $count=$count+3;
}
print "\n";

~~~~~~~~

~~~~~~~~
#!/usr/bin/python3

T={'TTT':'F', 'TTC':'F', 'TTA':'L', 'TTG':'L', 'TCT':'S', 'TCC':'S', 'TCA':'S', 'TCG':'S', 
'TAT':'Y', 'TAC':'Y', 'TAA':'STOP', 'TAG':'STOP', 'TGT':'C', 'TGC':'C', 'TGA':'STOP', 'TGG':'W', 
'CTT':'L', 'CTC':'L', 'CTA':'L', 'CTG':'L', 'CCT':'P', 'CCC':'P', 'CCA':'P', 'CCG':'P', 'CAT':'H', 
'CAC':'H', 'CAA':'Q', 'CAG':'Q', 'CGT':'R', 'CGC':'R', 'CGA':'R','CGG':'R',
'ATT':'I','ATC':'I','ATA':'I','ATG':'M','ACT':'T','ACC':'T','ACA':'T','ACG':'T',
'AAT':'N','AAC':'N','AAA':'K','AAG':'K','AGT':'S','AGC':'S','AGA':'R','AGG':'R',
'GTT':'V','GTG':'V','GTA':'V','GTG':'V','GCT':'A','GCC':'A','GCA':'A','GCG':'A',
'GAT':'D','GAC':'D','GAA':'E','GAG':'E','GGT':'G','GGC':'G','GGC':'G','GGA':'G','GGG':'G'};

f=open('gene','r')
line=f.readline()
i=0

while(i<1000):
        x = line[i:i+3]
        print T[x],
        i=i+3
~~~~~~~~



