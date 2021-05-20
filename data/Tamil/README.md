## Proteno Tamil Dataset

This dataset contains 30, 350 sentences for text normalization sampled from English-Tamil parallel corpus (Ramasamy et al., 2012) and Comparable Corpora (Eckart and Quasthoff, 2013).  There are two Python pickled lists containing tokenized unnormalized sentences (unnorm_list.pkl) and their corresponding tokenized normalizations (norm_list.pkl). First 60% of the data was used for training Proteno and the models were evaluated on the other 40%.

## License
This dataset is licensed under CC-BY-NC-SA License.

## References

```
@inproceedings{ramasamy-etal-2012-morphological,
    title = "Morphological Processing for {E}nglish-{T}amil Statistical Machine Translation",
    author = "Ramasamy, Loganathan  and
      Bojar, Ond{\v{r}}ej  and
      {\v{Z}}abokrtsk{\'y}, Zden{\v{e}}k",
    booktitle = "Proceedings of the Workshop on Machine Translation and Parsing in {I}ndian Languages",
    month = dec,
    year = "2012",
    address = "Mumbai, India",
    publisher = "The COLING 2012 Organizing Committee",
    url = "https://www.aclweb.org/anthology/W12-5611",
    pages = "113--122",
}
```

```
@Inbook{Eckart2013,
    author={Eckart, Thomas and Quasthoff, Uwe},
    title="{Statistical Corpus and Language Comparison on Comparable Corpora}",
    bookTitle={Building and Using Comparable Corpora},
    year={2013},
    publisher={Springer Berlin Heidelberg},
    address={Berlin, Heidelberg},
    pages={151--165},
    isbn={978-3-642-20128-8},
    doi={10.1007/978-3-642-20128-8_8},
    url={https://doi.org/10.1007/978-3-642-20128-8_8}
}
```

