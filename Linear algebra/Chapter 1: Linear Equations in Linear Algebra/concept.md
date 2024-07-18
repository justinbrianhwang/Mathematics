# In English

### 1. Systems of Linear Equations

An equation of the form $ax + b$ is called a linear equation, where $x$ is the variable.

The goal of the equation is to find $x$. Before discussing the term "equation," let's first explore the relationship of the term "expression."

![Linear Equation1](https://i.imgur.com/wr7zuZu.png)

Let's summarize the basic form of a linear equation through the diagram above.

(i) If $a \not = 0$ → Multiply both sides by $a^{-1}$. 
⇒ $x = a^{-1}b$

(ii) If $a = 0 ,~ b \not = 0$ → No solution.

(iii) If $a = 0 ,~ b = 0$ → $x$ can be any real number.

⇒ The above conditions are concepts learned in middle school, and while they are easy to understand, they will be very important when studying linear algebra in the future.

[General Case]

$a _ {1} x_1 + a_2 x_2 + \cdots + a_n x_n = b$ (where $a_i$ is the coefficient of $x_i$)

⇒ The ultimate goal of the above equation is to find the solution. Since there are more unknowns than equations, it is called an "indeterminate equation."

[Solving Systems of Equations]

It's helpful to know the following notation for understanding the concepts.

$a_{mn}$: $m$ → number of equations, $n$ → number of unknowns

A system of equations with such coefficients is called an $m \times n$ system of linear equations.

Now that we are familiar with the notation, let's examine the following system of equations.

$$
\begin{cases}
a_{11} x_1 + a_{12} x_2 + \cdots + a_{1n} x_n = b_1 \\
a_{21} x_1 + a_{22} x_2 + \cdots + a_{2n} x_n = b_2 \\
\vdots \\
a_{m1} x_1 + a_{m2} x_2 + \cdots + a_{mn} x_n = b_m
\end{cases}
$$

The solution to the above system of equations means the intersection of the solutions to each indeterminate equation.

① If $b_i = 0 ,~ \forall i = 1 ,~ 2 ,~ \cdots ,~ m$:

$$
\begin{cases}
a_{11} x_1 + a_{12} x_2 + \cdots + a_{1n} x_n = 0 \\
a_{21} x_1 + a_{22} x_2 + \cdots + a_{2n} x_n = 0 \\
\vdots \\
a_{m1} x_1 + a_{m2} x_2 + \cdots + a_{mn} x_n = 0
\end{cases}
$$

⇒ Such equations are called **homogeneous equations**.

If the solution is $x_1 = x_2 = \cdots = x_n = 0$, it is called a **trivial solution**.

⇒ It is important to find non-trivial solutions for homogeneous equations.

② If $b_i \not = 0 ,~ \forall i = 1 ,~ 2 ,~ \cdots ,~ m$:

⇒ Such equations are called **non-homogeneous equations**.

Solving non-homogeneous equations can actually be more difficult.

### Types of Solutions

1. Particular Solution: A specific solution to the equation
2. General Solution: The set of all solutions to the equation
3. Trivial Solution: For homogeneous equations, the solution $x_1 = x_2 = \cdots = x_n = 0$
4. Non-Trivial Solution: Solutions to homogeneous equations where not all $x_i$ are zero

⇒ Consistent ↔ When the equation has a solution

⇒ Inconsistent ↔ When the equation has no solution

### 2. Solving Systems of Linear Equations

(1) Equivalent Systems

$$
\begin{cases}
x + 2y = 3 &  ~~~ \cdots ① \\
x + 3y = 2 &  ~~~ \cdots ②
\end{cases}
$$

⇒ $-1 \times ① + ② \rightarrow ②$

$$
\begin{cases}
x + 2y = 3 &  ~~~ \cdots ① \\
y = -1 &  ~~~ \cdots ②
\end{cases}
$$

⇒ $-2 \times ② + ① \rightarrow ①$

$$
\begin{cases}
x = 5 &  ~~~ \cdots ① \\
y = -1 &  ~~~ \cdots ②
\end{cases}
$$

→ This process helps find the solution.

(2) Basic Operations for Systems of Equations → Elementary Row Operations of Matrices

Express the given system of equations as follows.

$S_1 ,~ S_2 ,~ \cdots ,~ S_i ,~ \cdots ,~ S_j ,~ \cdots ,~ S_n$

Using the given system of equations, let's explore the operations.

Operation 1) $S_i \leftrightarrow S_j$: Swap the $i$-th equation with the $j$-th equation.

