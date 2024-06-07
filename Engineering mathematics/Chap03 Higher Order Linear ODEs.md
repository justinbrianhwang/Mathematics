[In korean]
# Higher-Order Differential Equations

Higher-order differential equations have the form:

$$
F(x, y, y', \cdots, y^{(n)}) = 0
$$

The standard form is:

$$
y^{(n)} + p_n(x) y^{(n-1)} + \cdots + p_0(x) y = r(x)
$$

As with second-order differential equations, if \( r(x) = 0 \), the equation is homogeneous; otherwise, it is nonhomogeneous. Let's first consider the case where \( r(x) = 0 \).

## Homogeneous Higher-Order Linear ODEs

**General Solution**

The general solution can be expressed as:

$$
y(x) = c_1 y_1 + c_2 y_2 + \cdots + c_n y_n
$$

As with second-order differential equations, the concepts of linear independence and linear dependence exist. If two or more of the \( n \) terms can be expressed as multiples of each other, they are linearly dependent. To check for linear dependence, the Wronskian can be used, similar to second-order differential equations.

$$
W(y_1, y_2, \cdots, y_n) = 
\begin{vmatrix} 
y_{1} & y_{2} & \cdots & y_{n} \\
y_{1}' & y_{2}' & \cdots & y_{n}' \\
\vdots & \vdots & \ddots & \vdots \\
y_{1}^{(n-1)} & y_{2}^{(n-1)} & \cdots & y_{n}^{(n-1)} \\
\end{vmatrix} 
$$

### Constant Coefficient Higher-Order Differential Equations

For the equation:

$$
y^{(n)} + a_{n-1} y^{(n-1)} + \cdots + a_0 y = 0
$$

The solution form is \( y = e^{\lambda x} \). The characteristic equation is:

$$
\lambda^n + a_{n-1} \lambda^{n-1} + \cdots + a_0 = 0
$$

This characteristic equation must account for real roots, repeated roots, and complex roots.

## Nonhomogeneous Higher-Order Linear ODEs

For the equation:

$$
y^{(n)} + p_{n-1} y^{(n-1)} + \cdots + p_0 y = r(x), \quad (r(x) \neq 0)
$$

The general solution is:

$$
y(x) = y_h(x) + y_p(x)
$$

Here, \( y_h(x) \) is the solution to the homogeneous equation. To find \( y_p(x) \), there are two methods:

### Coefficient Comparison Method

First, solve for \( y_h(x) \) and then determine \( y_p(x) \) based on the form of \( r(x) \).

### Method of Variation of Parameters

$$
y_p(x) = \sum_{k=1}^{n} y_k(x) \int \frac{W_k}{W} r(x) \, dx
$$

The rest requires knowledge of linear algebra.


[In English]
# 고계 미분 방정식

고계 미분 방정식은 다음과 같은 형태를 가진다:

$$
F(x, y, y', \cdots, y^{(n)}) = 0
$$

표준형은 다음과 같다:

$$
y^{(n)} + p_n(x) y^{(n-1)} + \cdots + p_0(x) y = r(x)
$$

이계 미분 방정식과 마찬가지로, \( r(x) \)가 \( 0 \)이냐 아니냐에 따라 동차(homogeneous)인지 비동차(nonhomogeneous)인지 구분할 수 있다. 먼저 \( r(x) = 0 \)일 때를 다루어 보자.

## 동차 고계 선형 미분 방정식

**일반 해**

일반 해는 다음과 같이 표현할 수 있다:

$$
y(x) = c_1 y_1 + c_2 y_2 + \cdots + c_n y_n
$$

이계 미분 방정식과 마찬가지로 선형 독립과 선형 종속의 개념이 존재한다. \( n \)개의 항 중에서 2개 이상이 실수 배로 표현될 수 있으면 선형 종속이라 할 수 있다. 선형 종속의 여부를 확인하기 위해 Wronskian을 이용해 판별할 수 있다.

$$
W(y_1, y_2, \cdots, y_n) = 
\begin{vmatrix} 
y_{1} & y_{2} & \cdots & y_{n} \\
y_{1}' & y_{2}' & \cdots & y_{n}' \\
\vdots & \vdots & \ddots & \vdots \\
y_{1}^{(n-1)} & y_{2}^{(n-1)} & \cdots & y_{n}^{(n-1)} \\
\end{vmatrix} 
$$

### 상수 계수로 이루어진 고계 미분 방정식

다음과 같은 방정식에 대해:

$$
y^{(n)} + a_{n-1} y^{(n-1)} + \cdots + a_0 y = 0
$$

해의 꼴은 \( y = e^{\lambda x} \)이다. 특성 방정식은 다음과 같다:

$$
\lambda^n + a_{n-1} \lambda^{n-1} + \cdots + a_0 = 0
$$

이 특성 방정식은 실근, 중근, 허근을 모두 포함하여 해를 구해야 한다.

## 비동차 고계 선형 미분 방정식

다음과 같은 형태의 방정식이다:

$$
y^{(n)} + p_{n-1} y^{(n-1)} + \cdots + p_0 y = r(x), \quad (r(x) \neq 0)
$$

일반 해는 다음과 같이 표현된다:

$$
y(x) = y_h(x) + y_p(x)
$$

여기서 \( y_h(x) \)는 동차 방정식의 해이다. \( y_p(x) \)를 특정하기 위해 두 가지 방법이 있다.

### 계수 비교법

먼저 \( y_h(x) \)를 구한 뒤 \( r(x) \)를 보고, 적절한 \( y_p(x) \)를 특정한다.

### 매개변수 변환법

$$
y_p(x) = \sum_{k=1}^{n} y_k(x) \int \frac{W_k}{W} r(x) \, dx
$$

나머지는 선형대수학을 배우고 나서...

