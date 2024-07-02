# In English
1. $y' + 2y = 0$
    
    This is in the form $y' + p(x) y = 0$.
    
    The solution is of the form $y = ce^{-h}$.
    
    Therefore, $y = c e^{-2x}$.

2. $y' = 1 - y^2$ 
    
    This is separable: $\frac{y'}{1-y^2} = 1$
    
    $\frac{dy}{(1 + y)(1 - y)} = dx$
    
    $\frac{1}{2} \left(\frac{1}{1-y} + \frac{1}{1+y}\right) dy = dx$
    
    $\frac{-1}{2} \ln |1-y| + \frac{1}{2} \ln |1+y| = x + c$
    
    $\frac{1-y}{1+y} = ce^{-2x}$
    
    Therefore, $y = \frac{1 + ce^{-2x}}{1 - ce^{-2x}}$.

3. $y' = y - 4y^2$ 
    
    This is separable: $\frac{1}{y(1-4y)} dy = dx$
    
    $\int \left(\frac{1}{y} + \frac{4}{1-4y}\right) dy = \int dx$
    
    $\ln \left|\frac{y}{1-4y}\right| = x + c$
    
    Therefore, $\frac{y}{1-4y} = ce^x$
    
    Hence, $y = \frac{ce^x}{1 + 4ce^x}$.

    4. $xy' = y + x^2$

    $y' = \frac{y}{x} + x^2$

    $y' - \frac{1}{x} y = x$

    This is in the form $y' + py = r$.

    The general solution for this first-order differential equation is:

    $y = e^{-h} \left( \int e^h r \, dx + c \right)$

    Here, $h$ is defined as $h = \int p \, dx$.

    $h = - \ln |x|$

    Therefore, $y = x \left( \int \frac{1}{x} x \, dx + c \right)$

    Hence, $y = x \left( x + c \right)$

    Therefore, $y = x^2 + cx$.


# In korean

1. $y' + 2y = 0$
    
    $y' + p(x) y = 0$ 꼴
    
    $y = ce^{-h}$의 형태로 나온다. 
    
    $y = c e^{-2x}$이다.

2. $y' = 1 - y^2$ 
    
    ${y' \over 1-y^2 } = 1$  (separable)
    
    ${dy\over (1 + y ) (1- y)} = dx$
    
    $\frac{1}{2} \left(\frac{1}{1-y} + \frac{1}{1+y}\right) dy = dx$ 
    
    $-{1\over2} \ln |1-y| + {1\over2} \ln |1+y| = x+c$ 
    
    ${1-y \over 1+ y}= ce^{-2x}$
    
    $y = {1+ce^{-2x} \over 1-ce^{-2x}}$

3. $y' = y - 4y^2$ 
    
    ${1\over y(1-4y)}dy = dx$ 
    
    $\int \left({1\over y} + {4\over 1-4y}\right) dy = \int dx$
    
    $\ln \left|{y\over 1-4y}\right| = x+c$ 
    
    ${y \over 1-4y} = ce^x$
    
    $y = {ce^x \over 1 + 4ce^x}$

4. $xy' = y + x^2$ 
    
    $y' = {y \over x} + x^2$ 
    
    $y' - {1 \over x} y = x$
    
    $y' + py = r$의 형태이다. 
    
    $y = e^{-h} \left{ \int e^h r \, dx + c \right\}$ 가 위의 일차 미분방정식의 기본꼴이다. 
    
    이때, $h$는 $h = \int p \, dx$로 정의된다. 
    
    $h = - \ln |x|$
    
    $y = x \left{ \int {1 \over x} \times x \, dx + c \right\}$
    
    $y= x \left{ x + c \right\}$
    
    ∴ $y= x^2 + cx$

