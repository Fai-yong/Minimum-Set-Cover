# Minimum-Set-Cover

## Question Requirement

The project aims to select subsets from a larger dataset, ensuring specific overlap criteria among the selected groups. 

Given a set of `m` samples `(45 ≤ m ≤ 54)`, a subset of `n` samples is chosen `(7 ≤ n ≤ 25)`. 

From these `n` samples, all the combinations with `j` elements are formed. 

The goal is to find the least amount of `k-sized` combinations `(4 ≤ k ≤ 7)`, ensuring that for each `j-sized` combinations `(s ≤ j ≤ k) from  `n` numbers ` where  `(3 ≤ s ≤ 7)`, there is at least one `k-sized` group that shares `s` common elements with it.

### Example

With `m=45, n=16, k=6, j=5, and s=4`, if the `n` samples are selected, which is just 16 numbers. 

We want to find the least number of combinations with `k=6` elements that for each combination with `j=5` elements from the `n` numbers, there is at least one `k-sized` group that shares `s=4` common elements with it.

Here is the Relationship of n-k-j-s: 

![Relation of nkjs](https://github.com/Fai-yong/Minimum-Set-Cover/blob/main/image/n-k-%20%20relationship.svg)
## Abstract
  The project's core is a program developed using C++ (compiled into an exe executable file), which realizes more efficient matching results. 
  
  The program includes the generation of randomized or customized sample sizes and the computation of optimal results. 

  Experimental findings demonstrate that the proposed method can rapidly achieve solution approximations with favorable accuracy, effectively exhibiting high-performance outcomes.

## I. Introduction
  This project focuses on the growing need for efficient and accurate sample selection methods in critical areas such as healthcare, finance, and social networking.  

  The project introduces an approach using a grouped-based Hill climbing algorithm to solve a given combinatorial optimization problem with specific parameters.  

  It is based on a grouped-based Hill climbing algorithm and a search algorithm, aiming to find optimal solutions in the problem's search space. By using this approach, we aim to find a relatively optimal solution to the problem within an acceptable computation time.

## II. Methods
### 2.1 Grouped Hill Climbing Algorithm



This approach employs a modified Hill Climbing algorithm, tailored specifically for group-based optimization.  This algorithm starts with a randomly selected solution and iteratively improves it by exploring neighboring solutions. 

By focusing on group dynamics within the sample selection, we enhance the traditional Hill Climbing method, enabling it to efficiently navigate complex optimization landscapes.  

This results in more effective solution identification, balancing both speed and accuracy in the context of large datasets.

### 2.2 Algorithm Implementation
- `generate_random_numbers`: Generates a set of random numbers within a specified range.
- `Generate_Comb`: Calculates all possible combinations of a given size from a set of numbers.
- `get_intersection_size`: Determines the size of the intersection of two groups.
- `calc_intersection`: Computes the intersections of different groups.
- `Hill_Climb`: The main hill-climbing algorithm, iteratively searching for the optimal solution by evaluating neighboring solutions and selecting the one with the best performance.

Here is the diagram explanation:

![algorithm](https://github.com/Fai-yong/Minimum-Set-Cover/blob/main/image/algorithm.svg)

## III. Features Developed/Used
Highlights manual input of parameters, user-specified integer sets, progress bar, automatic saving of results, and UI features for improved usability.

![algorithm](https://github.com/Fai-yong/Minimum-Set-Cover/blob/main/image/a2y8x-uqeew.svg)

![ui01](https://github.com/Fai-yong/Minimum-Set-Cover/blob/main/image/ui01.png)

![ui02](https://github.com/Fai-yong/Minimum-Set-Cover/blob/main/image/ui02.png)


## IV. Contributions
This project has made noteworthy contributions towards achieving efficient runtime performance and obtaining optimal or nearly optimal solutions in this project. 

The following are the key highlights of our contributions:

**Improved solving speed**: We extensively optimized the algorithm to discover solutions for various problem instances within a relatively shorter span of time. Our program can compute answers for n values between 7 and 25 within an acceptable timeframe.

Optimal or nearly optimal results: After running a gamut of tests on different parameter combinations, we found that the algorithm produced optimal or nearly optimal solutions. The "Test Sample Parameters" file shows that our program did an exemplary job of balancing runtime and optimal outcomes. Our algorithm's error rate, compared to optimal solutions, ranged from 5% to 30%, and time within 10 seconds.

![bar chart](https://github.com/Fai-yong/Minimum-Set-Cover/blob/main/image/bar%20chart.svg)


![image](https://github.com/Fai-yong/Minimum-Set-Cover/blob/main/image/line%20chart.svg)


