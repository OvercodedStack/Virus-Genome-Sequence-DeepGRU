# Virus-Genome-Sequence-DeepGRU

This repository is a collection of work that I did for a course that I did at UCF called CAP 6545 Machine Learning with Bioinformatics. This is forking some code derivied from the original DeepGRU paper by Maghoumi at https://github.com/Maghoumi/DeepGRU . I also used some code to start off derivived from advice and preview code by Austin Mathew, however all of this implementation is roughly standard to the DeepGRU implementation, however the code had to be adjusted in order to provide some of the results presented in my end-report for the class

# What can this package offer? 

This package offers DeepGRU adapted to bring in data, learn it through an autoencoder, and test given a dataset. Genome sequences are based on 4 different types of nucleotypes that are used to build life from and learn the type of species's dna. In this case, the targetted goal of DeepGRU was to attempt to learn which sequences of data are based for one type of species and which ones correlate to which species. For application and relevancy, there was a paper by Gurjit S Randhawa that used machine learning and COVID 19 as a basis for comparative genoming, a part of which this package is attempting to target. As such what this package can offer is as follows:

- Comparing genones by training and testing on data
- Loading a series of sequences and learning them and testing them. Preloads them using the appropiate nucleotype organization
- Uses CUDA for training and testing on the genome sequencing

# What needs to be done?

A lot, basically it needs an easier way to load data, preferrably thorugh a GUI or selection box, a better way to control which experiments are selected and which cases are needed to manipulate DeepGRU performance. 

One particular problem about this package is performance, DeepGRU isn't remarkably optimized and tends to require a lot of resources. Since my own computer as stated in the report paper is very beefy, I would suggest the following at minium to run the package:

- At least 32 GB of RAM
- At least 8GB of VRAM (2080 GeForce)
- At least a gen 10+ Intel processor or equivalent.
- SDD for data hard-disking to improve performance. 

# Shortcomings

Unfortunately because of lack of time at the time of the class and even now, most of the code results I did to give the results show in the report had to be done by hand, that means that if there were more layers or less batch size used, I had to manually go into the code and change it. I haven't had the code to change its implementation yet so this is going to have to stay as it. 


# References

[1] Gurjit S Randhawa, Maximillian PM Soltysiak, Hadi El Roz, Camila PE
de Souza, Kathleen A Hill, and Lila Kari. Machine learning using intrinsic
genomic signatures for rapid classification of novel pathogens: Covid-19 case
study. Plos one, 15(4):e0232391, 2020

[2] Mehran Maghoumi and Joseph J LaViola. Deepgru: Deep gesture recognition
utility. In International Symposium on Visual Computing, pp. 16–31. Springer,
2019.
