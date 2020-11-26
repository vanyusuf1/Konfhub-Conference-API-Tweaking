# Konfhub Conference API Tweaking Program [**TASK**] 🛠️

An **API** `(which provides the list of upcoming technical conferences)` tweaker program written in **python** which performs following tasks:

- _Extract contents from given Api link_

- _Print the contents in a human readable format, e.g.: `“San Antonio CyberSecurity Conference”, November 6th, 2019, San Antonio, TX, US, Paid. https://futureconevents.com/events/san-antonio/”`_

  ![Output](https://github.com/vanyusuf1/Konfhub-Conference-API-Tweaking/blob/main/images/task1.PNG)

- _Identify exact duplicates (if any)_

  ![Output](https://github.com/vanyusuf1/Konfhub-Conference-API-Tweaking/blob/main/images/task2.PNG)

- _Identify semantic duplicates (i.e., the conferences are same but the details provided are slightly different, e.g., “**React Conference 2019**” in one entry and “**ReactConf ‘1**9” in another entry but the other fields are same or similar)._

  ![Output](https://github.com/vanyusuf1/Konfhub-Conference-API-Tweaking/blob/main/images/task3.PNG)

## Tasks Status

- ## **Task1** ✔️
- ## **Task2** ✔️
- ## **Task3** ✓✓....
        Task 3 is partly completed. Semantic duplicates are extracted
        with complete accuracy when implemented in NLP which is out of scope
        for this task. Therefore, python library fuzzywuzzy is
        used here for getting better results.
  - `fuzzywuzzy` has 4 types, `FuzzyWuzzyRatio` `FuzzyWuzzy PartialRatio` `FuzzyWuzzyTokenSortRatio` and `FuzzyWuzzyWRatio`.
  - Among these four, `FuzzyWuzzyRatio` produces descent result for this particular _api_ with **ratio>=71**.
