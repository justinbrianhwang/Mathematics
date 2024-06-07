[In english]
# Second-Order Ordinary Differential Equations

Consider the second-order ODE:

$$
y'' + p(x) y' + q(x)y = r(x) 
$$

If \( r(x) = 0 \), it is called homogeneous. If the solutions for \( y(x) \) are \( y_1 \) and \( y_2 \), then \( c_1 y_1 + c_2 y_2 \) is also a solution for \( y \). If \( k_1 y_1 + k_2 y_2 = 0 \) and \( k_1 = 0 \) and \( k_2 = 0 \), the solutions are **linearly independent**. If \( k_1 \neq 0 \) and \( k_2 \neq 0 \), they are **linearly dependent**, meaning \( y_1 \) and \( y_2 \) are multiples of each other, \( y_2 = k y_1 \).

→ To check for linear dependence:

## Wronskian Method

$$
W(y_1, y_2) = 
\begin{vmatrix}
y_1 & y_2 \\
y_1' & y_2'
\end{vmatrix}
= y_1 y_2' - y_1' y_2
$$

If \( W = 0 \) for all \( x \), the solutions are **linearly dependent**.

### Solving Homogeneous Equations

$$
y'' + p(x) y' + q(x)y = 0
$$

#### Reduction of Order

If \( y_1 \) is known, let \( y_2 = u y_1 \). Substitute this into the equation and differentiate, then simplify to get:

$$
u' = \frac{1}{y_1^2} e^{-h}, \quad h = \int p(x) dx
$$

#### Constant Coefficient Equations

For equations of the form:

$$
y'' + ay' + by = 0
$$

Assume the general solution \( y = e^{\lambda x} \). Substituting this into the equation, we get the characteristic equation:

$$
e^{\lambda x} (\lambda^2 + a\lambda + b) = 0
$$

The characteristic equation \( \lambda^2 + a\lambda + b = 0 \) can be solved using the discriminant.

- **Case 1**: Discriminant is positive (two distinct real roots)

    $$
    y(x) = c_1 e^{\lambda_1 x} + c_2 e^{\lambda_2 x}
    $$

- **Case 2**: Discriminant is zero (repeated roots)

    $$
    y(x) = (c_1 + c_2 x)e^{-\frac{a}{2}x}
    $$

- **Case 3**: Discriminant is negative (complex roots)

    $$
    y(x) = e^{-\frac{a}{2}x} (A \cos \omega x + B \sin \omega x)
    $$

    where \( \lambda = -\frac{a}{2} \pm i \omega \) and \( \omega^2 = b - \frac{1}{4}a^2 \).

### Euler-Cauchy Equation

For equations of the form:

$$
x^2 y'' + axy' + by = 0
$$

Assume the general solution \( y = x^m \). Substituting this into the equation, we get the characteristic equation:

$$
x^m (m^2 +(a-1)m + b) = 0
$$

The characteristic equation \( m^2 +(a-1)m + b = 0 \) can be solved using the discriminant.

- **Case 1**: Discriminant is positive (two distinct real roots)

    $$
    y(x) = c_1 x^{m_1} + c_2 x^{m_2}
    $$

- **Case 2**: Discriminant is zero (repeated roots)

    $$
    y(x) = (c_1 + c_2 \ln x)x^m , \quad (m = \frac{1}{2}(1-a))
    $$

- **Case 3**: Discriminant is negative (complex roots)

    This case is not commonly encountered and is therefore omitted.

## Solving Nonhomogeneous Equations

$$
y'' + p(x) y' + q(x)y = r(x), \quad (r(x) \neq 0)
$$

The general solution is \( y(x) = y_h (x) + y_p(x) \), where \( y_h \) is the solution to the homogeneous equation. \( y_p \) depends on the form of \( r(x) \). Refer to the following table for different forms of \( r(x) \):

| \( r(x) \)                               | \( y_p(x) \)                                             |
| --------------------------------------- | ------------------------------------------------------- |
| \( K e^{\gamma x} \)                     | \( C e^{\gamma x} \)                                     |
| \( K x^n \)                              | \( K_n x^n + k_{n-1} x^{n-1} + \cdots + k_0 \)           |
| \( K \cos \omega x \) or \( K \sin \omega x \) | \( K \cos \omega x + M \sin \omega x \)                |
| \( K e^{\alpha x} \cos \omega x \) or \( K e^{\alpha x} \sin \omega x \) | \( e^{\alpha x}( K \cos \omega x + M \sin \omega x) \) |

