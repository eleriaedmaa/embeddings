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
CBOW  | 100| 5| 10| 20| <a href="https://eestikeeleinstituut-my.sharepoint.com/:u:/g/personal/eleri_aedmaa_eki_ee/EfUe4o-XqdFNvtVTccchX_ABXCz_rvV2siqBPH1JdqVVUw?e=bJzw0S" download>cbow\_100\_5\_10\_20.zip</a>
CBOW  | 150| 15| 10| 20| <a href="http://193.40.33.66/pretrained/cbow_150_15_10_20.zip">cbow\_150\_15\_10\_20.zip</a>
CBOW  | 150| 15| 5| 20| <a href="http://193.40.33.66/pretrained/cbow_150_15_5_20.zip">cbow\_150\_15\_5\_20.zip</a>
CBOW  | 150| 5| 10| 20| <a href="http://193.40.33.66/pretrained/cbow_150_5_10_20.zip">cbow\_150\_5\_10\_20.zip</a>
CBOW  | 150| 5| 10| 5| <a href="http://193.40.33.66/pretrained/cbow_150_5_10_5.zip">cbow\_150\_5\_10\_5.zip</a>
CBOW  | 150| 5| 5| 20| <a href="http://193.40.33.66/pretrained/cbow_150_5_5_20.zip">cbow\_150\_5\_5\_20.zip</a>
CBOW  | 300| 10| 10| 5| <a href="http://193.40.33.66/pretrained/cbow_300_10_10_5.zip">cbow\_300\_10\_10\_5.zip</a>
CBOW  | 300| 15| 10| 20| <a href="http://193.40.33.66/pretrained/cbow_300_15_10_20.zip">cbow\_300\_15\_10\_20.zip</a>
CBOW  | 300| 15| 10| 5| <a href="http://193.40.33.66/pretrained/cbow_300_15_10_5.zip">cbow\_300\_15\_10\_5.zip</a>
CBOW  | 300| 1| 10| 20| <a href="http://193.40.33.66/pretrained/cbow_300_1_10_20.zip">cbow\_300\_1\_10\_20.zip</a>
CBOW  | 300| 30| 10| 20| <a href="http://193.40.33.66/pretrained/cbow_300_30_10_20.zip">cbow\_300\_30\_10\_20.zip</a>
CBOW  | 300| 5| 10| 10| <a href="https://eestikeeleinstituut-my.sharepoint.com/:u:/g/personal/eleri_aedmaa_eki_ee/EfUe4o-XqdFNvtVTccchX_ABXCz_rvV2siqBPH1JdqVVUw?e=egaDRb">cbow\_300\_5\_10\_10.zip</a>
CBOW  | 300| 5| 10| 20| <a href="http://193.40.33.66/pretrained/cbow_300_5_10_20.zip">cbow\_300\_5\_10\_20.zip</a>
CBOW  | 300| 5| 10| 5| <a href="http://193.40.33.66/pretrained/cbow_300_5_10_5.zip">cbow\_300\_5\_10\_5.zip</a>
CBOW  | 300| 5| 15| 5| <a href="http://193.40.33.66/pretrained/cbow_300_5_15_5.zip">cbow\_300\_5\_15\_5.zip</a>
CBOW  | 300| 5| 2| 20| <a href="http://193.40.33.66/pretrained/cbow_300_5_2_20.zip">cbow\_300\_5\_2\_20.zip</a>
CBOW  | 300| 5| 5| 20| <a href="http://193.40.33.66/pretrained/cbow_300_5_5_20.zip">cbow\_300\_5\_5\_20.zip</a>
CBOW  | 300| 5| 5| 5| <a href="http://193.40.33.66/pretrained/cbow_300_5_5_5.zip">cbow\_300\_5\_5\_5.zip</a>
CBOW  | 450| 5| 10| 5| <a href="http://193.40.33.66/pretrained/cbow_450_5_10_5.zip">cbow\_450\_5\_10\_5.zip</a>
CBOW  | 750| 5| 10| 20| <a href="http://193.40.33.66/pretrained/cbow_750_5_10_20.zip">cbow\_750\_5\_10\_20.zip</a>
Skip-gram | 150| 5| 10| 5| <a href="http://193.40.33.66/pretrained/skip_150_5_10_5.zip">skip\_150\_5\_10\_5.zip</a>
Skip-gram | 300| 10| 10| 5| <a href="http://193.40.33.66/pretrained/skip_300_10_10_5.zip">skip\_300\_10\_10\_5.zip</a>
Skip-gram | 300| 15| 10| 5| <a href="http://193.40.33.66/pretrained/skip_300_15_10_5.zip">skip\_300\_15\_10\_5.zip</a>
Skip-gram | 300| 5| 10| 10| <a href="http://193.40.33.66/pretrained/skip_300_5_10_10.zip">skip\_300\_5\_10\_10.zip</a>
Skip-gram | 300| 5| 10| 20| <a href="http://193.40.33.66/pretrained/skip_300_5_10_20.zip">skip\_300\_5\_10\_20.zip</a>
Skip-gram | 300| 5| 10| 5| <a href="http://193.40.33.66/pretrained/skip_300_5_10_5.zip">skip\_300\_5\_10\_5.zip</a>
Skip-gram | 300| 5| 15| 5| <a href="http://193.40.33.66/pretrained/skip_300_5_15_5.zip">skip\_300\_5\_15\_5.zip</a>
Skip-gram | 300| 5| 5| 5| <a href="http://193.40.33.66/pretrained/skip_300_5_5_5.zip">skip\_300\_5\_5\_5.zip</a>
Skip-gram | 450| 5| 10| 5| <a href="">skip\_450\_5\_10\_5.zip</a>

-----

## Credits ##

Author: Eleri Aedmaa (Institute of Estonian and General Linguistics, University of Tartu) 

This work was carried out in the High Performance Computing Center of University of Tartu.




## References ##


[1] Tomas Mikolov, Kai Chen, Greg Corrado, and Jeffrey Dean. [Efficient Estimation of Word Representations in Vector Space](https://arxiv.org/pdf/1301.3781.pdf). In Proceedings of Workshop at ICLR, 2013.

[2] Tomas Mikolov, Ilya Sutskever, Kai Chen, Greg Corrado, and Jeffrey Dean. [Distributed Representations of Words and Phrases and their Compositionality](http://papers.nips.cc/paper/5021-distributed-representations-of-words-and-phrases-and-their-compositionality.pdf). In Proceedings of NIPS, 2013.

[3] Tomas Mikolov, Wen-tau Yih, and Geoffrey Zweig. [Linguistic Regularities in Continuous Space Word Representations](https://www.aclweb.org/anthology/N13-1090). In Proceedings of NAACL HLT, 2013.

[4] Maria Pelevina, Nikolay Arefyev, Chris Biemann, and Alexander Panchenko. [Making Sense of Word Embeddings](http://aclweb.org/anthology/W16-1620). In Proceedings of the 1st Workshop on Representation Learning for NLP, 2016.
