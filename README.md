# Random-Fibonacci-Series
This series is defined by the following relationship with the initial values ​​of F1 = F2 = 1:

![image](https://github.com/SogolGoodarzi/Random-Fibonacci-Series/assets/125180530/d6ff3fb4-a711-43f9-ad23-3db88d1ba0a0)

The second member of the Fibonacci series asymptotically converges to $\phi^{n}$, which is called the golden ratio. that means:

![image](https://github.com/SogolGoodarzi/Random-Fibonacci-Series/assets/125180530/9560afbf-ce76-4ce9-9d61-0fb12532a510)

<p align="justify"> The random Fibonacci series is defined in the form of the following relationship, where the value of $\beta_{n}$ is a discrete random variable that includes ±1 values ​​with equal probability. </p>

![image](https://github.com/SogolGoodarzi/Random-Fibonacci-Series/assets/125180530/a0005a86-9599-416e-82d6-a2275490a30d)

<p align="justify"> Obviously, $f_{n}$ is a complex random variable and depends on its previous $\alpha_{n}$. As a result, this series does not have an asymptotic value. Although the random Fibonacci series is always smaller than the regular Fibonacci series, it does not have an asymptotic value, because as n converges to infinity, the value of $f_{n}$ fluctuates between positive and negative values. But in 1960, Furstenberg and Kestenm proved that the absolute magnitude of the sequence converges asymptotically to $\alpha_{n}$. </p>

### Part a.
<p align="justify"> To determine the confidence interval for $\alpha$, the following relationship is used for 95% confidence, which is clear that by sampling for the number of different sentences of the Fibonacci series, we should have the values ​​of variance and mathematical expectation or the same average. </p>

![image](https://github.com/SogolGoodarzi/Random-Fibonacci-Series/assets/125180530/8faa40c7-0632-48fd-88c2-d49b77781f81)

![image](https://github.com/SogolGoodarzi/Random-Fibonacci-Series/assets/125180530/731e8155-135c-4bd0-9d6e-118dbeb78d39)

<p align="justify"> Now, as it was said, for different samples, for example 100, 300, and 500 in the Fibonacci series, we find the values ​​of variance and expectation, and we find the confidence interval approximately, which can be said that the more the number of samples, the more accurate the confidence interval will be. The output of the code is as follows. </p>

![image](https://github.com/SogolGoodarzi/Random-Fibonacci-Series/assets/125180530/2c49de4c-bbfc-4535-8735-f8417c0bfc5b)

### Part b.
<p align="justify"> Consider the following series. We show the largest pretended term by ($f_{max}$), which is a random variable with positive support. We want to estimate the distribution of this random variable as an exponential distribution. First, prove the relation of the maximum magnification of the parameter of the exponential distribution ($\lambda$), then by sampling from $f_{max}$(25) fit a distribution on it. </p>

First, we obtain the maximum likelihood relation for the exponential distribution parameter or $\lambda$.

![image](https://github.com/SogolGoodarzi/Random-Fibonacci-Series/assets/125180530/2483c0e0-dfa7-4a3d-9d56-2e8fa608768b)

<p align="justify"> Using the relationship we obtained, first, for one value, we obtain n samples from the Fibonacci series, which include the maximum value among the sentences of the series. Using the relationship we obtained for parameter estimation, the value of Landa can be estimated with the samples taken. Note that the distribution that can be considered for ($f_{max}$) is the exponential distribution with the parameter $\lambda$. </p>

![image](https://github.com/SogolGoodarzi/Random-Fibonacci-Series/assets/125180530/46ba22be-ae86-4abf-9d23-581c7b2c0dc8)

The output of the program for 25-sentence series with 500 repetitions of sampling is as follows:

![image](https://github.com/SogolGoodarzi/Random-Fibonacci-Series/assets/125180530/9c86d612-e1ae-4e5a-9e06-9b658c5ada1d)

This value is estimated and variable, and every time the program is executed, a numerical value in the same range is obtained.

### Part c.
<p align="justify"> A non-parametric method is to estimate the density function based on the distribution histogram. Fit the empirical density function to the data using the examples you took in the previous section. Then plot this density function along with the estimated function in the previous section in a graph. </p>

![image](https://github.com/SogolGoodarzi/Random-Fibonacci-Series/assets/125180530/85b1bb12-e380-4294-b2d7-b1fa9e887afa)

<p align="justify"> As it is known, the distribution of the samples tends to the same exponential distribution with the parameter $\lambda$, and the distribution of the samples can be almost modeled with the exponential distribution. </p>

### Part d.
Check the effect of increasing n on mathematical expectation  $\lambda$ by plotting a graph. 

<p align="justify"> Let's do the same program that was done for part(b) for this part and for different values ​​for n, and finally, we will plot the mathematical expectation of the estimates for  $\lambda$ for each n. </p>

![image](https://github.com/SogolGoodarzi/Random-Fibonacci-Series/assets/125180530/d0a85b44-6445-4d79-aff9-7553d34a17cc)

<p align="justify"> By looking at the graph, we can conclude that as the value increases, the mathematical expectation of the estimates for  $\lambda$ converges to the value estimated in part(b) (the approximate value of the estimate in part(b) was about 0.011). This estimate is more accurate for  $\lambda$ because it is checked for different n and their expectation is taken. So, the higher the n number, the better and more accurate the estimate will be. </p>
