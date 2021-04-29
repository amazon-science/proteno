## Proteno Spanish Dataset

This dataset contains 4,791 sentences for text normalization.  There are two Python pickled lists containing tokenized unnormalized sentences (unnorm_list.pkl) and their corresponding normalizations (norm_list.pkl).  Every token that needs to be normalized (expanded) is surrounded with <error> tags in the normalization list with its corresponding unnormalized token. The normalizations also have lang id tags when text from a different language is present along with Spanish. Foreign language text was removed and the models are trained on only Spanish text. 
  
E.g., 
Normalized:  <lang id="en">Transworld Publishers Ltd. Londres,</lang> <error what="mil novecientos noventa y nueve">1999</error>.Taylor,P.<error what="mil  novecientos noventa y seis"> 1996</error>. 

Tokenized unnormalized (after foreign language text removal): ['1999', '.', 'taylor', ',', 'p', '.', '1996', '.'] 

Normalized to unnormalized mapping: <error what="mil novecientos noventa y nueve">1999</error> => Unnormallized token: 1999 Normalization: "mil novecientos noventa y nueve".

First 60% of the data was used for training Proteno and the the models were evaluated on the other 40%.

## License
This dataset is licensed under CC-BY-SA License.


