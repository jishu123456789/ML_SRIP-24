# Animal Image Classification

## Task
The primary task was to perform image classification on the Animal Dataset, consisting of 90 different classes. The tasks were divided into two parts:

1. One Vs All Classification
2. 5 Class Classification Problem

## Datasets
The dataset was initially divided into a training set and a held-out test set. The training set was further split into three parts for 3-fold cross-validation. The final model was evaluated on the held-out test set, which consisted of 12 images.

## Approach
For both classification tasks, we utilized a pre-trained model (ResNet-50) and a custom CNN architecture from scratch:

### For One Vs All Classification:
- Pre-trained model: Trained in 3 folds, with each fold containing 5 epochs.
- Custom CNN: Trained in 3 folds, with 25 epochs each.

### For the 5 Class Classification problem:
- Both pre-trained ResNet-50 and Custom CNN were trained for 3 folds, with each fold containing 20 epochs.

## Results
### Pre-trained Model (One Vs All Classification):
- Achieved accuracy well over 98.5% for all classes, with 100% accuracy for some classes.

### Custom CNN Model (One Vs All Classification):
- High accuracy but low precision. Requires more epochs for a meaningful precision score.

### Pre-trained Model (5 Class Classification):
- Achieved accuracy of over 95%.

### Custom CNN Model (5 Class Classification):
- Low accuracy achieved, only 66%. Requires more training for improved accuracy.

Overall, the pre-trained models demonstrated superior performance compared to the custom CNN models, suggesting the effectiveness of transfer learning for this task. Further tuning and training are required to enhance the performance of custom CNN models.


## DatasetLink 

###
- https://drive.google.com/drive/folders/1vhu3LJ9eYDDQfmUZB62jFRf6PuqMbqr-
- This drive contains the Animal Dataset which contains the testing and training data
