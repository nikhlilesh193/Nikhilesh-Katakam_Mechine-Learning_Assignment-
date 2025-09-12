CS5710- Homework 1
---------------------------------------------------------------------------------------------------
Student Name: Nikhilesh Katakam

Student ID: 700772365

Course: CS5710- Machine Learning 

---------------------------------------------------------------------------------------------------
📍Overview
---------------------------------------------------------------------------------------------------
This assignment explores the foundations of linear regression, gradient descent, and key machine learning concepts such as underfitting, overfitting, and model evaluation.

It consists of both theoretical exercises (manual calculations and conceptual reasoning) and a programming task (implementing linear regression using both closed-form and gradient descent solutions).

--------------------------------------------------------------------------------------------------
☑️ Assignment Breakdown
-------------------------------------------------------------------------------------------------

Q1. Function Approximation by Hand

. Compared two candidate linear models on a small dataset.

. Computed Mean Squared Error (MSE) for each model.

.  Concluded that Model B ((\theta = (0.5, 1))) is the better fit with MSE = 0.75.

-------------------------------------------------------------------------------------------------

Q2. Random Guessing Practice

. Evaluated a quadratic cost function (J(a,b)) at two random guesses.

. Found ((0.5, 0.9)) is closer to the true minimum.

. Explained why random guessing is inefficient compared to gradient descent.

-------------------------------------------------------------------------------------------------

Q3. First Gradient Descent Iteration

. Dataset: ((1,3), (2,4), (3,6), (4,5)).

. Started from (\theta = (0,0)), (\alpha = 0.01).

. After two iterations, parameters improved and cost decreased from 10.75 → 7.75.

-------------------------------------------------------------------------------------------------

Q4. Random Guessing vs Gradient Descent

. Compared two random guesses vs one gradient descent step.

. Found that random guess ((0.2,0.5)) yielded a lower cost than one GD step.

. Highlighted that GD systematically reduces error and eventually outperforms random guessing.

-------------------------------------------------------------------------------------------------

Q5. Recognizing Underfitting

. Case: High training error + High test error → Underfitting.

. Causes: Model too simple, not enough features, insufficient training.

. Fixes: Increase capacity, add features, reduce regularization, train longer.

-------------------------------------------------------------------------------------------------

Q6. Comparing Models

. Model A: Good training error but poor test error → Overfitting.

. Fixes: Regularization, simplify model, early stopping, more data.

. Model B: Poor training and test error → Underfitting.
    Fixes: Increase complexity, add features, train longer.

-------------------------------------------------------------------------------------------------

Q7. Programming: Linear Regression (Closed-form vs Gradient Descent)
Implemented linear regression in Python:

1. Data Generation:

   . Synthetic dataset:
   
     [ y = 3 + 4x + \epsilon, \quad \epsilon \sim \mathcal{N}(0,1) ]
   
   . 200 samples, (x \in [0,5]).
   
2. Closed-form Solution (Normal Equation):

   [ \theta = (X^T X)^{-1} X^T y ]

3. Gradient Descent (GD):

    . Learning rate (\eta = 0.05), 1000 iterations.

    . Loss = Mean Squared Error (MSE).

4. Results:
   
    . Closed-form: ((b_0, b_1) \approx (2.69, 4.13))

    . Gradient Descent: ((b_0, b_1) \approx (2.69, 4.13))

    . ✅ GD converged very close to closed-form.

5. Visualizations:

    . Scatter plot with regression lines (Closed-form vs GD).
  
    . GD loss curve (MSE vs iterations).

-----------------------------------------------------------------------------------------------

📁Files Included 

. Homework 1_Solution_Nikhilesh_Katakam.py 

------------------------------------------------------------------------------------------------


