# Data from Chapter 4

The data from Chapter 4 largely follows the same structure as in the other chapters.
This README.md outlines the few changes.

- The `idf.json` in this directory is used as the general IDF or ICF file.
We created this IDF file from a large sample of tweets about no subject in particular, which we call the general corpus.
We share the IDs from the general corpus in the `data/` directories.
- In our analyses, we experiment with different configurations of the baselines.
To speed up the process, we tokenized the corpora in various ways.
We do not store the entire tokenized corpora here, both to reduce data usage and to maintain user anonymity.
Instead, we provide only the meta files in the `evaluation-data/` directories, which describe _how_ we generated the tokenized files.
You can re-tokenize the files by re-using the same parameters as in the meta files.