Operation 2) $cS_i \rightarrow S_i$: Multiply the $i$-th equation by a constant $c$, where $c \not = 0$.

Operation 3) $S_i + c S_j \rightarrow S_i$: Replace the $i$-th equation with the result of the operation.

⇒ These three operations form the basis for elementary row operations in matrices.

### 3. Matrices

A matrix is a rectangular array of numbers (variables, functions, etc.).

(1) $m \times n$ Matrix

$$
A = [a_{i , j}]{m \times n} = \begin{bmatrix}
a_{11} & a_{12} & \cdots & a_{1j} & \cdots & a_{1n} \\
a_{21} & a_{22} & \cdots & a_{2j} & \cdots & a_{2n} \\
\vdots & \vdots & & \vdots & & \vdots \\
a_{i1} & a_{i2} & \cdots & a_{ij} & \cdots & a_{in} \\
\vdots & \vdots & & \vdots & & \vdots \\
a_{m1} & a_{m2} & \cdots & a_{mj} & \cdots & a_{mn}
\end{bmatrix}
$$


① $A$ is called an $m \times n$ matrix, and $m \times n$ is the size of matrix $A$.

② The horizontal rows of matrix $A$ are called **rows** , and the vertical columns are called **columns**.

③ $a_{ij}$ is called the $(i ,~ j)$-th element or entry of matrix $A$.

④ $A_{(i)} = 
\begin{bmatrix}
a_{i1} & a_{i2} & \cdots & a_{in}
\end{bmatrix}$: The $i$-th $1 \times n$ **row** vector of matrix $A$.

⑤ $A^{(j)} = 
\begin{bmatrix}
a_{1j} \\
a_{2j} \\
\vdots \\
a_{mj}
\end{bmatrix}$: The $j$-th $m \times 1$ **column** vector of matrix $A$.

⑥ $A = 
\begin{bmatrix}
A_{(1)} \\
A_{(2)} \\
\vdots \\
A_{(m)}
\end{bmatrix}
=
\begin{bmatrix}
A^{(1)} &
A^{(2)} &
\cdots &
A^{(n)}
\end{bmatrix}$: The row vector and column vector representations of matrix $A$.

⑦ When $m = n$, matrix $A = [a_{ij}]_{n \times n}$ is called an $n$th-order square matrix. Additionally, $a_{11} ,~ a_{22} ,~ \cdots ,~ a_{nn}$ are called the **main diagonal elements** of $A$.

(2) Set of Matrices $M_{m ,~ n} (\R) = M_{m ,~ n}$

① $M_{m ,~ n} (\R) = \{ A | A = [a_{ij}]_{m \times n} ,~ a_{ij} \in \R \}$: The set of $m \times n$ matrices.

② When $m = n$, $M_{n ,~ n} = M_n$: The set of square matrices.

(3) Equality of Matrices

When $A = [a_{ij}] ,~ B = [b_{ij}] \in M_{m ,~ n}$, if the elements of $A$ and $B$ are the same, the two matrices are **equal** and defined as follows.

$$
A = B \leftrightarrow a_{ij} = b_{ij} ,~ \forall i ,~ j
$$

(4) Zero Matrix

$O = [o_{i ,~ j}] \in M_{m ,~ n}$: Zero matrix ↔ $o_{ij} = 0 ,~ \forall i ,~ j$

### 4. Matrix Operations

To treat matrices as mathematical objects, we define the basic operations of addition, scalar multiplication, and multiplication, and explore their properties.

(1) Addition and Subtraction

When $A = [a_{ij}] ,~ B = [b_{ij}] \in M_{m ,~ n}$:

① Addition:

$$
A + B = [a_{ij}] + [b_{ij}] = [a_{ij} + b_{ij}]
$$

② Subtraction:

$$
A - B = [a_{ij}] - [b_{ij}] = [a_{ij} - b_{ij}]
$$

