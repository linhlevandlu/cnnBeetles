# Summary
This repository contains the predicted landmarks on all parts of beetle when we apply the CNN to our problems.
The repository contains the folders corresponding to the results of different scenario test.

# TRAIN_FROM_SCRATCH folder
Contains the results when we run the model from scratch on  five parts of beetles: left mandible, right mandible, head, body and pronotum.
The results are evaluated by the statistic methods: Pearson, Spearman, Kendall.
Besides the accuracy of each landmarks are eveluated by consider the predicted location and manual location.

# FINE_TUNING folder (#2)
This folder contains the result on tete, elytre and pronotum. 
The result have been obtained by fine-tuning a trained model.
To obtain the trained model, the architecture 3 was trained on a combining
dataset of pronotum, head and tete ( 260 images for each).
Then, it used to fine-tune on each dataset without freeze the lower layers.
The main folder in each part is LANDMARKS folder: it contains the manual landmarks and corresponding predicted landmarks in TPS files.

# FINE_TUNING_FROZEN folder (#3)
This folder contained the fine-tuning results with frozen procedure.
(Same procedure with #2 but freeze first of 12 layers)

# LATEX folder
Latex folder contains the descriptions.

