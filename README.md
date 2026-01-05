# Inverse Transformation
Inverse transformation is a method of simulation that allows sampling from an invertible function to generate data from said function. This has various applications such as taking said data to compute expceted  values, variance, standard deviation etc.  

We will use both Monte Carlo and Inverse transform to approximate the area of a circle of radius "r" with area "Y".   
Radius "r" is distributed on a uniformly on [1,4].
We will try to find the expected value of "Y" (our area) and compare to the theoretical value via manual calculation.

This project will cover:

- Comparing Monte Carlo to Inverse transform methods.
- Approximate the expected value of Area of a circle based on a distributed "r"
- Plotting histogram of Inverse method vs Line graph of theoretical probability density function.
 
## HOW IT'S MADE 
Languages used: R (version 4.5.1)    
Environment: RStudio  

[![Language: R](https://img.shields.io/badge/Language-R-276DC3.svg?style=flat-square)](https://www.r-project.org/)
[![Built with RStudio](https://img.shields.io/badge/IDE-RStudio-75AADB?style=for‐the‐badge&logo=rstudio&logoColor=white)](https://www.rstudio.com/)
![Status](https://img.shields.io/badge/Status-Completed-lightgrey)

## METHODS AND TECHNIQUES  
**Monte Carlo Method**  
`sim_circle()` - We begin by defining a funcion that we will call to approximate the area of our circle with this method. This function:   
- Defines our set seed to allow for reproducibility.
- Sets up 10,000 runs of the simulation.
- Randomly generate 10,000 values of "r" from a uniform distribution from 1 to 4 and store the value to the vector `r`.
- Find the  area from the generated vector `r` using the fomrula π(r^2) and get the mean of all 10,000 values.
- The expected value of the area of such a circle ≈ 21.84337.

**Inverse CDF Method**   
`sim_circle_2()` - For this method was also also set our seed, number of           trials (10,000). This funtions alos includes: 
- Create a list of values "u" from a unifrom [0,1] distribution and assign to the vector `u`
- Calculate radii "r" using samples from the uniform distribution and assign to the vector `r`
- Find the  area from the generated vector `r` using the fomrula π(r^2) and get the mean of all 10,000 values.
- The expected value of the area of such a circle ≈ 21.84337.
 
 This result proves that the inverse transform and monte carlo methods are identical in result for invertible functions with the same seed and number of simulation runs.
  
 ## VISUALISING SIMULATION 
We can compare the histogram and line graph of our generated areas and compare them to the actual probability density function of areas.

We modify our above inverse cdf funtion in order to output a list of areas. This new function called `sim_circle_plot()` will have values of areas assigned to the vectors  `areas`.

**Histogram** - shows us the density i.e proportion of total that each bucket of areas accounts for with the bucket of area 5-10 beaing the most prevalent.  
- We graph the density of the areas generated with the limits of the x-axis being π(1^2) = π and π(4^2) ≈ 50.264.

**Line graph** - creates a probability density of our areas following the simulated sample data.
- Graphs the theoretical probability denity function of the areas.
 
<img width="1058" height="838" alt="Image" src="https://github.com/user-attachments/assets/9dbe6cb9-3ddf-48e4-a0b1-102d9ea89575" />
 
 ## PROJECT STRUCTURE      
|[Simulation- Inverse Transform](https://github.com/leta199/Simulation-Random-Walks)  
|├── [Inverse Transform Method R script](https://github.com/leta199/Simulation-Inverse-Transform/blob/main/Inverse%20Transform%20Method.r)   
|└──[README](https://github.com/leta199/Simulation-Inverse-Transform/blob/main/README.md)
  
## AUTHORS   
[leta199](https://github.com/leta199)  
