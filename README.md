# Contrasting Human- and Machine-Generated Word-Level Adversarial Examples for Text Classification
This repository contains the data collected for our EMNLP 2021 [paper](https://aclanthology.org/2021.emnlp-main.651/) *Contrasting Human- and Machine-Generated Word-Level Adversarial Examples for Text Classification*.

## Human- and machine-generated adversarial examples
The human- and machine-generated adversarial examples are in the file `collected_adversarial_examples.csv`. The file contains 1020 rows, representing the 170 sequences unperturbed and perturbed with each of the 5 attacks.

The columns are as follows:
* id: the sequence ID, which also identifies the attack used (or no attack)
* text: the corresponding text
* succ: whether the adversarial examples successfully flipped the classifier label
* label: the actual ground truth label of the sequence
* num_queries: the number of queries needed to generate the adversarial example
* sub_rate: the word substitution rate

## Collected data

### Stage one
The raw collected data from the crowdsourcing experiments corresponding to Task 4 of the first data collection stage (see Section 3.1 in the paper) can be found in `task_4.json`.

### Stage two
The collected ratings for each generated adversarial example can be found in `ratings.json`. For each rated text, the JSON provides the total amount of ratings for both naturalness and sentiment. For both criteria, the ratings are on a scale from 1 (very negative sentiment/very unnatural) to 5 (very positive sentiment/very natural).

## References
If you find this repository useful, please consider citing our paper:
```
@inproceedings{mozes-etal-2021-contrasting,
    title = "Contrasting Human- and Machine-Generated Word-Level Adversarial Examples for Text Classification",
    author = "Mozes, Maximilian  and
      Bartolo, Max  and
      Stenetorp, Pontus  and
      Kleinberg, Bennett  and
      Griffin, Lewis",
    booktitle = "Proceedings of the 2021 Conference on Empirical Methods in Natural Language Processing",
    month = nov,
    year = "2021",
    address = "Online and Punta Cana, Dominican Republic",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2021.emnlp-main.651",
    doi = "10.18653/v1/2021.emnlp-main.651",
    pages = "8258--8270",
}
```