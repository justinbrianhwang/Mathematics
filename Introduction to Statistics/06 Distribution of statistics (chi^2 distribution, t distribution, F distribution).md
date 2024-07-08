## In English
### $\chi^2$ Distribution, $t$ Distribution, $F$ Distribution

These distributions are derived from transforming a random sample ($X_1,~X_2, \cdots,~X_n$) drawn from a normal population. They are widely used in statistical inference (estimation and testing).

(1) $\chi^2$ Distribution

- **Theorem**: $\chi^2$ Distribution
    
    If $Z_1, ~Z_2, ~\cdots, ~Z_k$ are $k$ independent standard normal random variables, then the distribution of $Y = {Z_1}^2 + {Z_2}^2 + \cdots + {Z_k}^2$ is called a $\chi^2$ distribution with $k$ degrees of freedom and is denoted as ${\chi_k}^2$.
    
- If $Y \sim {\chi_k}^2$, then
    
    Probability density function: $f_Y (y;k) = \frac{1}{\Gamma(\frac{k}{2})2^{\frac{k}{2}}}y^{\frac{k}{2} - 1} e^{- \frac{y}{2}}$, $0 < y < \infty$, $E(Y) = k$, $Var(Y) = 2k$
    
- The shape and characteristics of the $\chi^2$ distribution are determined by the degrees of freedom.
- Used for inference about population variance, independence tests in contingency tables, and the definitions of $t$ and $F$ distributions.
- **Important**: If $X_1, ~X_2, ~\cdots, ~X_n$ are random samples drawn from a normal population with mean $\mu$ and variance $\sigma^2$, then
    
    $$
        \frac{(n-1)s^2}{\sigma^2} = \frac{\sum_{i=1}^{n} (X_i - \bar{X})^2}{\sigma^2}
    $$
    
    follows a $\chi^2$ distribution with $n-1$ degrees of freedom, i.e., ${\chi_{n-1}}^2$.
    
- ${\chi_{\alpha;k}}^2$: Denotes the value on the x-axis where the right tail area of a $\chi^2$ distribution with $k$ degrees of freedom is $\alpha$. That is, $P({\chi_{k}}^2 > {\chi_{\alpha;k}}^2) = \alpha$.

  ![chi distribution](https://upload.wikimedia.org/wikipedia/commons/thumb/2/21/Chi-square_distributionPDF.png/270px-Chi-square_distributionPDF.png)
    
(2) $t$ Distribution: Especially useful for small samples (sample size $< 30$)

- **Definition**: $t$ Distribution
    
    Let $Z$ and $V$ be independent random variables, where $Z$ follows a standard normal distribution and $V$ follows a $\chi^2$ distribution with $k$ degrees of freedom. The random variable $t^* = \frac{Z}{\sqrt{V/k}}$ follows a $t$ distribution with $k$ degrees of freedom and is denoted as $t_k$.
    
- The shape and characteristics of the $t$ distribution are determined by the degrees of freedom $k$.
- If $t^* \sim t_k$, then $E(t^*) = 0$ for $k > 1$, and $Var(t^*) = \frac{k}{k - 2}$ for $k > 2$.
- The $t$ distribution is symmetric around the mean $0$ similar to the standard normal distribution.
- As the degrees of freedom $k$ increase, the shape of the $t$ distribution approaches that of the standard normal distribution.
- For small samples, it is used for inference about the population mean, difference between population means, and in regression analysis.
- **Important**: Distribution of the studentized sample mean:
    
    If $X_1, ~X_2, ~\cdots, ~X_n$ are random samples drawn from a normal population $N(\mu, ~\sigma^2)$, then $t^* = \frac{\bar{X} - \mu}{s / \sqrt{n}}$ follows a $t$ distribution with $n-1$ degrees of freedom, i.e., $t_{n-1}$.
    
- $t_{\alpha;k}$: Denotes the value on the x-axis where the right tail area of a $t$ distribution with $k$ degrees of freedom is $\alpha$.
  
  ![t Distribute](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcS36rBlK6utKjHc6vx3JqQqwWvjDT6Rpw3bKw&s)
  
(3) $F$ Distribution: This will not be covered yet.
