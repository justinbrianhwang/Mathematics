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
- If $t^* \sim t_k$, then $E(t^*) = 0$ for $k > 1$, and $Var(t^{*}) = \frac{k}{k - 2}$ for $k > 2$.
- The $t$ distribution is symmetric around the mean $0$ similar to the standard normal distribution.
- As the degrees of freedom $k$ increase, the shape of the $t$ distribution approaches that of the standard normal distribution.
- For small samples, it is used for inference about the population mean, difference between population means, and in regression analysis.
- **Important**: Distribution of the studentized sample mean:
    
    If $X_1, ~X_2, ~\cdots, ~X_n$ are random samples drawn from a normal population $N(\mu, ~\sigma^2)$, then $t^* = \frac{\bar{X} - \mu}{s / \sqrt{n}}$ follows a $t$ distribution with $n-1$ degrees of freedom, i.e., $t_{n-1}$.
    
- $t_{\alpha;k}$: Denotes the value on the x-axis where the right tail area of a $t$ distribution with $k$ degrees of freedom is $\alpha$.
  
  ![t Distribute](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcS36rBlK6utKjHc6vx3JqQqwWvjDT6Rpw3bKw&s)
  
(3) $F$ Distribution: This will not be covered yet.






## In korean

### $\chi^2$ 분포, $t$ 분포, $F$ 분포

이러한 분포는 정규 모집단에서 추출한 확률 표본($X_1,~X_2, \cdots,~X_n$)을 변형하여 도출된 분포입니다. 통계적 추론(추정과 검정)에 널리 사용됩니다.

(1) $\chi^2$ 분포

- **정리**: $\chi^2$ 분포
    
    $Z_1, ~Z_2, ~\cdots, ~Z_k$가 $k$개의 상호 독립인 표준정규분포 확률변수일 때, $Y = {Z_1}^2 + {Z_2}^2 + \cdots + {Z_k}^2$의 분포를 자유도가 $k$인 $\chi^2$ 분포라 하고, ${\chi_k}^2$로 나타냅니다.
    
- $Y \sim {\chi_k}^2$이면,
    
    확률밀도함수: $f_Y (y;k) = \frac{1}{\Gamma(\frac{k}{2})2^{\frac{k}{2}}}y^{\frac{k}{2} - 1} e^{- \frac{y}{2}}$, $0 < y < \infty$, $E(Y) = k$, $Var(Y) = 2k$
    
- $\chi^2$ 분포의 형태와 특성은 자유도의 크기에 의해 결정됩니다.
- 모분산에 대한 추론, 분할표에서의 독립성 검정, $t$ 분포와 $F$ 분포의 정의 등에 사용됩니다.
- **중요**: $X_1, ~X_2, ~\cdots, ~X_n$이 정규 모집단에서 추출된 확률 표본이라면

$$
\frac{(n-1)s^2}{\sigma^2} = \frac{\sum_{i=1}^{n} (X_i - \bar{X})^2}{\sigma^2}
$$

은 자유도가 $n-1$인 $\chi^2$ 분포, 즉 ${\chi_{n-1}}^2$ 분포를 따릅니다.
    
- ${\chi_{\alpha;k}}^2$: 자유도가 $k$인 $\chi^2$ 분포에서 오른쪽 꼬리의 면적이 $\alpha$인 $x$축 값을 나타내는 기호입니다. 즉, $P({\chi_{k}}^2 > {\chi_{\alpha;k}}^2) = \alpha$입니다.

  ![chi distribution](https://upload.wikimedia.org/wikipedia/commons/thumb/2/21/Chi-square_distributionPDF.png/270px-Chi-square_distributionPDF.png)
    
(2) $t$ 분포: 특히 작은 표본(표본수 $< 30$)에 유용하게 사용됩니다.

- **정의**: $t$ 분포
    
    $Z$와 $V$가 상호 독립이고, $Z$는 표준정규분포를 따르며, $V$는 자유도가 $k$인 $\chi^2$ 분포를 따른다고 하자. 이때, $t^* = \frac{Z}{\sqrt{V/k}}$로 정의되는 확률 변수는 자유도가 $k$인 $t$ 분포를 따른다고 정의하고 $t_k$로 나타냅니다.
    
- $t$ 분포의 형태와 특성은 자유도 $k$에 의해 결정됩니다.
- $t^* \sim t_k$이면, $E(t^*) = 0$ (for $k > 1$), $Var(t^*) = \frac{k}{k - 2}$ (for $k > 2$)
- $t$ 분포는 평균이 $0$을 중심으로 대칭 분포합니다.
- 자유도 $k$가 커질수록 $t$ 분포의 형태는 표준정규분포에 가까워집니다.
- 작은 표본인 경우, 모평균에 대한 추론, 모평균 차에 대한 추론 및 회귀분석 등에 사용됩니다.
- **중요**: 스튜던트화된 표본평균의 분포:
    
    $X_1, ~X_2, ~\cdots, ~X_n$이 정규 모집단 $N(\mu, ~\sigma^2)$에서 추출된 확률 표본이라면, $t^* = \frac{\bar{X} - \mu}{s / \sqrt{n}}$는 자유도가 $n-1$인 $t$ 분포, 즉 $t_{n-1}$ 분포를 따릅니다.
    
- $t_{\alpha;k}$: 자유도가 $k$인 $t$ 분포에서 오른쪽 꼬리의 면적이 $\alpha$인 $x$축 값을 나타내는 기호입니다.
  
  ![t distribution](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcS36rBlK6utKjHc6vx3JqQqwWvjDT6Rpw3bKw&s)
  
(3) $F$ 분포: 이는 아직 다루지 않습니다.


