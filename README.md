# Simulation-Inverse-Transform
Inverse transformation is a method of simulation that allows sampling from an invertible function to generate data from said function. This has various applications such as taking said data to compute expceted  values, variance, satdnard devaition etc.  

We will use both Monte Carlo and Inverse transform to approximate the area of a circle of radius "r" with area "Y".   
Radius "r" is distributed on a uniform distribution of [1,4]  
We will try to find the expected value of "Y" (our area). 

This project will cover:

- Comparing Monte Carlo to Inverse transform methods
- Approximate the expected value of Area of a circle
- Plotting histogram of Inverse method vs Line graph of theoretical value
 
## HOW IT'S MADE 
Languages used: R (version 4.5.1)    
Environment: RStudio  

[![Language: R](https://img.shields.io/badge/Language-R-276DC3.svg?style=flat-square)](https://www.r-project.org/)
[![Built with RStudio](https://img.shields.io/badge/IDE-RStudio-75AADB?style=for‐the‐badge&logo=rstudio&logoColor=white)](https://www.rstudio.com/)
![Status](https://img.shields.io/badge/Status-Completed-lightgrey)

## METHODS AND TECHNIQUES  
**Monte Carlo Method**
`sim_circle()` - We begin by defining a funcion that we will call to approximate the area of our circle with this method.     
- Define our set seed to allow for reproducibility
- Set up 10,000 runs of the simulation
- Randomly generate value of "r" from a uniform distribution from 1 to 4 and save to a list
- Find the mean of the area from the generated

  **Inverse CDF Method**
  `sim_circle_2()` - For this method was also also set our seed, number of trials
  - Create a list of values "u" from a unifrom [0,1] distribution
  - Calculate radii "r" using samples from the uniform distribution
  - Store list of ares calculated from the radii "r" in the object "areas"
  
 ## VISUALISING SIMULATION 
We can compare the histogram and line graph of our generated areas and compare them to the actual probability denisty function of areas.

 

 ## PROJECT STRUCTURE      
|[Simulation- Random Walks](https://github.com/leta199/Simulation-Random-Walks)  
|├── [Randomwalk R script](https://github.com/leta199/Simulation-Random-Walks/blob/main/Randomwalk.r)   
|└──[Random latex](https://github.com/leta199/Simulation-Random-Walks/blob/main/Random_Walk_Gamblers_Ruin.pdf)
  

## AUTHORS   
[leta199](https://github.com/leta199)  