### Coefficient Comparison Method

#### Basic Rule

If \( r(x) \) is a monomial, \( y_p(x) \) directly follows the table.

#### Modification Rule

If \( y_h(x) \) is similar to \( r(x) \), modify \( y_p \) by multiplying by \( x \) or \( x^2 \) as needed.

#### Sum Rule

If \( r(x) \) consists of multiple terms, \( y_p \) is the sum of corresponding solutions.

### Lagrange Method

Using the Wronskian, we can solve more complex \( r(x) \) forms.

Let \( W = f_1 {f_2}' - {f_1}' f_2 \). Then, \( y_p \) can be found as follows:

$$
y_p = -y_1 \int \frac{y_2}{W} r dx + y_2 \int \frac{y_1}{W} r dx
$$

This formula helps solve nonhomogeneous differential equations.

---

By following these steps and methods, you can solve both homogeneous and nonhomogeneous second-order ODEs efficiently.


[In korean]
**이계 상미분 방정식**

$$
y'' + p(x) y' + q(x) = r(x) 
$$

   $r(x) = 0$이면 Homogeneous하다고 한다. $y(x)$가 각각 $y1,~y_2$로 나온다면 $c_1 y_1 + c_2 y_2$ 도 $y$의 해이다. 이때, $k _1 y_1 + k_2 y_2 = 0$에서, $k_1 = 0 , ~k_2 = 0$이면 **일차 독립**이고, $k_1 \not= 0,~k_2 \not=0$이면 **일차 종속**이다! 일차 종속일 때, $y_1$과 $y_2$의 관계는 실수 배이다! $y_2 = ky_1$이다!

→ 일차 종속의 여부를 확인하는 방법

**Wronskian 방법**

$$
W(y_1 ,~y_2 ) = 
\begin{vmatrix}
y_1 & y_2 \\
y_1' & y_2'
\end{vmatrix}
= y_1 y_2 '- y_1'y_2
$$

  위의 공식의 형태이며, $W = 0$일 때, 모든 $x$에 대해 **일차 종속**이다! 

- Homogeneous할 때 풀이법
    
    $$
    y'' + p(x) y' + q(x) y = 0
    $$
    
    - Reduction of solution
        
          $y_1$을 알면, $y_2 = uy_1$ 이라 두고, 위의 식을 이계 미분과 미분하여 해당 식에 넣어서 정리한다. 그렇게 되면, 다음과 같은 일반식이 나오게 된다. 
        
        $$
        u' = {{1}\over{{y_1}^2}} e^{-h},~~h=\int p(x) dx
        $$
        
    - 상수 계수로 이루어진 이계상미분방정식인 경우
        
        $$
        y'' + ay' + by = 0
        $$
        
           이 때, $y$의 기본꼴은 $y = e^{\lambda x}$이다. 기본꼴에서 미분과 이계미분해서 위의 식에 넣으면 다음과 같이 정리할 수 있다. 
        
        $$
        e^{\lambda x} (\lambda^2 + a\lambda + b) = 0
        $$
        
        이때 위에서 $\lambda^ 2 + a\lambda + b$를 특성방정식이라 한다. 위의 식에서 $e^{\lambda x}$가 $0$이 될 수 없다. 그러니 특성방정식이 $0$이 될 수밖에 없다. 특성방정식은 판별식을 통해 케이스를 나눠서 생각할 수 있다. 
        
        - 첫 번째 케이스 - 판별식이 양수일 때 (서로 다른 두 실근)
            
            $$
            y(x) = c_1 x^{\lambda_1} + c_2 x^{\lambda_2 }
            $$
            
            각각 $\lambda_1 ,~ \lambda_2$ 는 특성 방정식의 해이다. 
            
        - 두 번째 케이스 - 판별식이 0일 때 (중근일 때)
            
            $$
            y(x) = (c_1 + c_2 x)e^{-{{a}\over{2}}}
            $$
            
        - 세 번째 케이스 - 판별식이 음수일 때 (서로 다른 두 허근)
            
            $$
            y(x) = e^{-{{a}\over{2}}x} (A \cos \omega x + B \sin \omega x)
            $$
            
            이때, $\lambda = -{{1}\over{2}}a   ~\pm i \omega ~(\omega^2 = b - {{1}\over{4}}a^2 )$ 
            
    - 오일러-코시 방정식
        
        $$
        x^2 y'' + axy' + by = 0
        $$
        
        이 때, 기본 꼴은 $y = x^m$이다. 위에서 상수 계수로 이루어진 이계 상미분방정식과 마찬가지로 정리하면 다음과 같다. 
        
        $$
        x^m (m^2 +(a-1)m + b) = 0
        $$
        
        이다. 약간의 차이는 있으나, $m^2 +(a-1)m + b = 0$을 특성 방정식이라 한다. 상수 계수와 마찬가지로 판별식으로 구분해보자. 
        
        - 첫 번째 케이스 - 판별식이 양수일 때 (서로 다른 두 실근)
            
            $$
            y(x) = c_1 x^{m_1} + c_2 x^{m_2 }
            $$
            
            각각 $\lambda_1 ,~ \lambda_2$ 는 특성 방정식의 해이다. 
            
        - 두 번째 케이스 - 판별식이 0일 때 (중근일 때)
            
            $$
            y(x) = (c_1 + c_2 \ln  x) x^m 
            , ~(m = {{1}\over{2}}(1-a))
            $$
            
        - 세 번째 케이스 - 판별식이 음수일 때 (서로 다른 두 허근)
            
            잘 나오는 형태가 아니니 정리는 생략했다. 
            
        