③ Basic Properties

When $A ,~ B ,~ C \in M_{m ,~ n}$, the following hold:

(1) $A + B = B + A$  ⇒ Commutative Property

(2) $(A + B) + C = A + (B + C)$ ⇒ Associative Property

(3) $A + O = A$ ⇒ Additive Identity

(4) $A + (-A) = O$ ⇒ Additive Inverse

(2) Scalar Multiplication

① Definition

When $A = [a_{ij}] \in M_{m ,~ n}$ and $k \in \R$, it is defined as follows:

$$
kA = k[a_{ij}] = 
\begin{bmatrix}
k a_{11} & k a_{12} & \cdots & k a_{1n} \\
k a_{21} & k a_{22} & \cdots & k a_{2n} \\
\vdots & \vdots & & \vdots \\
k a_{m1} & k a_{m2} & \cdots & k a_{mn}
\end{bmatrix}
$$

② Basic Properties

When $A ,~ B \in M_{m ,~ n}$ and $\alpha ,~ \beta \in \R$, the following hold:

(1) $\alpha (A + B) = \alpha A + \alpha B$

(2) $(\alpha + \beta) A = \alpha A + \beta A$

(3) $(\alpha \beta) A = \alpha (\beta A) = \beta (\alpha A)$

(4) $1 A = A$

(3) Matrix Multiplication

For two matrices $A = [a_{ik}] \in M_{m ,~ p}$ and $B = [b_{kj}] \in M_{p ,~ n}$, the product $A \cdot B$ is defined as follows:

$$
AB := [c_{ij}] \in M_{m ,~ n} ,~ c_{ij} := a_{i1} b_{1j} + a_{i2} b_{2j} + \cdots + a_{ip} b_{pj} = \sum_{k=1}^{p} a_{ik} b_{kj}
$$

⇒ Note: $AB \not = BA$ (Commutative Property does not hold)

The idea of matrix multiplication is as follows:

$a_1 x_1 + a_2 x_2 + \cdots a_n x_n = b$

↔ $<a_1 ,~ a_2 ,~ \cdots ,~ a_n> \cdot <x_1 ,~ x_2 ,~ \cdots x_n> = b$

↔ 
$$
\begin{bmatrix}
a_1 & a_2 & \cdots & a_n  
\end{bmatrix}
\begin{bmatrix}
x_1 \\ x_2 \\ \vdots \\ x_n  
\end{bmatrix}
=b
$$

### 5. Properties of Matrix Multiplication

(1) Matrix Multiplication using Row and Column Vectors

For $A = [a_{ik}] \in M_{m ,~ p}$ and $B = [b_{kj}] \in M_{p ,~ n}$, the following hold:

① $A_{(i)} B^{(j)} = 
\begin{bmatrix}
a_{i1} & a_{i2} & \cdots & a_{in}  
\end{bmatrix}
\begin{bmatrix}
b_{1j} \\
b_{2j} \\
\vdots \\
b_{pj}
\end{bmatrix}
= \sum_{k=1}^{p} a_{ik} b_{kj}$

② $(AB)_{(ij)} = A_{(i)} B^{(j)}$

③ $AB =
\begin{bmatrix}
A_{(1)} B^{(1)} & A_{(1)} B^{(2)} & \cdots & A_{(1)} B^{(n)} \\
A_{(2)} B^{(1)} & A_{(2)} B^{(2)} & \cdots & A_{(2)} B^{(n)} \\
\vdots & \vdots & & \vdots \\
A_{(m)} B^{(1)} & A_{(m)} B^{(2)} & \cdots & A_{(m)} B^{(n)}
\end{bmatrix}$

④ $(AB)_{(i)} = A_{(i)} B ,~ (AB)^{(j)} = AB^{(j)}$

(2) Transpose of a Matrix

① Definition

A matrix obtained by exchanging the rows and columns of matrix $A$ is called the transpose of $A$ and is denoted by $A^t$ or $A^T$.

$$
A = [a_{ij}] \in M_{m ,~ n} \leftrightarrow A^t = [\hat{a}_{ij}] \in M_{n ,~ m} ,~ \hat{a}_{ij} = a_{ji}
$$

