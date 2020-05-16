# Neural-Networks-

Creating a Deep Neural network Model ::

1. Initialize parameters 
2. Loop for number of iterations: <br>
    a. Forward propagation <br>
    b. Compute cost function <br>
    c. Backward propagation <br>
    d. Update parameters (using parameters, and grads from backpropagation ) <br>
3. Finally, Use trained parameters to predict labels

Starting from :
Point 1. -

layer_dims=number of layers  and  Linear Hypothesis  --->   Z=W*X + b
So, initializing W and b for each layer using random to make them differnt in each layer 

Point2. -
(A)

For forward propagation ,first we need activation functions 
So, creating sigmoid and relu functions with Z hypothesis
And implementing RELU activation for each layer and sigmoid for last layer ,also storing outputs of linear hypothesis and activation functions as cache.

(B)

Now, computing cost i.e. how much error is their from actual output 
using , cost = (-1/m)*np.sum(Y*np.log(AL)+(1-Y)*np.log(1-AL))

(C)

For backward propagation ,we will calculate grads(gradients for each layer)
        from last layer(with sigmoid activation ) to  1st layer(in between layers with relu activation)

(D)

Now, We will update parameters (W and b ) .Since, we know the gradients 
and with some learning rate(manually calibrated).

All these steps (A),(B),(C),(D) are iterated in loop (also called epoches) , to get the correct parameters by again and agin updating then and hence decreasing cost .

Final parameters obtained are then used to predict new examples.



