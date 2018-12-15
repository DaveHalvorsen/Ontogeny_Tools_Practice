there isn't a detailed guide for this one ... what is a submission?
is it a submission to a database?
i ran it in an empty directory and got the following: 
"
./ontogeny_inspectSubmission.sh: line 157: hgsql: command not found
./ontogeny_inspectSubmission.sh: line 158: hgsql: command not found
./ontogeny_inspectSubmission.sh: line 164: hgsql: command not found

It appears there aren't any submissions related to this directory. We will instead validate tag storm and manifest files, if any are found.
"
^I think this is for SQL submissions to a database (UCSC genome browser?)

both my foldered version and the original clay version yield this error ONLY when a meta.txt file is included ... is it cause the ontology tools isn't set up?
cat: '~clay/qa/tags.schema': No such file or directory
trying ontology tools:
nope ... i still get cat: '~clay/qa/tags.schema': No such file or directory
i think ~clay is specifically for his home directory ... maybe 
I'm looking through inspectSubmission.sh and i found the line this is coming from:
"
validTags=$(cat ~clay/qa/tags.schema | cut -f 1 -d " " | grep -v "^#")
"
i think it's a list of valid tags that clay has on his local computer, but not this repo
I don't think I can fix this ...
well, anyways it reads throught he meta.txt file and yields this
2018-12-06 quakeBrainGeo1_meta.txt: 3411 lines, and has 33 unique tags. 
all the tags are listed as invalid ... I THINK because there's no way to check against clays' list of valid tags, lol

I don't think you can run this outside of it's directory. This yielded info for .sh storage directory
./ontogeny_inspectSubmission.sh Kriegstein/

i tried running it in the directory w/; the tsv and txt meta files and it only recognized the txt
Kriegstein$ ./ontogeny_inspectSubmission.sh ^C

I think the meta.txt and meta.tsv files can be interchanged ... maybe that's what the Kent TagStorm files are about?


====
DATA

Kriegstein
sc002MJC
http://cirm.ucsc.edu/cgi-bin/cdwWebBrowse?cdwCommand=oneFile&cdwFileTag=file_name&cdwFileVal=sc002MJC.tsv&hgsid=83335_51JgbnuomO1Qcr4aVk5YZM53aZlc
sc002MJB
http://cirm.ucsc.edu/cgi-bin/cdwWebBrowse?cdwCommand=oneFile&cdwFileTag=file_name&cdwFileVal=sc002MJB.txt&hgsid=83335_51JgbnuomO1Qcr4aVk5YZM53aZlc