② Basic Properties

When $A ,~ B \in M_{m ,~ n}$ and $k \in \R$, the following hold:

1) $(A^t)^t = A$

2) $(A \pm B)^t = A^t \pm B^t$

3) $(kA)^t = k A^t$

(3) Properties of Matrix Multiplication

① When $A ,~ B \in M_{m ,~ p}$ and $C \in M_{p ,~ n}$, $(A \pm B) C = AC \pm BC$ (Distributive Property)

② When $A \in M_{m ,~ p} ,~ B \in M_{p ,~ q}$, and $C \in M_{q ,~ n}$, $(AB) C = A(BC)$ (Associative Property)

③ When $A \in M_{m ,~ p} ,~ B \in M_{p ,~ n}$, $(AB)^t = B^t A^t$ (Transpose of a Product)

(4) Cautions in Properties of Matrix Multiplication

The following statements do not hold:

① If $A^2 = O$, then $A = O$. ⇒ False

② If $AB = O$, then $A = O$ or $B = O$. ⇒ False

③ If $A (B + C) = O$, then $A = O$ or $B + C = O$. ⇒ False

④ If $AC = BC$, then $A = B$ or $C = O$. ⇒ False

⑤ If $AB = AC$ and $A \not = O$, then $B = C$. ⇒ False




# In Korean

### 1. 연립일차방정식

$ax + b$과 같은 형태를 일차 방정식이라 하며, $x$는 변수이다. 

결국 방정식의 목표는 $x$를 찾는 것이다. 방정식이라는 용어를 보기 전, 먼저 ‘식’이라는 용어의 관계를 살펴볼 것이다. 

![Linear Equation1](https://i.imgur.com/wr7zuZu.png)

위의 그림을 통해 일차방정식의 기본꼴을 정리해보자. 

(i) $a \not = 0$ → $a^{-1}$을 양변에 곱하면 된다. 
⇒ $x = a^{-1}b$로 표현가능

(ii) $a = 0 , ~ b \not = 0$ → 해가 없다. 

(iii) $a = 0 , ~ b = 0$ → $x$는 모든 실수

⇒ 위 조건은 중학교에서 배웠을 개념이고, 누구나 받아들이는 쉬운 개념이지만 앞으로 선형대수학을 공부하는 과정에서 매우 중요한 개념이 될 것이다. 

[보편적인 경우]

$a _ {1} x_1 + a_2 x_2 + \cdots + a_n x_n = b$ (단, $a_i$는 $x_i$의 계수)

⇒ 위의 방정식의 궁극적인 목표는 해를 찾는 것이다. 위의 식만 보면 미지수의 수가 방정식의 수보다 많으므로, 이를 “부정방정식”이라 한다. 

[연립 방정식의 풀이]

다음과 같은 표현을 먼저 알아두고 가는 것이 개념 정리하기에 좋을 것이다. 

$a_{mn}$: $m$→ 방정식의 수, $n$ → 미지수의 수

위와 같은 계수를 가진 방정식을 $m \times n$ 연립 일차 방정식이라 한다. 

이제 위의 표현을 익혔으니, 다음과 같은 연립방정식을 살펴보자. 

$$
\begin{cases}
a_{11} x_1 + a_{12} x_2 +\cdots + a_{1n} x_n = b_1 \\
a_{21} x_1 + a_{22} x_2 +\cdots + a_{2n} x_n = b_2 \\
\vdots \\
a_{m1} x_1 + a_{m2} x_2 +\cdots + a_{mn} x_n = b_m
\end{cases}
$$

위의 방정식의 해의 의미는 각 부정방정식의 해의 교집합이 해당 연립방정식의 해라는 의미이다! 

① $b_i = 0 , ~ \forall i =1 , ~ 2 , ~ \cdots , ~ m$

$$
\begin{cases}
a_{11} x_1 + a_{12} x_2 +\cdots + a_{1n} x_n = 0 \\
a_{21} x_1 + a_{22} x_2 +\cdots + a_{2n} x_n = 0 \\
\vdots \\
a_{m1} x_1 + a_{m2} x_2 +\cdots + a_{mn} x_n = 0
\end{cases}
$$

⇒ 이와 같은 방정식을 **제차방정식**이라 한다. 

이때 해가 $x_1 = x_2 = \cdots = x_n = 0$이라면 이를 **자명한 해**라고 한다. 

⇒ 제차 방정식은 자명하지 않은 해를 알아내는 것이 중요하다. 

② $b_i \not = 0 ,~ \forall i =1 ,~ 2 ,~ \cdots ,~ m$

⇒ 이와 같은 방정식을 **비제차방정식**이라 한다. 

비제차 방정식의 풀이가 실제로 더 어려움을 느낄 수 있다.

### 해의 종류

1. 특수해: 방정식의 해 중의 하나의 해
2. 일반해: 방정식의 해 전체의 집합
3. 자명한 해: 제차 방정식 중 $x_1 = x_2 = \cdots = x_n =0$인 해
4. 자명하지 않은 해: 모두 $0$이 아닌 제차방정식의 해

⇒ 무모순 ↔ 방정식의 해가 존재할 때

⇒ 모순 ↔ 방정식의 해가 존재하지 않을 때 

### 2. 연립일차방정식의 풀이

(1) 동치

$$
\begin{cases} 
x + 2y = 3 &  ~~~ \cdots ① \\
x + 3y = 2 &  ~~~ \cdots ② 
\end{cases}
$$

⇒ $-1 \times ① + ② → ②$

$$
\begin{cases} 
x + 2y = 3 &  ~~~ \cdots ① \\
y = -1 &  ~~~ \cdots ② 
\end{cases}
$$

⇒ $-2 \times ② + ① → ①$

$$
\begin{cases} 
x = 5 &  ~~~ \cdots ① \\
y = -1 &  ~~~ \cdots ② 
\end{cases}
$$

→ 다음과 같은 계산 과정을 통해 해를 구하는 것이다. 

(2) 연립 방정식의 기본 연산 → 행렬의 기본행 연산

주어진 연립 방정식의 집합을 다음과 같이 표현하자. 

$S_1 ,~ S_2 ,~ \cdots ,~ S_i ,~ \cdots ,~ S_j ,~ \cdots ,~ S_n$

위의 주어진 연립방정식을 통해 연산 방법에 대해 알아보자. 

연산 1) $S_i \leftrightarrow S_j$: $i$번째 방정식과 $j$번째 방정식을 교환한다. 

