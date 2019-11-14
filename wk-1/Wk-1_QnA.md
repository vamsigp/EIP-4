# Week 1
 Answers to the Questions
 
1. Convolution
In NN, applying a filter(can say a matrix) over a target(can say larger matrix). It calculates the weighted sum of all the elements. In general; Calculating the weighted sum of the elements in a matrix by running over a  filter matrix over a target matrix, In general filter matrix is smaller than the target matrix. In the process of convolution 

2. Filters/Kernels - They are used to apply some effects on the target. This resultant process is called Convolution. Generally its a square matrix having odd number of rows/columns. In Image processing they are used to extract features

3. Epochs -  It describes number of times a algorithm iterates(trains) on the complete train data

4. 1x1 Convolution -  Convolution with 1x1 matrix is called as 1x1 convolution. Its used to either increase(DeConvolution)/decrease(Convolution) the depth of the mutli dimensional target(can say image/video). Decreasing(Convolving) will result in the Dimensionality reduction.

5. 3x3 Convolution - Convolution with 3x3 matrix is called as 3x3 convolution. In geneal several small convoulutions shall be applied to source matrix(image) to identify several features. 

6. Feature Maps - It is 'Resultant of the Convolution'. In general it maps any particular feature(based on the filter, if blur filter is applied the resultant/target matrix)would be blurred portion of the Source matrix)

7. Activation Function - Its defines the output of a layer/node/neuron. Typically a mathematical function the inputs are fed to function and output is expected

8. Receptive Field - The area where the forward  neuron/ode/layer can have information about the networks trailing neuron/nodes/layers. After applying convolution, the forward layers can have information about the trailing layers.
