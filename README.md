# ERAV2_Session7

# Stage 1 - Determine model skeleton
## Target:
1. Get the set-up right
2. Set Transforms
3. Set Data Loader
4. Set Basic skeleton 
5. Make model lighter

## Results:
1. Parameters: 62k
2. Best Training Accuracy: 99.04
3. Best Test Accuracy: 99.03

## Analysis:
1. Heavy Model for such a problem
2. Model is over-fitting although the gap is reduced

# Stage 2 - Add regularization, Batch Normalization , increase capacity and use GAP
## Target:
1. Recitfied Max pooling location from previous stage - only one max pool layer after RF 5 
2. Add layers at the end after GAP layer
3. Add Regularization - Dropout and batch normalization
4. Make model lighter < 8k 

## Results:
1. Parameters: 7,878
2. Best Training Accuracy: 99.09
3. Best Test Accuracy: 99.14

##Analysis:
1. No overfitting
2. Test accuarcay is oscillating at final epoch, adding LR schedular or Image Augumentation might help

# Stage 3 - Apply Image Augumentation and Fine Tune Learning rate
## Target:
1. Increasing Test Accuracy >= 99.4 % and making it consistent.
2. Add Image Augmentation in Training dataset
3. Add Step LR

## Results:
1. Parameters: 7,878
2. Best Training Accuracy: 99.10
3. Best Test Accuracy: 99.51

##Analysis:

1. No overfitting
2. Test accuracy is stabilised and consistent over last few epochs.
