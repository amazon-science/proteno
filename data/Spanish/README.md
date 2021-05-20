## Proteno Spanish Dataset

This dataset contains 4,791 sentences gathered from Wikipedia and annotated for text normalization.  There are two Python pickled lists containing tokenized unnormalized sentences (unnorm_list.pkl) and their corresponding normalizations (norm_list.pkl).  Every token that needs to be normalized is surrounded with <error> tags in the normalization list with its corresponding unnormalized token. The normalizations also have lang id tags when text from a different language is present along with Spanish. Foreign language text was removed and the models are trained on only Spanish text. If the normalized text contains hyperlinks or web address then they are ignored as well for training purposes.

```
E.g.,
  
Normalized Text: 
<lang id="en">Science</lang> <error what="trescientos">300</error>:<error what="veintinueve">29</error><error what="a">–</error><error what="treinta">30</error> Así, la selección femenina podría promover la salud general de las poblaciones en esta especie.

Unnormalized Tokenized Text(after foreign language text removal): 
['300' , ':' , '29' , '–' , '30' , 'así' , ',' , 'la' , 'selección' , 'femenina' , 'podría' , 'promover' , 'la' , 'salud' , 'general' , 'de' , 'las' , 'poblaciones' , 'en' , 'esta' , 'especie' , '.']
  
Normalized to unnormalized token mapping: 
<error what="trescientos">300</error> => Unnormalized token: 300 , Normalization: "trescientos".
```
  
First 60% of the data was used for training Proteno and the models were evaluated on the other 40%.

## License
This dataset is licensed under CC-BY-SA License.