- Nonhomogeneous할 때 풀이법
    
    $$
    y'' + p(x) y' + q(x) y = r(x) 
    ,~(r(x) \not = 0)
    $$
    
    일반 해 : $y(x) = y_h (x) + y_p(x)$ 
    
    이 때, $y_h$는 homogeneous한 해를 의미하는 함수이다. 즉 $r(x) = 0$을 가정하고 해를 구한 다음 풀이하는 방식이다. $y_p$는 $r(x)$의 형태에 의존하는 방식이다. 이때, $r(x)$ 의 형태를 정리하기 위해 표를 보도록 하자. 
    
    |                                    $r(x)$ |                                   $y_p(x)$ |
    | --- | --- |
    |                                 $K e^{\gamma x}$ 꼴 |                                 $C e^{\gamma x}$  |
    |                                 $K x^n $ 꼴 |           $K_n x^n + k_{n-1} x^{n-1 } + \cdots + k_0$  |
    |                                 $K {\cos \omega x}$ 꼴
                                    $K {\sin \omega x}$ 꼴 |                   $K {\cos \omega x} + M\sin \omega x $ 꼴 |
    |                              $K e^{\alpha x} {\cos \omega x}$ 꼴
                                 $K e^{\alpha x} {\sin \omega x}$ 꼴 |                $e^{\alpha x}( K{\cos \omega x} + M\sin \omega x)$ |
    - 계수 비교법
        
        $r(x)$의 형태가 위의 표를 따르는 방식이다.
        
        - Basic Rule
            
            $r(x)$가 단항으로 있을 때, $y_p(x)$는 다음 표를 바로 따른다. 
            
        - Modification Rule
            
            만약 homogeneous한 함수 $y_h(x)$가 $r(x)$꼴로 나왔다면, $y_p$ 는 $y_h(x)$에 $x$또는 $x^2$ 을 곱한 식으로 표현하면 된다. 검증하고 나서 적절한 식을 찾자.
            
        - Sum Rule
            
            $r(x)$가 여러 개의 항으로 더해진 형태로 이루어졌을 때, 사용하는 방식으로 $y_p$는 표에 맞게 $r(x)$를 각각 대응시켜 더하면 된다. 
            
    - 라그랑주 방법
        
        위에서 언급한 Wronskian을 이용하는 방법이다. 위의 계수 비교법의 가장 큰 단점은 $r(x)$가 한정된다는 것이다. 특정 꼴에서만 사용하는 방식이다. 이를 해결하는 방식이 라그랑주 방법인 것이다. 
        
           $W = f_1 {f_2}' - {f_1}' f_2$ 를 생각하고, $y_p$를 구해보자. 
        
        $$
        y_p = -y_1 {\int {{y_2}\over{W}}}rdx 
        + y_2 {\int {{y_1}\over{W}}}rdx
        $$
        
        이 공식을 이용하면 된다!!
