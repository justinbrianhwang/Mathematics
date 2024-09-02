# In English

## Linear Simultaneous Equations

A linear function is one where the exponent of the independent variable is 1, meaning its graph is a straight line. When dealing with multiple variables and equations, we form a system of linear simultaneous equations.

Although linear simultaneous equations are commonly taught in middle and high school mathematics, it's essential to revisit the methods for solving them, particularly because the same techniques apply when working with matrices. Thus, a brief review of solving linear simultaneous equations is necessary.

Consider the following system of equations:

$$
\begin{cases}
a_{11} x_1 +  a_{21} x_2 + \cdots + a_{n1}x_n = b_1 \\
a_{12} x_1 + a_{22}x_2 + \cdots + a_{n2}x_n = b_2 \\
\vdots \\
a_{1m}x_1 + a_{2m}x_2 + \cdots + a_{nm}x_n = b_n
\end{cases}
$$

If $n = m$, a unique solution exists. However, if they differ, a definite solution cannot be determined. In such cases, solutions may involve free variables like $s$, leading to infinitely many solutions, but only in form.

In a system of linear equations, if all $b_n$ are zero, it’s called a homogeneous system; otherwise, it’s a non-homogeneous system.

## Basic Operations for Solving Simultaneous Equations

There are three fundamental operations:

### (S1) 

$$S_i \iff S_j$$

### (S2) 

$$cS_i \rightarrow S_i$$

### (S3) 

$$S_i + cS_j \rightarrow S_j$$

Let’s explore these three operations.

**S1** refers to swapping. Swapping the $i$-th and $j$-th equations doesn’t affect the solution but can make the equation easier to solve, especially if you place the equation with a coefficient of $1$ for $x_1$ at the top. This can simplify the calculations.

**S2** refers to multiplying an equation by a constant. Multiplying both sides of an equation by a constant doesn’t change the solution, but it’s essential for eliminating variables. This operation is frequently used, so apply it as necessary.

**S3** involves combining the $i$-th and $j$-th equations to simplify the $j$-th equation, making it easier to solve for a variable. While this might sound confusing, it will become clearer when you see it in action in an example.

These are the basics of solving simultaneous equations. While the following problem-solving method may seem unnecessary for small systems of equations, it’s crucial when dealing with larger systems or matrices. This approach will serve as a foundation for future calculations. Even if it seems inefficient, I recommend practicing this method to solidify your understanding.

# In Korean

## 선형 연립 방정식

선형 함수는 독립 변수의 지수가 1인 함수로, 그래프가 직선으로 나타나는 특징이 있습니다. 여러 개의 변수와 방정식을 다룰 때, 선형 연립 방정식의 시스템이 형성됩니다.

선형 연립 방정식은 중학교와 고등학교 수학에서 흔히 다루지만, 행렬을 다룰 때도 동일한 방법을 사용하기 때문에 그 풀이 방법을 다시 한 번 점검하는 것이 중요합니다. 따라서 선형 연립 방정식의 풀이에 대해 간단히 정리해보겠습니다.

다음과 같은 방정식 시스템을 고려해 봅시다:

$$
\begin{cases}
a_{11} x_1 +  a_{21} x_2 + \cdots + a_{n1}x_n = b_1 \\
a_{12} x_1 + a_{22}x_2 + \cdots + a_{n2}x_n = b_2 \\
\vdots \\
a_{1m}x_1 + a_{2m}x_2 + \cdots + a_{nm}x_n = b_n
\end{cases}
$$

만약 $n = m$이면 유일한 해가 존재하지만, 그렇지 않다면 명확한 해를 구할 수 없습니다. 이 경우 자유 변수 $s$와 같은 변수를 포함한 해를 얻을 수 있지만, 형태만 구할 수 있으며, 무수히 많은 해가 존재하게 됩니다.

선형 연립 방정식에서, 모든 $b_n$이 0이면 이것을 동차 방정식이라고 부르고, 0이 아니면 비동차 방정식이라고 부릅니다.

## 연립 방정식의 기본 연산

기본 연산은 세 가지가 있습니다:

### (S1) 

$$S_i \iff S_j$$

### (S2) 

$$cS_i \rightarrow S_i$$

### (S3) 

$$S_i + cS_j \rightarrow S_j$$

이제 이 세 가지 연산을 살펴보겠습니다.

**S1**은 교환을 의미합니다. $i$번째 방정식과 $j$번째 방정식을 교환해도 해에는 영향을 주지 않지만, $x_1$의 계수가 1인 방정식을 맨 위에 놓으면 계산이 더 쉬워질 수 있습니다.

**S2**는 상수배를 의미합니다. 방정식의 양변에 상수를 곱해도 해에는 영향을 주지 않지만, 변수 제거를 위해 필수적인 작업입니다. 이 연산은 자주 사용되므로 적절히 활용해야 합니다.

**S3**은 $i$번째 방정식과 $j$번째 방정식을 조합하여 $j$번째 방정식을 더 쉽게 풀 수 있도록 단순화하는 것입니다. 처음에는 혼란스러울 수 있지만, 예제를 통해 이 방법을 보면 더 명확해질 것입니다.

이것이 연립 방정식을 푸는 기본입니다. 연립 방정식의 수가 적을 때는 이 방법이 불필요해 보일 수 있지만, 행렬과 같은 더 큰 시스템을 다룰 때는 필수적인 접근법입니다. 이 방법을 익히면 이후 계산에서 큰 도움이 될 것입니다. 비효율적으로 보일 수 있지만, 반드시 연습해보시기를 권장합니다.
