[In English]
# Second-Order Ordinary Differential Equations

Consider the second-order ODE:

$$
y'' + p(x) y' + q(x)y = r(x) 
$$

If $r(x) = 0$, it is called homogeneous. If the solutions for $y(x)$ are $y_1$ and $y_2$, then $c_1 y_1 + c_2 y_2$ is also a solution for $y$. If $k_1 y_1 + k_2 y_2 = 0$ and $k_1 = 0$ and $k_2 = 0$, the solutions are **linearly independent**. If $k_1 \neq 0$ and $k_2 \neq 0$, they are **linearly dependent**, meaning $y_1$ and $y_2$ are multiples of each other, $y_2 = k y_1$.

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

If $W = 0$ for all $x$, the solutions are **linearly dependent**.

### Solving Homogeneous Equations

$$
y'' + p(x) y' + q(x)y = 0
$$

#### Reduction of Order

If $y_1$ is known, let $y_2 = u y_1$. Substitute this into the equation and differentiate, then simplify to get:

$$
u' = \frac{1}{y_1^2} e^{-h}, \quad h = \int p(x) dx
$$

#### Constant Coefficient Equations

For equations of the form:

$$
y'' + ay' + by = 0
$$

Assume the general solution $y = e^{\lambda x}$. Substituting this into the equation, we get the characteristic equation:

$$
e^{\lambda x} (\lambda^2 + a\lambda + b) = 0
$$

The characteristic equation $\lambda^2 + a\lambda + b = 0$ can be solved using the discriminant.

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

   where $\lambda = -\frac{a}{2} \pm i \omega$ and $\omega^2 = b - \frac{1}{4}a^2$.

### Euler-Cauchy Equation

For equations of the form:

$$
x^2 y'' + axy' + by = 0
$$

Assume the general solution $y = x^m$. Substituting this into the equation, we get the characteristic equation:

$$
x^m (m^2 +(a-1)m + b) = 0
$$

The characteristic equation $m^2 +(a-1)m + b = 0$ can be solved using the discriminant.

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

The general solution is $y(x) = y_h (x) + y_p(x)$, where $y_h$ is the solution to the homogeneous equation. $y_p$ depends on the form of $r(x)$.

### Coefficient Comparison Method

1. **Exponential Form**: If $r(x) = K e^{\gamma x}$, then $y_p(x) = C e^{\gamma x}$.
2. **Polynomial Form**: If $r(x) = K x^n$, then $y_p(x)$ is a polynomial of degree $n$.
3. **Trigonometric Form**: If $r(x) = K \cos \omega x$ or $r(x) = K \sin \omega x$, then $y_p(x) = K \cos \omega x + M \sin \omega x$.
4. **Combination Form**: If $r(x) = K e^{\alpha x} \cos \omega x$ or $r(x) = K e^{\alpha x} \sin \omega x$, then $y_p(x) = e^{\alpha x}( K \cos \omega x + M \sin \omega x)$.

#### Basic Rule

If $r(x)$ is a monomial, $y_p(x)$ directly follows the form above.

#### Modification Rule

If $y_h(x)$ is similar to $r(x)$, modify $y_p$ by multiplying by $x$ or $x^2$ as needed.

#### Sum Rule

If $r(x)$ consists of multiple terms, $y_p$ is the sum of corresponding solutions.

### Lagrange Method

Using the Wronskian, we can solve more complex $r(x)$ forms.

Let $W = f_1 {f_2}' - {f_1}' f_2$. Then, $y_p$ can be found as follows:

$$
y_p = -y_1 \int \frac{y_2}{W} r dx + y_2 \int \frac{y_1}{W} r dx
$$

This formula helps solve nonhomogeneous differential equations.

---

By following these steps and methods, you can solve both homogeneous and nonhomogeneous second-order ODEs efficiently.


[In Korean]
# 이계 상미분 방정식

이계 상미분 방정식은 다음과 같이 주어진다:

$$
y'' + p(x) y' + q(x)y = r(x) 
$$

$r(x) = 0$이면 동차(homogeneous)라고 한다. $y(x)$의 해가 $y_1$과 $y_2$라면, $c_1 y_1 + c_2 y_2$도 $y$의 해이다. $k_1 y_1 + k_2 y_2 = 0$에서 $k_1 = 0$이고 $k_2 = 0$이면 **일차 독립**이고, $k_1 \not= 0$이고 $k_2 \not= 0$이면 **일차 종속**이다. 일차 종속일 때, $y_1$과 $y_2$의 관계는 실수 배이다, 즉 $y_2 = k y_1$이다.

→ 일차 종속의 여부를 확인하는 방법:

## Wronskian 방법

$$
W(y_1, y_2) = 
\begin{vmatrix}
y_1 & y_2 \\
y_1' & y_2'
\end{vmatrix}
= y_1 y_2' - y_1' y_2
$$

