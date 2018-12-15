# About Data_Wrangler_Tools

Dec 6th 2018
I just started my Learning_Ontogeny repository as a copy of claymfischer's ontogeny toolkit ... check it out here: https://github.com/claymfischer/ontogeny

I like Clay's goal of helping with the transition from wet lab to computer lab. That's what I'm trying to do :)

There's a lot of good stuff in his repository, but it's a little overwhelming for me seeing everything all in one place (the bin directory). I plan to break up his shell scripts into individual folders; I'll add practice data into each folder and fiddle around with it. Additionally, I'll read through the scripts themselves and figure out how they work.

I don't intend to use his bash startup file aliases just yet ... that lib/ontogeny_toolkit.sh file is big. Once I get a handle on his shell scripts, I'll work through his ontogeny_toolkit.sh Along the way I'll record any errors I run into and possibly fix them. I *really* like all of the pictures he's included ... I think a great tutorial could be built from his repository with the addition of practice data files and protocol suggestions ... that's kinda the direction I plan to go with in my Learning_Ontogeny repo.

==========
* learning how all these scripts work w/ data cause this seems to be best UCSC data wrangler resource
* add example files and example commands + output to help future folks learn faster
* possibly work toward creating a data wrangling tutorial
* add to original README explanations and also usage info (many missing)

splitting into diff folders breaks all the aliases, so it forces me to dig through that toolkit file to fix all of them ... it's a solid learning exercise :)
* splitting ontology_tools.sh into individual files BREAKS => forces learning
* changing file names as part of that too
* adding data and testing shows understanding

# Distinctions from Prior Work
* added data files, "commands", expected output

# Data Sources
* Personal Genome Project https://www.personalgenomes.org/
* Center for Excellence in Stem Cell Genomics http://cirm.ucsc.edu/ 
* Human Cell Atlas https://www.humancellatlas.org/

^ I think those should break down into smaller headings ... this is markdown, so it should be
## smaller
### even smaller
#### very small
##### almost the smallest
###### the smallest

# Explanation of File Types
* .txt
* .csv
* .fastq.gz
* 

# Shell Scripts
* about.sh This script was originally written by GitHub user claymfischer. It can be found in his [ontogeny respository](https://github.com/claymfischer/ontogeny).
* changePrompt.sh This script was originally written by GitHub user claymfischer. It can be found in his [ontogeny respository](https://github.com/claymfischer/ontogeny).
* checkSubmission.sh This script was originally written by GitHub user claymfischer. It can be found in his [ontogeny respository](https://github.com/claymfischer/ontogeny).
* columnColorizer.sh This script was originally written by GitHub user claymfischer. It can be found in his [ontogeny respository](https://github.com/claymfischer/ontogeny).
* columns.sh This script was originally written by GitHub user claymfischer. It can be found in his [ontogeny respository](https://github.com/claymfischer/ontogeny).
* contents.sh This script was originally written by GitHub user claymfischer. It can be found in his [ontogeny respository](https://github.com/claymfischer/ontogeny).
* fastq.sh This script was originally written by GitHub user claymfischer. It can be found in his [ontogeny respository](https://github.com/claymfischer/ontogeny).
* findIt.sh This script was originally written by GitHub user cjvillar. It can be found in his [DogTools respository](https://github.com/cjvillar/DogTools).
* highlight.sh This script was originally written by GitHub user claymfischer. It can be found in his [ontogeny respository](https://github.com/claymfischer/ontogeny).
* inspectSubmission.sh This script was originally written by GitHub user claymfischer. It can be found in his [ontogeny respository](https://github.com/claymfischer/ontogeny).
* list.sh This script was originally written by GitHub user claymfischer. It can be found in his [ontogeny respository](https://github.com/claymfischer/ontogeny).
* mungerTest2.0.sh This script was originally written by GitHub user cjvillar. It can be found in his [ontogeny respository](https://github.com/cjvillar/DogTools).
* newLs.sh This script was originally written by GitHub user claymfischer. It can be found in his [ontogeny respository](https://github.com/claymfischer/ontogeny).
* splitColumns.sh This script was originally written by GitHub user claymfischer. It can be found in his [ontogeny respository](https://github.com/claymfischer/ontogeny).
* spreadsheetInput.sh This script was originally written by GitHub user claymfischer. It can be found in his [ontogeny respository](https://github.com/claymfischer/ontogeny).
* tagStormSummary.sh This script was originally written by GitHub user claymfischer. It can be found in his [ontogeny respository](https://github.com/claymfischer/ontogeny).
* tagSummary.sh This script was originally written by GitHub user claymfischer. It can be found in his [ontogeny respository](https://github.com/claymfischer/ontogeny).



# Terminal Extensions (Alias Commands for .bashrc)
* shell_script_aliases.sh

# Future Directions
* some folders get really messy when code is run ... make subdirectories
* I kept the "ontogeny_" prefix for all of Clay's scripts. I'll eventually remove them (once he's mentioned in the intro section).
* I should try and get Kent's tagStorm program working on meta.txt files ... later
* I think I'll remove unrelated folders: ASCII_Scripts, changePrompt, palette ... possibly others
* Add usage statement and better error handling to incomplete scripts
* Add better in-line comments to the scripts ... this'll help me learn bash faster
* Break up Clay's ontogeny_tools.sh into individual alias files (to learn how things work)
* Add a Data folder with an example of every kind of data (this'll be good for alias testing)
* Create tutorials to explain step by step data handling
* I couldn't get changePrompt to work, so I deleted it
* I liked cjvillar's ASCII scripts, but I removed them because not data-relevant
* I haven't used cjvillars' qaTools because I don't have access to those databases
* mungerTest2.0.sh isn't a detailed name. I should change it

