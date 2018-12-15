
MAYBE I COULD ADD PATTERNS.TXT ABILITY ... ?
	$ highlight file.txt pattern1 pattern2 ... pattern{n}

	$ cat file.txt | highlight stdin pattern1 pattern2 ... pattern{n}

	$ cat file.txt | highlight piped pattern1 pattern2 ... pattern{n}

gets instances of CC SNP in file
./ontogeny_highlight.sh hu0A6570.txt CC

gets instances of CC and AG in file
./ontogeny_highlight.sh hu0A6570.txt CC AG

uses stdin to get CC pattern
cat hu0C8573.txt | ./ontogeny_highlight.sh stdin CC

same but with piped instead of stdin
cat hu0C8573.txt | ./ontogeny_highlight.sh piped CC

\where file.txt can also be "file1.txt file2.txt" or "*.txt" to filter
./ontogeny_highlight.sh *.txt rs106005

reads all the files with .txt extension and highlights instances of 23andMe
./ontogeny_highlight.sh *.txt 23andMe

highlights all instances of 1
./ontogeny_highlight.sh *.txt 1


personal genome project survey added

./ontogeny_highlight.sh PGPBasicPhenotypesSurvey2015-20180531180158.csv blue
this highlights and the # of blues
this highlights and counts the # of browns
./ontogeny_highlight.sh PGPBasicPhenotypesSurvey2015-20180531180158.csv brown
this counts brown and blue
./ontogeny_highlight.sh PGPBasicPhenotypesSurvey2015-20180531180158.csv brown blue

here's a cool practical applicaiton:
I added 6 23andme data files (5 .txt and 1 .csv)
ran this:
./ontogeny_highlight.sh "*.txt" 23andMe
it found "23andMe" 8 times ... weird. It should be 2 X 5 = 10 times ... why?
okay, so it seems like it's a case thing: 23andMe vs 23andme ... diff formats
./ontogeny_highlight.sh "*.txt" 23andme
that command gets 5 hits
I should play w/ the regex when I get a chance
./ontogeny_highlight.sh hu0A6570.txt $'\s'
that pushed CPU up to 100% cause there's so many dang spaces X # lines in 23andMe files

