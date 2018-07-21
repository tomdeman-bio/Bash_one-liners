# Bash_one-liners
Bash one-liners useful for bioinformatics 

### Extract column 1, 2, and 3 from File.txt, concatenate and separate them by "-"
awk '{print $0, $1 "-" $2 "-" $3}' File.txt
