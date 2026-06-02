Skin Lesion Classification (ISIC Dataset)
Dataset
ISIC dataset used
~2,000 images
9 skin lesion classes
Random split used



1. Basic CNN
Simple convolutional neural network
Basic data augmentation used
Adam optimizer used
Accuracy: ~33%



2. ResNet-18
10 epochs
Pretrained ResNet-18 model used
Better data augmentation (jitter + normalization)
Weighted loss used for imbalance
Adam optimizer used
Accuracy: ~33%



3. ResNet-50 (Best Model)
Pretrained ResNet-50 model used
Strong augmentation + normalization
Weighted CrossEntropyLoss + label smoothing
AdamW optimizer used
Cosine Annealing learning rate scheduler used
Random split used  -> for splitting the data into training and validation
25 epochs training
Accuracy: 58.47%



Summary
Simple CNN → low performance (~33%)
ResNet-18 → no major improvement (~33%)
ResNet-50 → best result (~58%)