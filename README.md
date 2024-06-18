# Batch Normalization

Batch Normalization (Batch Norm) is a normalization technique applied between the layers of a Neural Network, rather than on the raw data. It operates on mini-batches instead of the full data set. This technique speeds up training and allows for higher learning rates, simplifying the learning process.

#### Key Points
**Internal Covariate Shift:** Batch Norm reduces internal covariate shift, which refers to changes in the input distribution of an internal layer of a Neural Network due to continuous adjustments in weights and multiple computations throughout the training process.

**Example:** In a car rental service model, if we only have data on cars and suddenly include motorbikes, the model might fail to predict motorbike prices accurately. This change in data is termed covariate shift.
####
**Stabilizing Inputs:** By applying Batch Norm, the mean (𝛽) and standard deviation (𝛾) of the layer inputs are kept consistent. This stability reduces the variability in input distributions, providing a more stable foundation for deeper layers during learning.
####
**Regularization Effect:** Batch Norm can have a regularization effect due to the noise introduced when computing over mini-batches. This noise helps combat overfitting, though it is usually small and often used in conjunction with Dropout for better regularization.

Overall, Batch Norm is crucial for faster and more reliable training of deep neural networks by managing internal covariate shifts and providing a regularization effect.

References: https://www.baeldung.com/cs/batch-normalization-cnn#batch-normalization
