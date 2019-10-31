# Task Set 1 

### Task 1

The structure of this repository is as follows: 
>- **task-set-1**
>  - **submissions** 
>    - **your_git_username** (You have to make this directory) 
>      - *task1.py*
>      - *task2.py*  

The first task will be to get up and running with using this repository. 

1. Fork this repository.
2. Make a clone of the forked repository.
   
   *This will create a local version of this repository on your system. All changes that you will make wil be to this local version. Make sure that you add the upstream remote to this local repository. You will have to routinely update your repository with the upstream*  
   
3. Navigate to **task-set-1**, go to **submissions**, and create your directory (i.e. **your_git_username**).
4. Add the solution files in this directory.
5. Once you have completed all your tasks, push the local version of your repository.
6. Open GitHub in your web browser. Search for your repository.  Click the "**Pull Request**" tab.
7. Click on the "**New pull request**" button, and then click on the "**Create pull request**" button. 
7. Well done! You have successfully submitted your progress.


### Some useful links for your reference 
1. [An Ultimate Guide to Git and Github](https://www.geeksforgeeks.org/ultimate-guide-git-github/) 
2. [Step Wise Guide to start with Open Source](https://www.geeksforgeeks.org/step-wise-guide-to-start-with-open-source/)
 

### Task 2 

Linear Regression from scratch  

Do this task in a Jupyter notebook
Your task is to implement linear regression from scratch on data with a single feature. You will fit a straight line to the given data. 

1. Read the data from data.csv   
2. Plot the X and y as a scatter plot using matplotlib   
3. Write a function **find_cost(X, y, parameters)**, with the following parameters -   
   - This function computes the cost using quadratic cost function   
   - Inputs   
      a. X - The X values   
      b. y - The target/y values   
      c. parameters - The parameter vector   
   - Output    
      a. cost - Cost for the given values   
      
4. Write a function **fit_data(X, y, parameters, learning_rate, iterations)** with the following parameters -  
   - This function finds the closest line using gradient descent for optimization   
   - Inputs    
      a. X - The X values   
      b. y - The target/y values    
      c. parameters - The parameter vector    
      d. learning_rate - Learning rate, with default = 0.1   
      e. iterations - The number of iterations, with default = 10000    
   - Outputs -    
      a. past_costs - The cost after each iteration    
      b. past_parameters - The parameters after each iteration    
      
5. Plot the line which you obtain using the final parameters along with the data    
6. Plot the cost after each iteration    
7. Additional challenge - Animate the line using parameters after each iteration    