연산 2) $cS_i \rightarrow S_i$: $i$번째 방정식의 상수배이며, $c$는 $0$을 제외한 수이다. 

연산 3) $S_i + c S_j \rightarrow S_i$: $i$번째 방정식의 다음 연산 결과를 대입

⇒ 위의 3가지 연산이 추후 행렬의 기본행 연산이 된다.  

### 3. 행렬

행렬은 수(변수, 함수, 행렬 등)를 직사각형 형태로 배열한 것이다. 

(1) $m \times n$행렬

$$
A = [a_{i , j}]_{m \times n} = 
\begin{bmatrix}
 a_{11} & a_{12} & \cdots & a_{1j} & \cdots & a_{1n} \\
 a_{21} & a_{22} & \cdots & a_{2j} & \cdots & a_{2n} \\
 \vdots & \vdots & & \vdots & & \vdots \\
 a_{i1} & a_{i2} & \cdots & a_{ij} & \cdots & a_{in} \\
 \vdots & \vdots & & \vdots & & \vdots \\
 a_{m1} & a_{m2} & \cdots & a_{mj} & \cdots & a_{mn}
\end{bmatrix}
$$

① $A$를 $m \times n$행렬이라 하고 $m \times n$는 행렬 $A$의 크기라 한다. 

② 행렬 $A$의 가로줄을 **행** , 세로 줄을 **열**이라 한다.

③ $a_{ij}$를 행렬 $A$의 $(i ,~ j)$-원소 또는 성분이라 한다. 

④ $A_{(i)} = 
\begin{bmatrix}
a_{i1} & a_{i2} & \cdots & a_{in}
\end{bmatrix}$ : 행렬 $A$의 $i$번째 $1 \times n$**행**벡터

