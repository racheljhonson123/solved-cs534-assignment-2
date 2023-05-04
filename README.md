Download Link: https://assignmentchef.com/product/solved-cs534-assignment-2
<br>
In this assignment, we are using 3 variations of perceptron to to classify handwritten digits of numbers 3 or 5.

<strong>Preprocessing </strong>

<ol>

 <li>The output Y from the train and validation datasets are changed to 1 and -1 ( +1 to 3 and -1 to 5) and removed from the dataset for further processing with the train and validation data.</li>

 <li>Add bias feature ( equals to 1 ) to train, validation and test data to improve the fit.</li>

</ol>

<strong>Part 1 : Online Perceptron </strong>

<ul>

 <li>​<strong>Implement the online perceptron model with algorithm described in Algorithm 1. Set the iters = 15. During the training, at the end of each iteration use the current w to make prediction on the validation samples. Record the accuracies for the train and validation at the end of each iteration. Plot the recorded train and validation accuracies versus the iteration number. </strong></li>

 <li><strong>Does the train accuracy reach to 100%? Why? <u>Solution</u></strong></li>

</ul>

<strong>Part 2 : Average Perceptron </strong>

<ul>

 <li><strong>Please implement the average perceptron described in Algorithm 2</strong></li>

 <li><strong>Plot the train and validation accuracies versus the iteration number for iters = 1, …, 15. </strong></li>

 <li><strong>How average model has affected the validation accuracy comparing to the online perceptron? </strong></li>

</ul>




<strong>Part 3 : Polynomial Kernel Perceptron </strong>

<ul>

 <li><strong>Implement the polynomial kernel function k<sub>p</sub></strong>​<strong> in the Algorithm 3. This function takes</strong><sub>​ </sub><strong> two vectors x</strong>​<strong>1</strong><strong> and x</strong><sub>​      </sub>​<strong>2</strong><strong> and an integer p for the polynomial degree, and returns a real value.</strong><sub>​         </sub></li>

 <li><strong>Define a Gram matrix K with size N × N where N is the number of training samples. Fill matrix K(i, j) = k p (x</strong>​<strong>i</strong><strong> , x</strong><sub>​ </sub>​<strong>j</strong><strong> ) for all of the pairs in the training set.</strong><sub>​ </sub></li>

 <li><strong>Implement the rest of the kernel perceptron in Algorithm 3. For each p in [1, 2, 3, 7,15]:</strong></li>

 <li><strong>Run the algorithm to compute α. </strong></li>

 <li><strong>At the end of each iteration use the current α to predict validation set. </strong></li>

</ul>




<ul>

 <li><strong>Record the train and validation accuracy for each iteration and plot the train and validation accuracies versus the iteration number. </strong></li>

</ul>

<strong> </strong>

<strong> </strong>

<strong> </strong>

<ul>

 <li><strong>Record the best validation accuracy achieved for each p over all iterations. </strong></li>

</ul>

<strong> </strong>

<table width="554">

 <tbody>

  <tr>

   <td width="123"><strong>POWER </strong></td>

   <td width="431"><strong>ACCURACY (in %) </strong></td>

  </tr>

  <tr>

   <td width="123"><strong>P = 1 </strong></td>

   <td width="431"><strong>95.0276243094 </strong></td>

  </tr>

  <tr>

   <td width="123"><strong>P = 2 </strong></td>

   <td width="431"><strong>98.3425414365 </strong></td>

  </tr>

  <tr>

   <td width="123"><strong>P = 3 </strong></td>

   <td width="431"><strong>98.4653161449 </strong></td>

  </tr>

  <tr>

   <td width="123"><strong>P = 7 </strong></td>

   <td width="431"><strong>97.7286678944 </strong></td>

  </tr>

  <tr>

   <td width="123"><strong>P = 15 </strong></td>

   <td width="431"><strong>96.5623081645 </strong></td>

  </tr>

 </tbody>

</table>




<ul>

 <li><strong>Plot the recorded best validation accuracies versus degrees. Please explain how p is affecting the train and validation performance.</strong></li>

 <li><strong>Use your best α (the best you found over all d and iterations above) to predict the test data-set. Please name the predicted file as kplabel.csv. </strong></li>

</ul>


