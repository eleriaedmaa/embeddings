# Pretrained word and multi-sense embeddings for Estonian #

----

Corpus: all embeddings are trained on lemmatized [etTenTen: Corpus of the Estonian Web](https://doi.org/10.15155/1-00-0000-0000-0000-0012el).

Word embeddings are trained with [word2vec](https://code.google.com/archive/p/word2vec/)<sup>[[1]](https://arxiv.org/pdf/1301.3781.pdf), [[2]](http://papers.nips.cc/paper/5021-distributed-representations-of-words-and-phrases-and-their-compositionality.pdf), [[3]](https://www.aclweb.org/anthology/N13-1090)</sup>.

Sense embeddings are trained with [SenseGram](https://github.com/uhh-lt/sensegram)<sup>[[4]](http://aclweb.org/anthology/W16-1620)</sup>.

Sense inventory is induced from word embeddings.

----

##Parameters##

Models were trained using various parameter settings. The values of architecture, number of dimensions, window size, minimum frequency threshold and number of iterations vary, but other parameters follow default values declared [here](https://github.com/uhh-lt/sensegram). 


The exact values are declared in the name of the folders containing three output files:

.word_vectors - word vectors in the word2vec text format

.sense_vectors - sense vectors in the word2vec text format

.sense_vectors.inventory.csv - sense probabilities in TSV format



The **format** of the folder name is following: *architecture\_dimensions\_window\_minc\_iter.zip*:

* architecture: - CBOW or Skip-gram: *cbow* or *skip*; 

* dimensions - number of dimensions: *100*, *150*, *300*, *450* or *750*;

* window - window size: *5*, *10*, *15* or *30*;

* minc - minimum count threshold: *2*, *5*, *10* or *15*; 

* iter - number of iterations: *5*, *10* or *20*.

---

## Download ##

architecture  | dimensions   | window size  | mininum count  | iterations  | download 
------------- | -------------| -------------| -------------| -------------| -------------
CBOW  | 100| 5| 10| 20| <a href="https://eestikeeleinstituut-my.sharepoint.com/:u:/g/personal/eleri_aedmaa_eki_ee/EUh-DeqGZQJItw4iB0L7EkIBrIC_5xSfFJbuTP3ap-neeg?e=I3cp7j" download>cbow\_100\_5\_10\_20.zip</a>
CBOW  | 150| 15| 10| 20| <a href="https://eestikeeleinstituut-my.sharepoint.com/:u:/g/personal/eleri_aedmaa_eki_ee/EQ1AB2Uo-HFAgbGVWjhoFcwB70hnbrpbyrZn41fNAC5QGg?e=9oBvpc">cbow\_150\_15\_10\_20.zip</a>
CBOW  | 150| 15| 5| 20| <a href="https://eestikeeleinstituut-my.sharepoint.com/:u:/g/personal/eleri_aedmaa_eki_ee/EcUBCn3tpPdIiSlI-q2qJYEBlldABbnT5m0b2JZbenSs_Q?e=Vq1euY">cbow\_150\_15\_5\_20.zip</a>
CBOW  | 150| 5| 10| 20| <a href="https://eestikeeleinstituut-my.sharepoint.com/:u:/g/personal/eleri_aedmaa_eki_ee/EWNkokyPDFZOg45nB5BbicoBcPg5vB7RiVEFhmMg_2dBFw?e=sVotgx">cbow\_150\_5\_10\_20.zip</a>
CBOW  | 150| 5| 10| 5| <a href="https://eestikeeleinstituut-my.sharepoint.com/:u:/g/personal/eleri_aedmaa_eki_ee/EWxN2TluQrxBhmrvWTwtzjsBO-Yupny7f3XfnHk4KrooIg?e=FhfpY8">cbow\_150\_5\_10\_5.zip</a>
CBOW  | 150| 5| 5| 20| <a href="https://eestikeeleinstituut-my.sharepoint.com/:u:/g/personal/eleri_aedmaa_eki_ee/EdUaCesBytlJtQBgWdrarRYBs7GWpZ8bEI6U_J3cSFmMmQ?e=RLJr2T">cbow\_150\_5\_5\_20.zip</a>
CBOW  | 300| 10| 10| 5| <a href="https://eestikeeleinstituut-my.sharepoint.com/:u:/g/personal/eleri_aedmaa_eki_ee/EWQ57WjGgVhDvwBfCAuqbbsBkM-4kcnAx6Oos5fNddfn7g?e=1pVTSy">cbow\_300\_10\_10\_5.zip</a>
CBOW  | 300| 15| 10| 20| <a href="https://eestikeeleinstituut-my.sharepoint.com/:u:/g/personal/eleri_aedmaa_eki_ee/EW2of4c6PztCsD9eDlF08GQBEfxqwrLLlswZyLtf_GhEJw?e=pONxG3">cbow\_300\_15\_10\_20.zip</a>
CBOW  | 300| 15| 10| 5| <a href="https://eestikeeleinstituut-my.sharepoint.com/:u:/g/personal/eleri_aedmaa_eki_ee/ERB8y8z8YwFLhQeTkuc1QWgBEvVgWxVCWNbV9OqU6eErOQ?e=oTPwXS">cbow\_300\_15\_10\_5.zip</a>
CBOW  | 300| 1| 10| 20| <a href="https://eestikeeleinstituut-my.sharepoint.com/:u:/g/personal/eleri_aedmaa_eki_ee/EfQyiYXBVA9EjIarh4nqKUcBQsihe4A1-yBUAAl2pWJU2A?e=CwMcZV">cbow\_300\_1\_10\_20.zip</a>
CBOW  | 300| 30| 10| 20| <a href="https://eestikeeleinstituut-my.sharepoint.com/:u:/g/personal/eleri_aedmaa_eki_ee/EfyuqPQpPa9NryJJoa6neIsBDJrpHdm7Bx5u5AaU9GwC1w?e=V4UKJe">cbow\_300\_30\_10\_20.zip</a>
CBOW  | 300| 5| 10| 10| <a href="https://eestikeeleinstituut-my.sharepoint.com/:u:/g/personal/eleri_aedmaa_eki_ee/EQJOVsGpbqBCup0bOnrapQkBZTUerpMnovx2sUS6ZEHyCw?e=P0VtBd">cbow\_300\_5\_10\_10.zip</a>
CBOW  | 300| 5| 10| 20| <a href="https://eestikeeleinstituut-my.sharepoint.com/:u:/g/personal/eleri_aedmaa_eki_ee/Eb8OA_yRDmtCqcYrEHSEAe4BnWspfRm9oExLYtmQtD_eMQ?e=Ypr2kd">cbow\_300\_5\_10\_20.zip</a>
CBOW  | 300| 5| 10| 5| <a href="https://eestikeeleinstituut-my.sharepoint.com/:u:/g/personal/eleri_aedmaa_eki_ee/EY0-W_xz1gZAnPWKnfIcOD4BjErX6qV1psPIcWhtjOoswA?e=mQd2ES">cbow\_300\_5\_10\_5.zip</a>
CBOW  | 300| 5| 15| 5| <a href="https://eestikeeleinstituut-my.sharepoint.com/:u:/g/personal/eleri_aedmaa_eki_ee/Ebm6fIszHsZBuAzHktn51OkBtTkSj-SPowRFhFs02fX7bQ?e=f33iuq">cbow\_300\_5\_15\_5.zip</a>
CBOW  | 300| 5| 2| 20| <a href="https://eestikeeleinstituut-my.sharepoint.com/:u:/g/personal/eleri_aedmaa_eki_ee/EX0GqChNF1RAtxHFdJLRl9MB1nv71qiKxhhr18tEXZBXyw?e=IofWTE">cbow\_300\_5\_2\_20.zip</a>
CBOW  | 300| 5| 5| 20| <a href="https://eestikeeleinstituut-my.sharepoint.com/:u:/g/personal/eleri_aedmaa_eki_ee/Ef7DNh3_FDlGgBoeD0kOwEQBfPqY6rU_3CojZK_m71NaKQ?e=ZPtSA1">cbow\_300\_5\_5\_20.zip</a>
CBOW  | 300| 5| 5| 5| <a href="https://eestikeeleinstituut-my.sharepoint.com/:u:/g/personal/eleri_aedmaa_eki_ee/ERh6rJzv60VAp4cmvao_O-EBrM1p1rrkj5gTVoGlybI_Qg?e=fP6cb6">cbow\_300\_5\_5\_5.zip</a>
CBOW  | 450| 5| 10| 5| <a href="https://eestikeeleinstituut-my.sharepoint.com/:u:/g/personal/eleri_aedmaa_eki_ee/EYc5IYTfm4BOiObuembKVQgBQGroppwfogvUhhhcijqAwA?e=Ofy4ep">cbow\_450\_5\_10\_5.zip</a>
CBOW  | 750| 5| 10| 20| <a href="https://eestikeeleinstituut-my.sharepoint.com/:u:/g/personal/eleri_aedmaa_eki_ee/EYMl5Ah4pWxEtRV8aVwxgQABOy8NjH76B9N03necVKD_Rg?e=XcQpOw">cbow\_750\_5\_10\_20.zip</a>
Skip-gram | 150| 5| 10| 5| <a href="https://eestikeeleinstituut-my.sharepoint.com/:u:/g/personal/eleri_aedmaa_eki_ee/ERRS139a7rNGnrDUQaZ1Jy8BE6pqOWGrpfR98CqURKY5yQ?e=FCEYgP">skip\_150\_5\_10\_5.zip</a>
Skip-gram | 300| 10| 10| 5| <a href="https://eestikeeleinstituut-my.sharepoint.com/:u:/g/personal/eleri_aedmaa_eki_ee/EWbRr9fyQKFNv-5-4xipERUBXYzBH3hWSkzgYOe5s826kw?e=q8oF7B">skip\_300\_10\_10\_5.zip</a>
Skip-gram | 300| 15| 10| 5| <a href="https://eestikeeleinstituut-my.sharepoint.com/:u:/g/personal/eleri_aedmaa_eki_ee/ET6cHakIqaJEp6knsJa179kBjIxxiulKF6XYz3jyOKaoSA?e=A9M4d2">skip\_300\_15\_10\_5.zip</a>
Skip-gram | 300| 5| 10| 10| <a href="https://eestikeeleinstituut-my.sharepoint.com/:u:/g/personal/eleri_aedmaa_eki_ee/EeCD3Xi5Mb1MmS0kwVOAsa0BnSt0QAspiK8QyAvM78o1Bg?e=sUR0yF">skip\_300\_5\_10\_10.zip</a>
Skip-gram | 300| 5| 10| 20| <a href="https://eestikeeleinstituut-my.sharepoint.com/:u:/g/personal/eleri_aedmaa_eki_ee/ERk-w-2CozZBmX5ojuMc8Q8B1S3tKz-gsUc0NHYOkyGqgw?e=zPG9v0">skip\_300\_5\_10\_20.zip</a>
Skip-gram | 300| 5| 10| 5| <a href="https://eestikeeleinstituut-my.sharepoint.com/:u:/g/personal/eleri_aedmaa_eki_ee/EXnBU8JtnyxMtFJRFqBmvW4BQeGa63TN0czTnv5Gjz76gw?e=7kAmUK">skip\_300\_5\_10\_5.zip</a>
Skip-gram | 300| 5| 15| 5| <a href="https://eestikeeleinstituut-my.sharepoint.com/:u:/g/personal/eleri_aedmaa_eki_ee/EVZRI_imAZlFsAK_01o-q58BzhwJxfhLWXhU4kAzk7FB5A?e=IJm3RK">skip\_300\_5\_15\_5.zip</a>
Skip-gram | 300| 5| 5| 5| <a href="https://eestikeeleinstituut-my.sharepoint.com/:u:/g/personal/eleri_aedmaa_eki_ee/ESJVVRish9FDmyT2RoKeT0cBpvu_sF8HzB515HYAPBgjSQ?e=3BKWQf">skip\_300\_5\_5\_5.zip</a>
Skip-gram | 450| 5| 10| 5| <a href="https://eestikeeleinstituut-my.sharepoint.com/:u:/g/personal/eleri_aedmaa_eki_ee/EenCeNgsurRMgMCuWxvNlbQBrRE9rAkU8YRardUCSV7jIg?e=4C4gqi">skip\_450\_5\_10\_5.zip</a>


-----

## Credits ##

Author: Eleri Aedmaa (Institute of Estonian and General Linguistics, University of Tartu) 

This work was carried out in the High Performance Computing Center of University of Tartu.



## References ##


[1] Tomas Mikolov, Kai Chen, Greg Corrado, and Jeffrey Dean. [Efficient Estimation of Word Representations in Vector Space](https://arxiv.org/pdf/1301.3781.pdf). In Proceedings of Workshop at ICLR, 2013.

[2] Tomas Mikolov, Ilya Sutskever, Kai Chen, Greg Corrado, and Jeffrey Dean. [Distributed Representations of Words and Phrases and their Compositionality](http://papers.nips.cc/paper/5021-distributed-representations-of-words-and-phrases-and-their-compositionality.pdf). In Proceedings of NIPS, 2013.

[3] Tomas Mikolov, Wen-tau Yih, and Geoffrey Zweig. [Linguistic Regularities in Continuous Space Word Representations](https://www.aclweb.org/anthology/N13-1090). In Proceedings of NAACL HLT, 2013.

[4] Maria Pelevina, Nikolay Arefyev, Chris Biemann, and Alexander Panchenko. [Making Sense of Word Embeddings](http://aclweb.org/anthology/W16-1620). In Proceedings of the 1st Workshop on Representation Learning for NLP, 2016.
