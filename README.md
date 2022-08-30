# Data from _Reading Between Events: Exploring the Role of Machine Understanding in Event Tracking_

This repository contains the data, outputs and results from the thesis _Reading Between Events: Exploring the Role of Machine Understanding in Event Tracking_.
For the algorithms developed during the project, please see the [EvenTDT library](https://github.com/NicholasMamo/EvenTDT).

## Repository structure

If you're reading this README.md file, then you're at the root of the repository.
The rest of the repository follows a consistent structure.

At the top-level, the repository branches into folders, one for each chapter.
The folder names refer directly to the chapters in the thesis titled _Reading Between Events: Exploring the Role of Machine Understanding in Event Tracking_.

Internally, each chapter branches with a consistent structure.
We separate the shared data according to sections with a similar naming convention as above.
Depending on the chapter, each of these folders may contain the following folders:

- The `data` folders store the tweets used in the chapter.
Due to Twitter's policy, we may only share the tweet IDs, not the original tweets.
You can download the tweets again using the `download` tool in [the EvenTDT library](https://github.com/NicholasMamo/EvenTDT).
- The `evaluation-data` folders store any other data that we used to generate the outputs, which we describe next.
The evaluation data may include concepts and term-weighting schemes, among other types of resources.
- The `ground-truth` folders contain the lists of ground truth that we use to evaluate our outputs.
This folder is present only whenever we used an automated evaluation approach.
- The `notebooks` folders contain the Jupyter Notebook files (and any associated files) that were used to create visualizations or to analyze the data.
You can open the notebooks by running Jupyter Notebook (`jupyter notebook` on Linux), but note that to re-run the experiments, you need to change the file paths, usually specified in the first cells.
Some file names have been edited for clarity, but the notebooks can be opened without being run to examine the output and analyses.
- The `outputs` folders store the outputs that we later evaluated.
We generated most of the outputs using the [EvenTDT library](https://github.com/NicholasMamo/EvenTDT), and similarly to before, we only store references to tweets.
You can replicate the outputs by downloading the data and then looking for the metadata of each file.
Some files have metadata stored in them (in the `pcmd` key); others have separate `.meta.json` files.
You can read the metadata easily using the `meta` tool in the [EvenTDT library](https://github.com/NicholasMamo/EvenTDT).
- The `results` folder stores the automated evaluation, often using the files in the `ground-truth` folders.
We separate results according to the analyses.
- The `sheets` folder stores the manual evaluations, which we carried out in spreadsheets.
You can download the spreadsheets to observe our annotations.
Note that some functions used in the spreadsheets may only be used with Google Sheets.

## Citing this repository

If you use any data in this repository, cite the following thesis:

> Mamo, N. Reading Between Events: Exploring the Role of Machine Understanding in Event Tracking. PhD thesis, Department of Artificial Intelligence, Faculty of Information & Communication Technology, University of Malta, XYZ 2022.