⑤ $A^{(j)} = 
\begin{bmatrix}
a_{1j} \\
a_{2j} \\
\vdots \\
a_{mj}
\end{bmatrix}$: 행렬 $A$의 $j$번째 $m \times 1$ **열**벡터 

⑥ $A = 
\begin{bmatrix}
A_{(1)} \\
A_{(2)} \\
\vdots \\
A_{(m)}
\end{bmatrix}
=
\begin{bmatrix}
A^{(1)} &
A^{(2)} &
\cdots &
A^{(n)}
\end{bmatrix}$: 행렬 $A$의 행벡터 표현과 열벡터 표현

⑦ $m = n$ ⇒ 행렬 $A = [a_{ij}]_{n \times n}$를 $n$차 정방행렬 또는 정사각행렬이라 한다. 또한, $a_{11} ,~ a_{22} ,~ \cdots ,~ a_{nn}$을 $A$의 **주대각원소**라 한다. 

(2) 행렬의 집합 $M_{m ,~ n} (\R) = M_{m ,~ n}$

① $M_{m ,~ n} (\R) = \{ A | A = [a_{ij}]_{m \times n} ,~ a_{ij} \in \R  \}$: $m \times n$ 행렬들의 집합

② $m = n$ ⇒ $M_{n ,~ n} = M_n$: 정사각행렬의 집합

(3) 행렬의 상등

$A = [a_{ij}] ,~ B = [b_{ij}] \in M_{m ,~ n}$일 때, $A$와 $B$의 원소가 같을 때, 두 행렬은 **상등**이라 하고 다음과 같이 정의된다. 

$$
A = B \leftrightarrow a_{ij} = b_{ij} ,~ \forall i ,~ j
$$

(4) 영행렬

$O = [o_{i ,~ j}] \in M_{m ,~ n}$: 영행렬 ↔ $o_{ij} = 0 ,~ \forall i ,~ j$

### 4. 행렬의 연산

 행렬을 수학적 대상으로 다루기 위해 필요한 기본 연산인 덧셈, 상수배, 곱셈들을 정의하고, 그 성질을 알아보자. 

(1) 덧셈과 뺄셈

$A = [a_{ij}] ,~ B = [b_{ij}] \in M_{m ,~ n}$일 때, 

① 덧셈: 

$$
A + B = [a_{ij}] + [b_{ij}] = [a_{ij} + b_{ij}]
$$

② 뺄셈: 

$$
A - B = [a_{ij}] - [b_{ij}] = [a_{ij} - b_{ij}]
$$

③ 기본성질

$A ,~ B ,~ C \in M_{m ,~ n}$일 때, 다음이 성립한다. 

(1) $A + B = B + A$  ⇒ 교환법칙

(2) $(A + B) + C = A + (B + C)$ ⇒ 결합법칙

(3) $A + O = A$ ⇒ 덧셈에 대한 항등원

(4) $A + (-A)  = O$ ⇒ 덧셈에 대한 역원

(2) 상수 배 또는 스칼라곱

① 정의

$A = [a_{ij}] \in M_{m ,~ n}$이고, $k \in \R$일 때, 다음과 같이 정의한다. 

$$
kA = k[a_{ij}] = 
\begin{bmatrix}
k a_{11} & k a_{12} & \cdots & k a_{1n} \\
k a_{21} & k a_{22} & \cdots & k a_{2n} \\
\vdots & \vdots & & \vdots \\
k a_{m1} & k a_{m2} & \cdots & k a_{mn}
\end{bmatrix}
$$

② 기본 성질

$A ,~ B \in M_{m ,~ n}$이고, $\alpha ,~ \beta \in \R$일 때, 다음이 성립한다.

(1) $\alpha (A + B) = \alpha A + \alpha B$

(2) $(\alpha + \beta) A = \alpha A + \beta A$

(3) $(\alpha \beta) A = \alpha (\beta A) = \beta (\alpha A)$

(4) $1 A = A$

(3) 행렬의 곱셈

두 행렬 $A = [a_{ik}] \in M_{m ,~ p} ,~ B = [b_{kj}] \in M_{p ,~ n}$일 때, 행렬 $A$와 $B$의 곱 $A \cdot B$를 다음과 같이 정의한다.

