## Clustering Project: Anuran Calls MFCCs

This dataset was used in several classifications tasks related to the challenge of anuran species recognition through their calls. 
It is a multilabeldataset with three columns of labels. 
This dataset was created segmenting - 60 audio records belonging to 

- 4 different families, 
- 8 genus, 
- 10 species. 

Each audio corresponds to one specimen (an individual frog), the record ID is also included as an extra column. It is used the spectral entropy and a binary 
cluster method to detect audio frames belonging to each syllable. The segmentation and feature extraction were carried out in Matlab. After the segmentation 
got 7195 syllables, which became instances for train and test the classifier. These records were collected in situ under real noise conditions 
(the background sound). Some species are from the campus of Federal University of Amazonas, Manaus, others from Mata AtlÃ¢ntica, Brazil, and one of them from 
CÃ³rdoba, Argentina. 

Mel-frequency cepstral coefficients (MFCCs) are coefficients that collectively make up an mel-frequency cepstrum (MFC). Due to each syllable has different length, every row (i) was normalized acording to MFCCs_i/(max(abs(MFCCs_i))).


In this project, I did first exploratory data analysis with help of matplotlib and seaborn visualization packages.
I tried to handle outliers by replacing them with each corresponding columns' mean values. 
I applied three different clustering algorithms, these are:

- K-Means
- DBSCAN
- AGNES

At the end of the notebook, you will see the comparison of algorithms. 

I hope you can enjoy while learning :)
