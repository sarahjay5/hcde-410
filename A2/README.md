# HCDE410
Files for HCDE410 - Assignment A2

## A2: Exploring Sources of Bias in Data

**Dataset:** Wikipedia Talk Corpus (Detox project): crowdworker demographics and toxicity annotations for comments on English Wikipedia talk pages.
**Source:** Figshare, "Wikipedia Talk Labels: Toxicity" (plus the attack and aggression datasets).
**Publisher:** Jigsaw and the Wikimedia Foundation.
**License / terms of use:** See the license on the Figshare page for each dataset. The code in this folder is under the MIT License (see `LICENSE`).

## What I looked at
- **Part 1:** Cleaning and sanity-checking the annotator demographic files. I found that the attack and aggression files are identical, and that `worker_id` is reused across datasets for different people, so I made a unique ID.
- **Part 2:** Distributions of the workers by gender, first language, age group, and education (Q1-Q4), missing data (Q5), what happens if duplicates are not removed (Q6), and how the workers compare to internet users (Q7-Q8).
- **Part 3:** The code questions (Q9-Q12): how many workers have demographics, and who produced the labels.

## How to re-run
Open `hcde410-a2.ipynb` and run all cells (needs `pandas` and `plotly`). The three worker demographics files and `toxicity_annotations.tsv` need to be in `wikipedia_datasets/`.

## Limitation / bias in the data
The workers are mostly male, under 45, highly educated, and mostly non-native English speakers, so the labels reflect their views of "toxic," which may not match the people a detector is used on. About 16% of the labels come from workers with no demographic data, and I can't tell whether the same person labelled more than one dataset under different IDs. My claims about how this could affect Perspective API are hypotheses; I did not test them.

## AI use
I used an AI assistant for help with coding (including fixing an error in the duplicate check and building the tables and graphs), then interpreted the results myself and used AI for background statistics in Q7 and for wording and checking that my answers and interpretations made sense.