$$
AB := [c_{ij}] \in M_{m ,~ n} ,~ c_{ij} := a_{i1} b_{1j} + a_{i2} b_{2j} + \cdots + a_{ip} b_{pj} = \sum_{k=1}^{p} a_{ik} b_{kj}
$$

⇒ 주의 $AB \not = BA$ (교환법칙이 성립하지 않음)

행렬 곱셈의 idea는 다음과 같다.

$a_1 x_1 + a_2 x_2 + \cdots a_n x_n = b$

↔ $<a_1 ,~ a_2 ,~ \cdots ,~ a_n> \cdot <x_1 ,~ x_2 ,~ \cdots x_n> = b$

↔ 
$$
\begin{bmatrix}
a_1 & a_2 & \cdots & a_n  
\end{bmatrix}
\begin{bmatrix}
x_1 \\ x_2 \\ \vdots \\ x_n  
\end{bmatrix}
=b
$$

### 5. 행렬의 곱에 대한 성질

(1) 행벡터와 열벡터를 통한 행렬의 곱셈 표현

$A = [a_{ik}] \in M_{m ,~ p} ,~ B = [b_{kj}] \in M_{p ,~ n}$일 때, 다음이 성립한다. 

① $A_{(i)} B^{(j)} = 
\begin{bmatrix}
a_{i1} & a_{i2} & \cdots & a_{in}  
\end{bmatrix}
\begin{bmatrix}
b_{1j} \\
b_{2j} \\
\vdots \\
b_{pj}
\end{bmatrix}
= \sum_{k=1}^{p} a_{ik} b_{kj}$

② $(AB)_{(ij)} = A_{(i)} B^{(j)}$

③ $AB =
\begin{bmatrix}
A_{(1)} B^{(1)} & A_{(1)} B^{(2)} & \cdots & A_{(1)} B^{(n)} \\
A_{(2)} B^{(1)} & A_{(2)} B^{(2)} & \cdots & A_{(2)} B^{(n)} \\
\vdots & \vdots & & \vdots \\
A_{(m)} B^{(1)} & A_{(m)} B^{(2)} & \cdots & A_{(m)} B^{(n)}
\end{bmatrix}$

④ $(AB)_{(i)} = A_{(i)} B ,~ (AB)^{(j)} = AB^{(j)}$

(2) 전치 행렬

① 정의

행렬 $A$의 행과 열을 교환해서 얻은 행렬을 $A$의 전치행렬이라 하고 $A^t$ 또는 $A^T$로 표기한다. 

$$
A = [a_{ij}] \in M_{m ,~ n} \leftrightarrow A^t = [\hat{a}_{ij}] \in M_{n ,~ m} ,~ \hat{a}_{ij} = a_{ji}
$$

② 기본 성질

$A ,~ B \in M_{m ,~ n}$이고, $k \in \R$일 때, 다음이 성립한다. 

1) $(A^t)^t = A$

2) $(A \pm B)^t = A^t \pm B^t$

3) $(kA)^t = k A^t$

(3) 행렬의 곱에 대한 성질

① $A ,~ B \in M_{m ,~ p}$이고 $C \in M_{p ,~ n}$이면 $(A \pm B) C = AC \pm BC$ (분배법칙)

② $A \in M_{m ,~ p} ,~ B \in M_{p ,~ q}$이고, $C \in M_{q ,~ n}$이면 $(AB) C = A(BC)$ (결합법칙)

③ $A \in M_{m ,~ p} ,~ B \in M_{p ,~ n}$이면 $(AB)^t = B^t A^t$ (곱의 전치)

(4) 주의해야 할 행렬의 곱의 성질

다음 명제들은 성립하지 않는다. 

① $A^2 = O$이면 $A = O$이다. ⇒ 거짓

② $AB = O$이면 $A = O$ 또는 $B = O$이다. ⇒ 거짓

③ $A (B + C) = O$이면 $A = O$ 또는 $B + C = O$이다. ⇒ 거짓

④ $AC = BC$이면 $A = B$ 또는 $C = O$이다. ⇒ 거짓

⑤ $AB = AC$이고, $A \not = O$이면 $B = C$이다. ⇒ 거짓



