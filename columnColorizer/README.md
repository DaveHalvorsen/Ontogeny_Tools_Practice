this script colorizes each column
the txt file is a 23andMe data file .. the top of it is descriptive, so Clay's script won't work unless I cut
here I used tail and got the different color outputs
tail hu0A6570.txt | ./ontogeny_columnColorizer.sh 

same issue w/ the illumina file 
tail Illumina_huBEF5E2_GSA-24v2.txt | ./ontogeny_columnColorizer.sh 

csv data
Big-Y 500 SNP CSV data (updated)
https://my.pgp-hms.org/profile/hu2FEC01

neither of these methods work
tail Big-Y\ 500\ SNP\ CSV\ data\ \(updated\).csv 
cat Big-Y\ 500\ SNP\ CSV\ data\ \(updated\).csv | ./ontogeny_columnColorizer.sh 





====
illumina file https://my.pgp-hms.org/profile/huBEF5E2
huBEF5E2_GSA-24v2.txt



