# Identifying SOGI-based crimes in  Russian court decisions
Uncovering crimes that are based on prejudices motivated by someone's sexual orientation and/or gender identity in Russian court decisions.
See the directory 'sogi_based_crimes' for the resulting dataset of collected crimes from the decisions between 2021 and 2022.

The cases with SOGI-based crimes were identified in all available court decisions for 2021 and 2022 scraped from the official Russian court websites (for the info about the websites, refer to [sudrfparser](https://github.com/dataout-org/sudrfparser/tree/main/courts_info)).

The Python module [sudrfparser](https://github.com/dataout-org/sudrfparser) allows to scrape cases from all court websites. There are also functions to search cases by custom keywords on the official Russian portal "Provosudie" (bsr.sudrf.ru).

### In-browser tool for reading court cases with auto-annotation
Court cases are ususually long texts. To exract data from them easier, we have built an in-browser interface that loads court cases texts from this repository and annotates (highlights) several categories. Currently, it supports highlighting (1) dates, (2) amounts of money, (3) sexual orientation markers, (4) keywords of extenuating and aggravating circumstances of punishments.
To use the interface, open [cases_reader.html](cases_reader.html) in a browser. The code can be customised to read court cases from other sources (for example, by modifying the const variable 'jsonUrl' –– a link to a json file with cases texts).


_Information for the Bellingcat hackathon:_

- Team name: Dataout
- Team members: Andrei Nesterov
- Future work: Releasing a larger database of SOGI-based crimes in Russia between 2008–2023
- The license is [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/)_
