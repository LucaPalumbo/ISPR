Assignment

Implement from scratch an RBM and apply it to DSET2. The RBM should be implemented fully by you (both training and inference steps) but you are free to use library functions for the rest (e.g. image loading and management, etc.). Implement a generalization of the Contrastive Divergence (CD) learning algorithm that defines the number of steps K of the Gibbs sampling Markov chain runned before collecting the samples to estimate the model expectation. For instance the standard CD learning would be obtained with K=1. Test your models by training two versions of them, one with a small K and one with a medium K (I suggest you do not go over 10 steps), and discuss the differences in performance/behaviour (if any).

Outline of the assigment:

1. Train an RBM with a number of hidden neurons selected by you (single layer) on the MNIST data (use the training set split provided by the website) using CD(K) with two choices of K.

2. Use the trained RBMs to encode a selection of test images (e.g. using one per digit type) using the corresponding activation of the hidden neurons.

3. Train a simple classifier (e.g. any simple classifier in scikit) to recognize the MNIST digits using as inputs their encoding obtained at step 2. Use the standard training/test split. Show a performance metric of your choice in the presentation/handout and use it to confront the two versions of the RBM (obtained with different K).