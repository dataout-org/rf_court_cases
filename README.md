# Identifying SOGI-based crimes in  Russian court decisions
Uncovering crimes that are based on prejudices motivated by someone's sexual orientation and/or gender identity in Russian court decisions.
See the directory 'sogi_based_crimes' for the resulting dataset of collected crimes from the decisions between 2021 and 2022.

The cases with SOGI-based crimes were identified in all available court decisions for 2021 and 2022 scraped from the official Russian court websites (see all websites in the file 'sudrf_websites.json');

* The python functions in 'sudrfparser.py' allow to scrape cases from all court websites;
* The functions in 'bsr_parser.py' are designed to search for cases on the official Russian portal "Provosudie" (bsr.sudrf.ru) containing keywords a user defines;
