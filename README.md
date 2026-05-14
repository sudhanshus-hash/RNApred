# RNApred: SVM-Based Prediction of RNA-Binding Proteins Using Binding Residues and Evolutionary Information

RNApred is a computational tool developed for predicting RNA-binding proteins from amino acid sequences.

RNA-binding proteins play important roles in transcription, RNA processing, gene regulation, RNA stability, RNA transport, and cellular localization. RNApred uses support vector machine-based models, RNA-binding residue information, and evolutionary profiles to classify proteins as RNA-binding or non-RNA-binding proteins.

Web Server: https://webs.iiitd.edu.in/raghava/rnapred



## Citation

Kumar, M., Gromiha, M. M., and Raghava, G. P. S. SVM based prediction of RNA-binding proteins using binding residues and evolutionary information. Journal of Molecular Recognition, 24, 303-313, 2011.

https://doi.org/10.1002/jmr.1061


This tool and dataset is also available on Zenodo at https://doi.org/10.5281/zenodo.20177962



## About the Research

RNA-binding proteins are proteins that interact with RNA molecules and regulate many essential biological processes. They are involved in ribosome function, spliceosome activity, RNA catalysis, transcriptional regulation, RNA processing, and gene expression control.

Experimental identification of RNA-binding proteins can be difficult and time-consuming. Therefore, RNApred was developed as a sequence-based computational method to predict whether a protein is likely to bind RNA.

Data Compilation: The main dataset contained 377 RNA-binding proteins and an equal number of non-RNA-binding proteins. The study also used independent datasets to evaluate the real-life performance of the prediction models.

Methodology: RNApred uses support vector machine models trained on amino acid composition, dipeptide composition, four-part amino acid composition, and evolutionary information in the form of PSSM profiles. The final hybrid method combines RNA-binding residue prediction using PPRINT with PSSM-400-based SVM prediction.



## Key Features

### 1. RNA-Binding Protein Prediction

Predictive Modeling: Allows users to submit protein sequences and predict whether they are RNA-binding or non-RNA-binding proteins.

Amino Acid Composition Model: The amino acid composition-based SVM model achieved MCC 0.60.

Dipeptide Composition Model: The dipeptide composition-based model achieved MCC 0.46.

Four-Part Composition Model: The four-part amino acid composition-based model achieved MCC 0.53.

Evolutionary Information Model: The PSSM-400-based SVM model achieved MCC 0.62.

Hybrid Model: The best hybrid approach achieved MCC 0.66 by combining RNA-binding residue prediction and evolutionary information.



### 2. Binding Residue and Evolutionary Information

PPRINT-Based Prediction: The method uses PPRINT to predict RNA-binding residues in a protein sequence.

PSSM-400 Features: Evolutionary information is extracted from PSI-BLAST position-specific scoring matrices and converted into fixed-length 400-dimensional vectors.

Hybrid Prediction Strategy: The final method uses predicted RNA-binding residue percentage as an initial filter and applies the PSSM-400 SVM model for remaining cases.

Independent Evaluation: The model was tested on independent datasets, showing reliable performance beyond cross-validation.



### 3. RNA-Binding Protein Subclassification

Sub-Class Prediction: RNApred also supports classification of RNA-binding proteins into major RNA-binding subclasses.

The study developed models for:

- rRNA-binding proteins
- tRNA-binding proteins
- mRNA-binding proteins

The rRNA-binding protein model showed the best subclassification performance, achieving accuracy of 90.14% and MCC 0.77.



## Applications

RNA-Binding Protein Annotation: RNApred can help identify RNA-binding proteins from newly sequenced protein datasets.

Functional Genomics: The tool can support annotation of proteins involved in RNA metabolism and gene regulation.

Transcriptome Regulation Studies: RNApred can help study proteins involved in RNA processing, RNA stability, RNA transport, and post-transcriptional regulation.

Protein Function Prediction: The method can assist in predicting molecular function when similarity-based annotation fails.

RNA-Protein Interaction Research: RNApred provides a computational framework for studying sequence-level features associated with RNA-binding proteins.



## Contact and Authors

Prof. Gajendra P. S. Raghava  
Corresponding Author  

Email: raghava@iiitd.ac.in

Department of Computational Biology, Indraprastha Institute of Information Technology (IIIT Delhi), New Delhi, India. 



## Support

This work was supported by grants from the Council of Scientific and Industrial Research and the Department of Biotechnology, Government of India.
