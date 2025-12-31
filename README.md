# Simulation-Inverse-Transform
Inverse transformation is a method of simulation that allows sampling from an invertible function to generate data from said function. This has various applications such as taking said data to compute expceted  values, variance, satdnard devaition etc.
We will use both Monte Carlo and Inverse transform to approximate the area of a circle of radius r with area Y. 

This project will cover:

- Compare Monte Carlo to Inverse transform methods
- Approximate the expecetd value of Area of a circle
- Plotting histogram of Inverse method vs Line graph of theoretical value
 
## HOW IT'S MADE 
Languages used: R (version 4.5.1)    
Environment: RStudio  

[![Language: R](https://img.shields.io/badge/Language-R-276DC3.svg?style=flat-square)](https://www.r-project.org/)
[![Built with RStudio](https://img.shields.io/badge/IDE-RStudio-75AADB?style=for‐the‐badge&logo=rstudio&logoColor=white)](https://www.rstudio.com/)
![Status](https://img.shields.io/badge/Status-Completed-lightgrey)

## METHODS AND TECHNIQUES  
**Monte Carlo Method**
We begin by defining a funcion that we will call to

<img width="1183" height="825" alt="Image" src="https://github.com/user-attachments/assets/56b7f5bc-90ec-4551-be9e-b8ba0fb1031c" />

## FUNCTION EXPLANATION  
In ann effort to identify how the casino will perfrom we will simulate the probability of the casino generating a specfic interval of money for each month. In this case, we want to know what the probability of the casino earning between $4600 and $6000.

`sim4ot6` - a function that simulates the probability of the casino generating between $4600 and $6000 

This function: 
has a list `list4to6` - stores an list of 100,000 values generated from the proabilities given above to earn -$1 and $1  
If the sum for each list generated is between $4600 and $6000 store the number 1 and 0 if not.

We then replicate this simulation 5000 times and get the mean of the outcome stored in `mean4to6` using `mean()` and `replicate()`

 ## PROJECT STRUCTURE      
|[Simulation- Random Walks](https://github.com/leta199/Simulation-Random-Walks)  
|├── [Randomwalk R script](https://github.com/leta199/Simulation-Random-Walks/blob/main/Randomwalk.r)   
|└──[Random latex](https://github.com/leta199/Simulation-Random-Walks/blob/main/Random_Walk_Gamblers_Ruin.pdf)
  

## AUTHORS   
[leta199](https://github.com/leta199)  
