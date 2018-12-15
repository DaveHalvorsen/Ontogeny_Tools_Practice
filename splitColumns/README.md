make sure you use the right delimiter!
weird ... this command
./ontogeny_splitColumns.sh hu0C8573.csv 
hields this output
s_np_chr_allele1_allele2.txt
why? it looks like the shell script just lower cased row 1 and added an underscore 
oh, nvm ... it created  a new file by that name w/ commas separating ...
there's more to it I imagine.

./ontogeny_splitColumns.sh PGPBasicPhenotypesSurvey2015-20180531180158.csv 
that creates this HUGE filename:
"
participant_timestamp_do_not_touch11_blood_type_height_weight14_comments21_left_eye_photograph_number_fullsize_image_httpsgoogl_xq2_voh22_right_eye_photograph_number_fullsize_image_httpsgoogl_xq2_voh_left_eye24_right_eye_color_text_description25_comments31_what_is_your_natural_hair_color_currently_when_without_artificial_color_or_dye32_hair_color_text_description33_comments41_any_final_thoughts14_handedness.txt
"
yet I don't see the file ... maybe the huge filename crashed the script?

this breaks each column up into files of the given column name w/ all the original column's rows in it
./ontogeny_splitColumns.sh PGPBasicPhenotypesSurvey2015-20180531180158.csv prefix_ ","

