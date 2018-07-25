# Bash_one-liners
Bash one-liners useful for bioinformatics 

### Extract column 1, 2, and 3 from File.txt, concatenate and separate them by "-". Then print original columns + new concatenated column 
awk '{print $0, $1 "-" $2 "-" $3}' File.txt

### Loop through plain text file and print
while read p; do echo $p; done < File.txt
