# Week 1

## Result from the MNIST
- Have tried several network architectures. All the tried architectures are listed in the 1st_DNN_trails.ipynb
- Among the tried architectures the one in this file gives better Evaluation/Testing Accuracy.

- 2 Convolutions (32,64)
- MaxPooling
- Convolutions (128)
- 1x1 Convolution
- Flatten
- Activation Function

In KERAS, Convolution can be applied via 2D methods 
1. Conv2D
2. Convolution2D
w.r.t KERAS documentation, one is alias of other.

But the with same architecture Conv2D gives better validation accuracy. (Ran for multiple iterations). 

From the model evaluation results, 

I am presenting the 'model_2' accuracy as result.

### Result - 99.1%

-------------------------------------

## Answers to the Questions
 
1. Convolution
Calculating the weighted sum of the elements in a matrix by running over a filter matrix over a target matrix, In general filter matrix is smaller than the target matrix.

2. Filters/Kernels - They are used to apply some/any specific effect(s) on the target. This resultant process is called Convolution. Generally its a square matrix having odd number of rows/columns. Typically they are matrices. Example - Blur filter

3. Epochs - It describes number of times a algorithm iterates(trains) on the complete training data

4. 1x1 Convolution - Convolution with 1x1 matrix is called as 1x1 convolution. Its used to either increase(DeConvolution)/decrease(Convolution) the depth of the mutli dimensional target(can say image/video). Decreasing(Convolving) will result in the Dimensionality reduction.

5. 3x3 Convolution - Convolution with 3x3 matrix is called as 3x3 convolution. In geneal several small convoulutions is applied to source matrix(image) to identify several features. 

6. Feature Maps - It is 'Resultant of the Convolution'. In general it maps any particular feature(based on the filter, if blur filter is applied the resultant/target matrix)would be blurred portion of the Source matrix)

7. Activation Function - Its defines the output of a layer/node/neuron. Typically a mathematical function the inputs are fed to function and output is expected

8. Receptive Field - The area where the forward  neuron/ode/layer can have information about the networks trailing neuron/nodes/layers. After applying convolution, the forward layers can have information about the trailing layers.
