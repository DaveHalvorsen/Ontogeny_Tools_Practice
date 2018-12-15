./ontogeny_list.sh 
that only lists the shell script and thre readme file
cd into higher directory and run
./list/ontogeny_list.sh
lists the directories and a README file. the \ and \.pub file aren't listed
this is one reason that aliases are great ... can jsut run the alias wherever instead of needing to link to actual directory

this works running from the fastq directory
fastq$ ./../list/ontogeny_list.sh 

this works running from the Data directory
/Data/brain_scRNA$ ./../../list/ontogeny_list.sh 

this seems better than newLs cause it gives # of lines for README file


