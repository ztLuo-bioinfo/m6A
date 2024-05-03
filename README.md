# Comprehensive review and assessment of computational methods for predicting N6-methyladenosine sites

## Abstract
N6-methyladenosine (m6A) plays a crucial regulatory role in the control of cellular functions and gene expression. Recent advances in sequencing techniques for transcriptome-wide m6A mapping have ac-celerated the accumulation of m6A site information at single-nucleotide level, providing more high-confidence training data to develop computational approaches for m6A site prediction. However, it is still a major challenge to precisely predict m6A sites using in silico approaches. To advance computational support for m6A site identification, here, we curated 13 up-to-date benchmark datasets from 9 different species (i.e. H. sapiens, M. musculus, Rat, S.cerevisiae, Zebrafish, A. thaliana, Pig, Rhesus and Chim-panzee).This will assist the research community in conducting an unbiased evaluation of alternative ap-proaches and support future research on m6A modification. We revisited 49 computational approaches published since 2015 for m6A site identification, including 29 traditional machine learning-based, 12 deep learning-based, and 8 ensemble learning-based methods. We comprehensively reviewed these computa-tional approaches in terms of their training datasets, calculated features, computational methodologies, performance evaluation strategy, and webserver/software usability. Using these benchmark datasets, we benchmarked 9 predictors with available online websites or stand-alone software, and assessed their prediction performance. We found that deep learning and traditional machine learning–based approaches generally outperformed scoring function–based approaches. In summary, the curated benchmark dataset repository and the systematic assessment in this study serve to inform the design and implementation of state-of-the-art computational approaches for m6A identification and facilitate more rigorous comparison of new methods in the future.

## Independent test dataset
We have uploaded 11 independent test datasets covering various species in `data_all`, including H. sapiens, M. musculus, Chimpanzee, Rhesus, Pig, Rat, Zebrafish, D.melanogaster, S.cerevisiae, etc. Each sample has a sequence length of 101 amino acids. Please adjust the sequence length to the appropriate size according to the requirements of your model.

## Evaluated model address
We have uploaded detailed information for all evaluation models to the `model_all` directory. Researchers can download and review the relevant details on their own. Additionally, for ease of use, we have listed the links to all available models as follows
* DeepM6ASeq: [https://github.com/rreybeyb/DeepM6ASeq](https://github.com/rreybeyb/DeepM6ASeq)
* MASS: [https://github.com/mlcb-thu/MASS](https://github.com/mlcb-thu/MASS)
* TL-Mtehy: [https://github.com/LDWang-dlmu/N6-methyladenine](https://github.com/LDWang-dlmu/N6-methyladenine)
* HMpre: [https://github.com/Zhixun-Zhao/HMpre](https://github.com/Zhixun-Zhao/HMpre)
* bCNN: [https://github.com/Naeem-jbnu/RNA_Modification_Sites](https://github.com/Naeem-jbnu/RNA_Modification_Sites)
* m6A-NeuralTool: [http://nsclbio.jbnu.ac.kr/tools/m6A-NeuralTool/](http://nsclbio.jbnu.ac.kr/tools/m6A-NeuralTool/)
* MultiRM: [https://github.com/Tsedao/MultiRM](https://github.com/Tsedao/MultiRM)
* iMethyl-Deep: [https://github.com/abdul-bioinfo/iMethyl-deep](https://github.com/abdul-bioinfo/iMethyl-deep)

Interested researchers can evaluate the models by following the detailed instructions available on the official webserver/github of each model.









