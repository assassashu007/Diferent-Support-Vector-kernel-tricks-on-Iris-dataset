# Diferent-Support-Vector-kernel-tricks-on-Iris-dataset

Support Vector Machine aka SVM in Machine Learning is used to find the hyperplane that best seggregates the examples into differnt classes.

Dimention of Hyperplane = ( number of classes - 1 )

In SVM we convert data or vectors in low dimentional space to data or vectors in high dimentional space.

Kernel Tricks are different techniques or tricks used in SVM for conversion of data.


Math behind every kernel is as follows:

1)Radial Basis Function Kernel(RBF):   

        k(x1, x2) = exp( -gamma * ( || x1 -x2||^2 ) )
        
    where value of gamma determines how many examples are to taken while calculating the margin. It can be tuned to get better results. 
        
        C is the regularization parameter.

2)Gaussian Kernel:
      
        k(x, y) = exp( -[ ( || x - y ||^2) / ( 2 * (variance)^2 ) ] )
        
        Gaussian kernel works well with Normal Distributed data.
        
3)Polynomial Kernel:

        k(x1, x2) = ( x1*x2 + 1)^d
        
        where d is the degree of polynomial.
        
        Polynomial Kernel holds good for image classification.
        
4)Sigmoid Kernel:

        k(x, y) = tanh( alpha * x.T * y + c)
        
        Sigmoid Kernel holds good in Neural Networks.
