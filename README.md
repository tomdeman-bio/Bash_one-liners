# Bash_one-liners
Bash one-liners useful for bioinformatics 

### Extract column 1, 2, and 3 from File.txt, concatenate and separate them by "-". Then print original columns + new concatenated column 
awk '{print $0, $1 "-" $2 "-" $3}' File.txt

### Loop through plain text file and print each line
while read p; do echo $p; done < File.txt

### Loop through plain text file and find lines in a second file 
while read p; do grep "$p" File-2.txt; done < File.txt

### Take every 9th line from a file
awk '!(NR % 9)' File.txt

### Append text to the end of every line in a file
awk '{print $0"SUFFIX"}' File.txt

### Append text to the beginning of every line in a file
awk '{print "PREFIX"$0}' File.txt

### Create a folder with multiple subfolders
mkdir -p output/{result_1,result_2}
