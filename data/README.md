# algorithm-bias-R
Searching for proof that algorithmic bias is significant 
# SISE2601 Project data description
================
Eran Aizikovich and Yuval Segal

Our original Data set has 131 columns, most of them were redundant.  
After cleaning the data, without losing any information that is meaningful   
to our research we were left with 30 columns.

Rows: 135,556
Columns: 30
Primary key in our data:
	* comment_id <int>   unique ID for each comment
	* annotator_id <int> unique ID for each annotator
* sentiment <dbl>  ordinal label that is combined into the continuous score
* respect <dbl> ordinal label that is combined into the continuous score
* insult <dbl> ordinal label that is combined into the continuous score
* humiliate <dbl> ordinal label that is combined into the continuous score
* dehumanize <dbl> ordinal label that is combined into the continuous score
* violence <dbl> ordinal label that is combined into the continuous score
* genocide <dbl> ordinal label that is combined into the continuous score
* attack_defend <dbl> ordinal label that is combined into the continuous score
* hatespeech <dbl> ordinal label that is combined into the continuous score.
* hate_speech_score <dbl> The continuous score of the post, higher = more hateful .
* infitms <dbl> inlier sensitive value(continuous) of the comment.
* outfitms <dbl> outlier sensitive value(continuous) of a comment.
* annotator_severity <dbl> continuous value that estimates the annotator’s survey interpretation bias.
* std_err <dbl> continuous value of the standard deviation between annotators on this comment.
* annotator_infitms  <dbl> inlier sensitive value(continuous) of the annotator.
* annotator_outfitms <dbl> outlier sensitive value(continuous) of a comment.
* target_race <chr>  categorical variable, tagged by annotator
* target_gender <chr>  categorical variable, tagged by annotator
* target_sexuality <chr> categorical variable, tagged by annotator
* annotator_gender <chr> categorical variable
* annotator_educ <chr> categorical variable, annotator’s education.
* annotator_income <chr> categorical variable, within range.
* annotator_ideology <chr> categorical variable: neutral, slightly_conservative, extremely_liberal,  
    extremely_conservative, liberal, conservative, slightly_liberal, no_opinion
* annotator_age <dbl> Discrete variable
* annotator_race <chr> Categorical variable
* annotator_religion  <chr> Categorical variable
* annotator_sexuality <chr> Categorical variable: straight, bisexual, gay, other
  
  
Our original data had 131 columns; the additional columns were removed by us in the cleaning stage.
The columns we removed were:
(All columns besides the first three were Boolean variables.)

platform, status, text, target_race_asian, target_race_black, target_race_latinx,   
target_race_middle_eastern, target_race_native_american, target_race_pacific_islander,   
target_race_white, target_race_other, target_religion_atheist, target_religion_buddhist,   
target_religion_christian,   target_religion_hindu, target_religion_jewish,  
target_religion_mormon, target_religion_muslim, target_religion_other,   
target_origin_immigrant, target_origin_migrant_worker , target_origin_specific_country,  
target_origin_undocumented, target_origin_other, target_gender_men, target_gender_non_binary,   
target_gender_transgender_men, target_gender_transgender_unspecified,   
target_gender_transgender_women, target_gender_women, target_gender_other,   
target_sexuality_bisexual, target_sexuality_gay , target_sexuality_lesbian,   
target_sexuality_straight, target_sexuality_other, target_age_children , target_age_teenagers,  
target_age_young_adults , target_age_middle_aged, target_age_seniors, target_age_other,  
target_disability_physical, target_disability_cognitive, target_disability_neurological,  
target_disability_visually_impaired, target_disability_hearing_impaired,  
target_disability_unspecific, target_disability_other , target_disability, annotator_trans,  
annotator_gender_men, annotator_gender_women, annotator_gender_non_binary,  
annotator_gender_prefer_not_to_say, annotator_gender_self_describe, annotator_transgender,  
annotator_cisgender, annotator_transgender_prefer_not_to_say, annotator_education_some_high_school,  
annotator_education_high_school_grad , annotator_education_some_college, annotator_education_college_grad_aa,   
annotator_education_college_grad_ba, annotator_education_professional_degree , annotator_education_masters,  
annotator_education_phd , annotator_income_<10k, annotator_income_10k>50k, annotator_income_50k>100k,   
annotator_income_100k>200k, annotator_income_>200k, annotator_ideology_extremeley_conservative,  
annotator_ideology_conservative, annotator_ideology_slightly_conservative, annotator_ideology_neutral,  
annotator_ideology_slightly_liberal , annotator_ideology_liberal, annotator_ideology_extremeley_liberal,  
annotator_ideology_no_opinion, annotator_race_asian, annotator_race_black, annotator_race_latinx,  
annotator_race_middle_eastern, annotator_race_native_american, annotator_race_pacific_islander,  
annotator_race_white, annotator_race_other, annotator_religion_atheist, annotator_religion_buddhist,  
annotator_religion_christian , annotator_religion_hindu , annotator_religion_jewish,  
annotator_religion_mormon, annotator_religion_muslim, annotator_religion_nothing, annotator_religion_other,  
annotator_sexuality_bisexual, annotator_sexuality_gay, annotator_sexuality_straight, annotator_sexuality_other. 
