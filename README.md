# Variable Selection in Regression: A Comparison of Direct and Indirect Methods

## Project Overview
This project focuses on addressing the variable selection problem in regression using both direct (Mixed Integer Quadratic Programming - MIQP) and indirect (LASSO) methods. The goal is to compare the computational efficiency and predictive performance of these techniques. The project involves cross-validation to determine the optimal hyperparameters, solving optimization problems, and evaluating models on test datasets.

## Deliverables
1. **Python Code File:** Python code file containing well-documented code, cross-validation, and model evaluation, utilizing packages like Pandas, Numpy for database, sklearn for Lasso Linear Regression with k-fold cross-validation using LassoCV, and Matplotlib, Seaborn for data visualization.
2. **PDF Report:** A comprehensive PDF report detailing the problem, solution approach, results, and analysis. The report includes relevant visualizations and a comparison of direct and indirect variable selection methods.

## Problem Overview
The project addresses the variable selection problem in regression, where direct variable selection is formulated as an MIQP, and indirect variable selection is implemented using LASSO. The focus is on comparing these methods in terms of computational efficiency and predictive accuracy.

## Specifics
1. Utilize two datasets provided on Canvas, one for training and one for testing. Follow the data science pipeline, including 10-fold cross-validation on the training set to determine the optimal values of k or 𝜆.
2. Implement MIQP for direct variable selection, incorporating binary variables and the big-M method. Perform 10-fold cross-validation for various values of k, limiting the time for solving each MIQP problem.
3. Choose the optimal value of k based on the smallest cross-validation error and fit the MIQP model on the entire training set. Use the obtained 𝛽s to predict y values on the test set.
4. Utilize scikit learn to perform 10-fold cross-validation on the training set to determine the optimal 𝜆 for LASSO. Fit a LASSO model on the entire training set using the selected 𝜆 and predict y values on the test set.
5. Present the results as if delivering a report to a boss considering a shift from LASSO to direct variable selection. Include advantages, disadvantages, and visualizations to support the comparison. Assume interest in the provided data for the report.

## Notes for Code Execution
- Implemented efficient cross-validation code for MIQP, considering the large number of variables (50).
- Set a reasonable time limit for solving each MIQP problem during cross-validation.
- Ensured that the code is structured to save results to avoid lengthy runtimes during subsequent runs.
- Included a time limit variable at the beginning of the Python code for ease of adjustment
- Used visualizations to convey important points and aid in the comparison of both techniques.
- Provided insights into the computational efficiency and performance trade-offs between direct and indirect variable selection methods.
