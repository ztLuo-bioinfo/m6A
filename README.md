Independent test dataset
We have uploaded 11 independent test datasets covering various species, including H. sapiens, M. musculus, Chimpanzee, Rhesus, Pig, Rat, Zebrafish, D.melanogaster, S.cerevisiae, etc. Each sample has a sequence length of 101 amino acids. Please adjust the sequence length to the appropriate size according to the requirements of your model.

models
DeepM6ASeq:
The script main_test.py is used to predict if a given sequence contain m6A sites. The required arguments
model_type: cnn-rnn
input_fa: a fasta file for test samples ( the length of sequences should be no more than 101bp)
model_dir: the path of model directory
out_fn: output file
This script ouput the prediction scores for given sequences.
for example:python main_test.py -m cnn-rnn -infa test.fa -md model/dr/256-128_10-5_0_0.5_Y_Y_64_0.001_256_64 -outfn out_fn1

