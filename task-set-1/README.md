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
4. In the future, you will add the solution files in this directory. For now, just add a text file called "details.txt", which wil contain your name and your branch.  
5. Commit these changes, and push to your github repo. 
6. Open GitHub in your web browser. Search for your repository.  Click the "**Pull Request**" tab.
7. Click on the "**New pull request**" button, and then click on the "**Create pull request**" button. 
7. Well done! You have successfully submitted your progress.


### Some useful links for your reference 
1. [An Ultimate Guide to Git and Github](https://www.geeksforgeeks.org/ultimate-guide-git-github/) 
2. [Step Wise Guide to start with Open Source](https://www.geeksforgeeks.org/step-wise-guide-to-start-with-open-source/)
 

### Task 2 

#### Naive Autocompletion  

This task can be done in any language of your choice. **Avoid using in-built functions for tasks such as sorting, finding etc.** 


For this task, you are given two text files - words.txt and words_with_counts.txt

You have to work with words.txt but can choose to work with words_with_counts.txt for an additional challenge, which has been described at the end.  

Your task will be to implement an autocomplete feature. The program will ask the user for a string and then print some strings which have the given string as a prefix.  
Eg - For an input string of "th", the output might be "the", "that", "that", "this". 
This output depends on the dictionary available to you.  
 
You have to finish the following subtasks -  
1. Write a function *read_txt_file(txt_file)*
   - This function will read the given text file and return an array with the words in the text file 
   - **Input**
      - txt_file - String containing the path to the text file 
   - **Output** 
      - word_list - An array containing all the words in the text file  

2. Write a function *sort_words(word_list)* 
   - This function sorts the given wordlist lexicographically 
   - **Do not use any in-built sorting function** 
   - **Inputs**
      - word_list - List of words that you wish to sort 
   - **Outputs**
      - sorted_word_list - List of words sorted according to their lexicographic order 
      
3. For the following function, we will need a helper function, *range_finder(A, E)*. The task of this helper function will be as follows - 
   - Given a sorted array A and an element E, return two indices - I<sub>0</sub> and I<sub>01</sub>. 
   I<sub>0</sub> is the first index such that A<sub>I<sub>0</sub></sub> is equal to E and I<sub>1</sub> is the last index such that A<sub>I<sub>1</sub></sub> is equal to E.   
   Essentially, find all the instances of the element E in the array.  
   - Example 
      - A = \[1,2,3,3,3,4], E = 3. 
      - I<sub>0</sub> = 2, I<sub>1</sub> = 4   
   - Perform this task using binary search. Hint - Binary search can do more than just searching for an element. You will need to do two passes of binary search.  
   - *Can you tell why we're using binary search instead of linear search?*  

4. Write a function *find_matching_word(word_list, string)*
   - This function will find words which start with the given string 
   - **Utilize *range_finder* for this, not linear search**. We didn't do all that sorting for nothing, did we now. You will have to slightly modify it as follows  
      - It will have to work for strings 
      - It will need to treat strings which start with the same characters as the same. Eg. 'th' and 'the' are the same for the purposes of this. 
   - **Inputs**
      - word_list - List of words sorted lexicographically 
      - string - The string which you want to match other string to 
   - **Outputs **
      - matching_strings - An array of strings which start with the given string 

5. Finally, write a command-line based interface which takes in an input and outputs matching strings.   
  
Additional Challenge - For additional challenge, use word_with_counts and sort the words according to two orders - primarily, their lexicographic order. Secondarily, the value of their frequency counts. Your autocomplete program will now sort its outputs according to the frequency of the words.   
 
