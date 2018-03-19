# cnnSummary
This repository presents the result of a model which use to predict the landmarks on beetle's images.
The model have been run on five parts of beetles: left mandible, right mandible, head, body and pronotum.
The results are evaluated by the statistic methods: Pearson, Spearman, Kendall.
Besides the accuracy of each landmarks are eveluated by consider the predicted location and manual location.

Latex folder contains the descriptions.
Data folder contains the experiment results.

# data folder (#1)
This folder contains the result on beetle database when we train the model (architecture 3)
on each dataset from scratch.

# fine_tuning folder (#2)
This folder contains the result on tete, elytre and pronotum. 
The result have been obtained by fine-tuning a trained model.
To obtain the trained model, the architecture 3 was trained on a combining
dataset of pronotum, head and tete ( 260 images for each).
Then, it used to fine-tune on each dataset without freeze the lower layers.

# fine_tuning_frozen folder (#3)
This folder contained the fine-tuning results with frozen procedure.
(Same procedure with #2 but freeze first of 12 layers)
