# In English

## Linear Simultaneous Equations

A linear function is a function where the exponent of the independent variable is 1, meaning its graph is a straight line. When multiple such variables and equations are involved, it forms a system of linear simultaneous equations.

While linear simultaneous equations are commonly covered in middle and high school mathematics, it’s important to re-establish our approach to solving them, especially since the same methods apply when dealing with matrices. Therefore, a brief review of solving linear simultaneous equations is necessary.

Consider the following system of equations:

$$
(*)\cdots 
\begin{cases}
a_{11} x_1 +  a_{21} x_2 + \cdots + a_{n1}x_n = b_1
\\
a_{12} x_1 + a_{22}x_2 + \cdots + a_{n2}x_n = b_2
\\
~~~\vdots ~~~~~~~~~~~~ \vdots~~~~~~~~~~~~~~~~~~~~~~~~\vdots~~~~~~~~~~~\vdots 
\\
a_{1m}x_1 + a_{2m}x_2 + \cdots + a_{nm}x_n = b_n
\end{cases}
$$

If $n = m$, a unique solution exists, but if they differ, a definite solution cannot be determined. In such cases, solutions may involve free variables like $s$, leading to infinitely many solutions, but only in form.

In a system of linear equations, if all ${b_n}$ are zero, it’s called a homogeneous system; otherwise, it’s a non-homogeneous system.

## Basic Operations for Solving Simultaneous Equations

There are three fundamental operations:

### (S1)

$S_i ⇔ S_j$

### (S2)

$cS_i → S_i$

### (S3)

$S_i + cS_j → S_j$

Let’s explore these three operations.

**S1** refers to swapping. Swapping the $i$-th and $j$-th equations doesn’t affect the solution but can make the equation easier to solve, especially if you place the equation with a coefficient of $1$ for $x_1$ at the top. This can simplify the calculations.

**S2** refers to multiplying an equation by a constant. Multiplying both sides of an equation by a constant doesn’t change the solution, but it’s essential for eliminating variables. This operation is frequently used, so apply it as necessary.

**S3** involves combining the $i$-th and $j$-th equations to simplify the $j$-th equation, making it easier to solve for a variable. While this might sound confusing, it will become clearer when you see it in action in an example.

These are the basics of solving simultaneous equations. While the following problem-solving method may seem unnecessary for small systems of equations, it’s crucial when dealing with larger systems or matrices. This approach will serve as a foundation for future calculations. Even if it seems inefficient, I recommend practicing this method to solidify your understanding.



# In korean

## 선형 연립 방정식

선형 함수는 독립 변수의 지수가 1인 함수를 의미한다. 즉 자취가 직선인 함수라고 생각하면 쉽다. 이러한 변수를 여러 개, 방정식의 수를 여러 개를 둔다면 이는 선형 연립 방정식이 된다.

물론, 선형 연립 방정식은 흔히 중학교나 고등학교에서 다루는 내용이라 어렵지는 않으나, 행렬을 다룰 때 정확히 동일한 방식으로 정리할 것이기에 선형 연립방정식 풀이의 태도를 새롭게 정립하는 과정이 필요할 것 같아, 한번 더 정리하는 것이다.

먼저, 아래와 같은 방정식들의 모임을 우리는 선형 연립방정식이라 부른다.

$$
(*)\cdots 
\begin{cases}
a_{11} x_1 +  a_{21} x_2 + \cdots + a_{n1}x_n = b_1
\\
a_{12} x_1 + a_{22}x_2 + \cdots + a_{n2}x_n = b_2
\\
~~~\vdots ~~~~~~~~~~~~ \vdots~~~~~~~~~~~~~~~~~~~~~~~~\vdots~~~~~~~~~~~\vdots 
\\
a_{1m}x_1 + a_{2m}x_2 + \cdots + a_{nm}x_n = b_n
\end{cases}
$$

만약, $n=m$이면, 해가 존재하지만, 다를 경우 명확한 해를 구할 수 없다. 즉 자유 변수 $s$와 같은 것을 넣어 무수히 많은 해가 있지만, 형태만을 구할 수 있다.

이때 선형 연립 방정식에서 , ${b_n}$이 $0$이면 재차 방정식, $0$이 아니면, 비재차 방정식이라 부른다.

## 연립 방정식의 기본 연산

기본 연산은 3개가 있다.

### (S1)

$S_i ⇔ S_j$

### (S2)

$cS_i → S_i$

### (S3)

$S_i + cS_j → S_j$

이렇게 3가지 연산만 기억하자.

S1의 의미는 교체이다. $i$ 번째 방정식과, $j$번째 방정식을 교체한다고, 방정식의 영향을 주지 않기에 연산이라 보지 않을 수도 있겠지만, 연립방정식을 손으로 풀어야 하는 우리 입장에서는 분수와 같은 형태가 나오면 풀이하기에 복잡함을 경험할 수 있을 것이다. 쉬운 계산을 위해 첫 번째 변수인 $x_1$의 계수가 $1$인 식을 맨 위에 두고 풀면 더 편한 경험을 할 수 있기에, 교체를 적절히 잘 확인해보자.

S2의 의미는 상수배이다. 연립방정식의 양변에 상수배를 해도 해에는 영향을 주지 않으나, 변수의 소거를 위해 반드시 필요한 작업이다. 이는 자주 사용되니, 반드시 적절하게 사용하자.

S3의 의미는 $i$번째 항과, $j$번째 항을 적절히 조합해 $j$번째 항에 대입하여 변수를 쉽게 구하도록 하는 것이다. 이 말자체가 헷갈릴 수도 있겠으나, 이는 예제를 푸는 과정을 보면 더욱 이해가 쉬울 것이다.

이렇게 연립 방정식의 기본을 정리해보았다. 물론, 푸는 문제풀이 방법은 개수가 적은 연립 방정식에서는 무의미할 수도 있다. 당연하다. 하지만 이 과정을 행렬에 적용해보면 더욱 빠른 풀이가 가능하며, 이를 기본으로 삼아 앞으로 계산을 진행할 것이다. 비효율적이라고 생각해도, 반드시 이런 풀이를 진행해보길 권한다.













