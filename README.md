> NOTE: Use the web-view hosted here https://anonymous54324.github.io/corefix_data/

# CoReFix Data Samples

This repository contains samples from the data of CoReFix paper. 
The samples are code reduced versions of the files.
In case you want to see the full version of the files, we also included github urls. Each rule folder has a README and it contains the two url links per delta and the filename in the repo. 
File url links should take you directly to the file and also highlight the line where the rule was reported by static analyzer.
The other url is the link to the commit.
Please read the last section in the README about github urls.

We would like to avoid sharing the complete dataset yet and therefore for each rule we randomly sampled two instances from our dataset. 
# How to view the samples?

Please use the web-viewer hosted here: https://anonymous54324.github.io/corefix_data/

# Structure of the repo for a single rule

├── AmbiguousConditional \
│   ├── delta_AmbiguousConditional.html # delta for the first sample \
│   ├── delta_AmbiguousConditional.html # delta for the second sample \
│   ├── README.md # contains github urls to original repos \
└── README.md 

# Note about GitHub URLs

In rare cases github urls will not lead you to the correct place. This is not a bug in our code but it is related to how libgit library works. We do not store the full files in our dataset to save memory but fetch them on the fly via libgit. Those commit hashes work for file fetching process because libgit also has some internal logic to handle rebases, merge commits and other things. Therefore, the commit hashes we save are meant to be used for file fetching via libgit not for url creation. That's why, when used as urls, the commit shas might not lead to the right place.

In such cases, you can open the github repo, find the file (filename is provided in html files) and search the history of that file. Some of the commits close to the given commit hash must contain the presented changes.

