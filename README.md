# EDNet4JDPEI

This repository contains the source code of the paper "Efficient Encoder-Decoder Architecture-Based Modeling for Joint Drug-Protein Entities and Interactions Extraction" published in BIBM 2022.

### Datasets ###

DrugProt datasets used for experiments in the paper can be downloaded from the following link:

https://drive.google.com/drive/folders/1YjD9T4ySu-lKNu5yKoWoGHl7XLeJ0Oew?usp=sharing

### Requirements ###

1) python 3.7
2) pytorch 1.9
3) CUDA 11.3

### How to run ###

#### Word Decoding Model ####

python word_decoder.py gpu_id random_seed source_data_dir target_data_dit train/test

python word_decoder.py 0,1,2 1027 DrugProt/data/ DrugProt/data/word_decode_model train

python word_decoder.py 0,1,2 1027 DrugProt/data/ DrugProt/data/word_decode_model test

#### Pointer Network-based Decoding Model #### 

python ptrnet_decoder.py gpu_id random_seed source_data_dir target_data_dit train/test

python ptrnet_decoder.py 0,1,2 1027 DrugProt/data/ DrugProt/data/ptrnet_decode_model train

python ptrnet_decoder.py 0,1,2 1027 DrugProt/data/ DrugProt/data/ptrnet_decode_model test