위 식에서 $W = 0$일 때, 모든 $x$에 대해 **일차 종속**이다.

### 동차 방정식 풀이법

$$
y'' + p(x) y' + q(x)y = 0
$$

#### 해의 감소법

$y_1$을 알면, $y_2 = uy_1$로 두고, 위의 식에 대입하고 정리하여 다음과 같은 일반식을 얻는다:

$$
u' = \frac{1}{y_1^2} e^{-h}, \quad h = \int p(x) dx
$$

#### 상수 계수 이계 상미분 방정식

방정식이 다음과 같은 형태일 때:

$$
y'' + ay' + by = 0
$$

기본 해는 $y = e^{\lambda x}$이다. 이를 방정식에 대입하면 특성 방정식을 얻는다:

$$
e^{\lambda x} (\lambda^2 + a\lambda + b) = 0
$$

특성 방정식 $\lambda^2 + a\lambda + b = 0$은 판별식을 이용해 풀 수 있다.

- **첫 번째 케이스**: 판별식이 양수일 때 (서로 다른 두 실근)

$$
y(x) = c_1 e^{\lambda_1 x} + c_2 e^{\lambda_2 x}
$$

- **두 번째 케이스**: 판별식이 0일 때 (중근일 때)

$$
y(x) = (c_1 + c_2 x)e^{-\frac{a}{2}x}
$$

- **세 번째 케이스**: 판별식이 음수일 때 (서로 다른 두 허근)

$$
y(x) = e^{-\frac{a}{2}x} (A \cos \omega x + B \sin \omega x)
$$

여기서 $\lambda = -\frac{a}{2} \pm i \omega$, $\omega^2 = b - \frac{1}{4}a^2$.


### 오일러-코시 방정식

방정식이 다음과 같은 형태일 때:

$$
x^2 y'' + axy' + by = 0
$$

기본 해는 $y = x^m$이다. 이를 방정식에 대입하면 특성 방정식을 얻는다:

$$
x^m (m^2 +(a-1)m + b) = 0
$$

특성 방정식 $m^2 +(a-1)m + b = 0$은 판별식을 이용해 풀 수 있다.

- **첫 번째 케이스**: 판별식이 양수일 때 (서로 다른 두 실근)

$$
y(x) = c_1 x^{m_1} + c_2 x^{m_2}
$$

- **두 번째 케이스**: 판별식이 0일 때 (중근일 때)

$$
y(x) = (c_1 + c_2 \ln x)x^m , \quad (m = \frac{1}{2}(1-a))
$$

- **세 번째 케이스**: 판별식이 음수일 때 (서로 다른 두 허근)

    흔히 나오지 않으므로 생략한다.

## 비동차 방정식 풀이법

$$
y'' + p(x) y' + q(x)y = r(x), \quad (r(x) \neq 0)
$$

일반 해: $y(x) = y_h (x) + y_p(x)$

여기서 $y_h$는 동차 방정식의 해이다. 즉, $r(x) = 0$일 때의 해를 구한 다음 풀이하는 방식이다. $y_p$는 $r(x)$의 형태에 의존하는 방식이다.

### 계수 비교법

1. **지수 함수 형태**: $r(x) = K e^{\gamma x}$이면, $y_p(x) = C e^{\gamma x}$.
2. **다항식 형태**: $r(x) = K x^n$이면, $y_p(x)$는 차수가 $n$인 다항식이다.
3. **삼각 함수 형태**: $r(x) = K \cos \omega x$ 또는 $r(x) = K \sin \omega x$이면, $y_p(x) = K \cos \omega x + M \sin \omega x$.
4. **결합 형태**: $r(x) = K e^{\alpha x} \cos \omega x$ 또는 $r(x) = K e^{\alpha x} \sin \omega x$이면, $y_p(x) = e^{\alpha x}( K \cos \omega x + M \sin \omega x)$.

#### 기본 규칙

$r(x)$가 단항식일 때, $y_p(x)$는 위의 형태를 따른다.

#### 수정 규칙

만약 동차 방정식의 해 $y_h(x)$가 $r(x)$와 유사하다면, $y_p$에 $x$ 또는 $x^2$을 곱하여 수정한다.

#### 합 규칙

$r(x)$가 여러 항으로 이루어진 경우, $y_p$는 각각의 해를 더하여 구한다.

### 라그랑주 방법

Wronskian을 사용하여 보다 복잡한 $r(x)$ 형태를 해결할 수 있다.

$W = f_1 {f_2}' - {f_1}' f_2$로 두고, $y_p$를 다음과 같이 구할 수 있다:

$$
y_p = -y_1 \int \frac{y_2}{W} r dx + y_2 \int \frac{y_1}{W} r dx
$$

이 공식을 이용하면 비동차 미분 방정식을 풀 수 있다.

---

이와 같은 방법을 따르면 동차 및 비동차 이계 상미분 방정식을 효율적으로 풀 수 있다.
