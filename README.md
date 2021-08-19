# Analyzing Gender Bias Across Turkish to English Machine Translation Datasets

by [Chloe Ciora](https://github.com/ChloeCiora), [Nur Iren](https://github.com/NurIren), [Malihe Alikhani](https://github.com/malihealikhani)

## Introduction

This work aims to bring attention to both overt and covert gender bias in Machine Translation (MT) through the use of the Turkish and English language. This repository provides the datasets and translated results. The generation and evaluation methods are described in the Experiments section of the paper. 

### Occupation Datatset: 

The [TR-EN occupation dataset](./Occupations_datasets/Occupations_Matched.csv) contains occupations that exist in both Turkey and the United States. Turkish occupation titles are inserted into the following sentences templates in order to evaluate for stereotype bias and the difference additional qualifiers make: 

Turkish Sentence | English Translation
------------ | -------------
O bir &lt;occupation&gt;.| He/She is a(n) &lt;occupation&gt;.
O &ccedil;ok iyi bir &lt;occupation&gt;.| He/She is a very good &lt;occupation&gt;.
O iyi bir &lt;occupation&gt;.| He/She is a good &lt;occupation&gt;.
O k&ouml;t&uuml; bir &lt;occupation&gt;.| He/She is a bad &lt;occupation&gt;.
O &ccedil;ok k&ouml;t&uuml; bir &lt;occupation&gt;.| He/She is a very good &lt;occupation&gt;.


The [original occupation lists](./Occupations_datasets/occupations_lists_from_source) used to create this corpus and the Google, Amazon, Microsoft, and SYSTRAN [translations](./Occupations_datasets/translations) are also provided.

### Descriptive Adjective Dataset

The list of [adjectives, sentence templates, and translated results](./Adjectives_datasets/Adjective_Dataset_and_Translations.csv) used in the paper. Turkish adjectives are inserted into the following sentence templates in order to evaluate for gender stereotypes and the difference personhood makes:

Turkish Sentence | English Translation
------------ | -------------
O &lt;adjective&gt;.| He/She is &lt;adjective&gt;.
O &lt;adjective&gt; birisidir.| He/She is someone who is &lt;adjective&gt;.

### Asymmetrical Gender Markings Dataset

The [asymmetrical gender markings dataset](./Asymmetrical_gender_datasets.Explicit_Gender_Markings_Dataset_and_Translations) for our newly proposed evaluation method and translations. 

The following subject words were inserted into a sentence involving a masculine or feminine stereotype such as an occupation, adjecitve, or action: 

English Gendered Word | Turkish Neutral Translation | Turkish Gendered Translation
--------------------- | ------------- | -------------
sister / brother | karde&scedil; | kız karde&scedil; / erkek karde&scedil;
girlfriend / boyfriend | arkada&scedil; | kız arkada&scedil; / erkek arkada&scedil;
niece / nephew | ye&gbreve;en | kız ye&gbreve;en / erkek ye&gbreve;en
young ladies / young men | gen&ccedil;ler | gen&ccedil; kadınlar / gen&ccedil; erkekler



## Citation

If you use this data, please cite the following paper:

Ciora Chloe, Iren Nur, Alikhani Malihe. 2021. Examining Covert Gender Bias: A Case Study in Turkish and English Machine Translation Models. In Proceedings of the 14th International Conference on Natural Language Generation (SIGGEN-INLG 2021)

BibTeX entry:
```
@InProceedings{CioraEtAl2021GenderBiasAcrossTurkishToEnglish,
  title        = {Examining Covert Gender Bias: A Case Study in Turkish and English Machine Translation Models},
  author       = {Ciora, Chloe and Iren, Nur and  Alikhani, Malihe},
  booktitle    = {Proceedings of the 14th International Conference on Natural Language Generation (SIGGEN-INLG 2021)},
  year         = {2021},
  publisher    = {Association for Computational Linguistics Special Interest Group on Natural Language Generation},
  address      = {Pittsburgh, PA, USA},
  location     = {Aberdeen, SCT, UK}, 
}

```
