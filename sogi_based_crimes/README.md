Crimes motivated by prejudices based on sexual orientation and gender identity (SOGI) collected from Russian court decisions (first instance criminal cases) for 2021 and 2022.
The dataset includes 42 cases with the following metadata:

* case_id_uid: a combination of a case identifier and uid (unique identifier) used in the case link;
* case_id_text: a case identifier given by a court (usually contained the case text);
* adm_date: corresponds to "Дата поступления" (the date a case was received by a court) (DD.MM.YYYY);
* article: a list of articles from the Criminal Code ("Перечень статей"); an article is linked to an accused; base offence;
* accused_n: number of accused;
* crime_group: if a crime was commited by a group; TRUE or FALSE (boolean);
* crime_date: date (DD.MM.YYY or MM.YYYY) of the actual crime (if known) from the case text ;
* crime_year: year of crime (if known); ithis datset includes crimes that happened between 2019 and 2022;
* victim_n: the number of victims in a case;
* victim_n_died: the number of victims who died as a result of the crime;
* crime_address: address or place where a crime took place (if known) taken from a case text;
* crime_description_tags: textual keywords that describe a crime: for example, "murder", "physical violence","threat of physical violence", "blackmailing"; these tags can be used only if there’s evidence in the case text; multiple tags can be used for one case;
* hate_motive: TRUE or FALSE, if a case contains indicators of a hate crime (according to [OSCE guidelines](https://www.osce.org/files/f/documents/1/4/523940.pdf));
* victim_sogi_markers: markers indicating victim's sexual orientation and/or gender identity (extracted as is, contains descriminatory language);
* victim_sogi_source: a source from which sogi info is taken: a victim, accused, witness, judge;
* notes: textual field with notes;

The archive 'sudrf_keyword_search.zip' containd 716 court decisions with keywords indicating SOGI;
The keywords with regular expressions are in the txt file 'sogi_keywords.txt';
The jupyter notebook 'searching_keywords.ipynb' contains a pipeline of retrieving decisions with keywords.
The file 'keyword_search_context_df.csv' contains 716 cases with case snippets;