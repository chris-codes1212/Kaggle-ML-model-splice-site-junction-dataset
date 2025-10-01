# DNA Splice Junction Machine Learning Clasifier

### Technical Background
Splice sites are the bookends of introns to be removed. There are two main components of splice sites (the two ends); first there is the Exon-Intron site (EI site) which marks the end of an exon and beginning of an intron to be removed, and then there is the Intron-Exon site (IE site) which marks the end of the intron to be removed and the beginning of a new exon to be merged together with the one at the EI site. 

### Dataset
The Splice-Junction Gene Sequences Dataset on Kaggle contains DNA samples (60 nucleotides long) from 1000 randomly selected individuals. The first 180 columns represent the nucleotides present at each location (broken out into patterns of 3 for each letter), and the last column contains the classification of the sequence as either containing an IE site, an EI site, or neither. (https://www.kaggle.com/datasets/muhammetvarl/splicejunction-gene-sequences-dataset)

### Goal
The goal is to create a classification model that can determine if a 60 nucleotide sequence contains an IE site, EI site or neither.
Exons are the coding DNA regions, and Introns are the regions that are removed.


### Methods 
For this project, I have created 3 shallow learning models using cross validation to determine the best hyperparameters for each model. The first model is a random forest classifier, the second is a gradient boost classifier (from sklearn), and the last uses an xgboost classifier.

### Future Considerations
IE sites are typically recognized by the GT dinucleotide and the EI site are typically recognized by the AG dinucelotide. There are other patterns/traits of introns and exons that would help a model recognize whether or not a region contains an IE or EI site, and a future consideration would be to build a Knowledge-Based Artificial Neural Network (KBANN) classification model 
