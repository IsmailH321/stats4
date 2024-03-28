Practical 4

Continuous random variable-
a. Probability distribution of continuous random variable
b. Probability density function

Syntax:
runif(n, min = 0, max = 1)
Parameter:

n= number of random samples
min=minimum value(by default 0)
max=maximum value(by default 1)
print("Random 15 numbers between 1 and 3") 
runif(15, min=1, max=3)
[1] “Random 15 numbers between 1 and 3” 
[1] 1.534 1.772 1.027 1.765 2.739 1.681 1.964 2.199 1.987 1.372 2.655 2.337 2.588 1.216 2.447

Quantile for a probability

Syntax:
qunif(p,  min = 0, max = 1)
Parameter : 

p – The vector of probabilities
min , max – The limits for calculation of quantile function
min <- 0 
max <- 40 
print ("Quantile Function Value") 
  
# calculating the quantile function value 
qunif(0.2, min = min, max = max)
[1] “Quantile Function Value” 
[1] 8
min <- 0 
max <- 1 
# Specify x-values for qunif function 
xpos <- seq(min, max , by = 0.02)                       
# supplying corresponding y coordinations 
ypos <- qunif(xpos, min = 10, max = 100)        
# plotting the graph  
plot(ypos)

Probability Density Function

Syntax:
dunif(x,  min = 0,  max = 1,  log = FALSE)
Parameter:

x: input sequence
min, max= range of values
log: indicator, of whether to display the output values as probabilities.
# generating a sequence of values 
x <- 5:10 
print ("dunif value") 
# calculating density function 
dunif(x, min = 1, max = 20)
[1] “dunif value” 
[1] 0.05263158 0.05263158 0.05263158 0.05263158 0.05263158 0.05263158
min <- 0 
max <- 100 
# Specify x-values for qunif function 
xpos <- seq(min, max , by = 0.5)                       
# supplying corresponding y coordinations 
ypos <- dunif(xpos, min = 10, max = 80)        
# plotting the graph  
plot(ypos , type="o"

Cumulative probability distribution

punif(q,   min = 0,   max = 1, lower.tail = TRUE)
min <- 0  
max <- 60 
# calculating punif value 
punif (15 , min =min , max = max)
[1] 0.25
min <- 0  
max <- 60 
# calculating punif value 
punif (15 , min =min , max = max, lower.tail=FALSE)
[1] 0.75
