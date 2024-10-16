## SRX-DTI

Predicting drug-target interactions based on fusing multiple features with data balancing and feature selection techniques
Predicting drug-target interaction (DTI) is an important research area in the field of drug discovery.  This framework proposes a novel drug–target interaction prediction method called SRX-DTI. First, we extract various descriptors from the protein sequences; and the drug is encoded as an FP2 molecular fingerprint. Besides, we present the One-SVM-US technique to deal with imbalanced data. We also developed the FFS-RF algorithm to remove the irrelevant features to obtain the best optimal features. Finally, the balanced dataset with optimal features is given to the XGBoost classifier to identify DTIs. 

![image](https://user-images.githubusercontent.com/72028345/204578716-30f41a3e-0f22-4881-82dc-f0af97e1eb52.png)

## About data
In this research, four golden standard datasets, including enzymes (EN), G-protein-coupled receptors (GPCR), ion channel (IC), and nuclear receptors (NR) released by [Yamanishi et al](http://web.kuicr.kyoto-u.ac.jp/supp/yoshi/drugtarget/).  All these datasets are freely available from [http://web.kuicr.kyoto-u.ac.jp/supp/yoshi/drugtarget/](http://web.kuicr.kyoto-u.ac.jp/supp/yoshi/drugtarget/). 

## Environment Settings
- Python version:  '3.9' or higher

- You have to install the required libraries

## To run the code
- Run ./feature extraction/00-AAC.py: extract AAC descriptor (for other descriptors, just change to related Python code).  
- Run ./NR-run/run.py: make a balanced dataset and feature selection.
- Run ./DTI prediction/DTI_predictor.py: predict drug-target interactions, and evaluate the results with five cross-validations.

# Citation
If you use our source code, dataset, and experiments for your research or development, please cite our paper:
Khojasteh, H., Pirgazi, J., & Ghanbari Sorkhi, A. (2023). Improving prediction of drug-target interactions based on fusing multiple features with data balancing and feature selection techniques. Plos one, 18(8), e0288173.
[https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0288173]

# Contact
If you have any questions, do not hesitate to contact me at `khojasteh.hb@gmail.com`, I will be happy to assist.
