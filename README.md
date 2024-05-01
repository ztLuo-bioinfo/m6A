# Independent test dataset
We have uploaded 11 independent test datasets covering various species, including H. sapiens, M. musculus, Chimpanzee, Rhesus, Pig, Rat, Zebrafish, D.melanogaster, S.cerevisiae, etc. Each sample has a sequence length of 101 amino acids. Please adjust the sequence length to the appropriate size according to the requirements of your model.

# models
## DeepM6ASeq:
The script main_test.py is used to predict if a given sequence contain m6A sites. The required arguments
### Requirements
* Python3
* numpy==1.14.2
* torch==0.4.0a0+0e24630 ( pytorch )
* scikit_learn==0.19.1
### Usage
* model_type: cnn-rnn
* input_fa: a fasta file for test samples ( the length of sequences should be no more than 101bp)
* model_dir: the path of model directory
* out_fn: output file

This script ouput the prediction scores for given sequences. For example:
```bash
python main_test.py -m cnn-rnn -infa test.fa -md model/dr/256-128_10-5_0_0.5_Y_Y_64_0.001_256_64 -outfn out_fn1
```
## m6AGE
m6AGE is a predictor for N6-methyladenosine (m6A) sites identification utilizing sequence characteristics and graph embedding-based geometrical information.
### Requirements
* python 3.7
* conda install numpy, pandas, scikit-learn, biopython, networkx
* pip install catboost, karateclub
### Usage
* pos_fa: positive samples in the training dataset corresponding to the species
* neg_fa: negative samples in the training dataset corresponding to the species
* test_fa: independent test dataset to be evaluated
* dataset: model category
* out: output file

The sequence length of the independent test dataset should be consistent with the training dataset. For example:
```bash
python main.py -pos_fa ./datasets/A101/A101_Train_P.fasta -neg_fa ./datasets/A101/A101_Train_N.fasta -test_fa ./datasets/A101/A101_Test.fasta -dataset A101 -out ./results/A101_results.csv
```











