[In English]


[In korean]
# 완전(exact) 미분 방정식 구하기

in. 전미분 꼴! 

변수 2개로 이루어진 함수인 $u(x,~y)$를 생각해보자. 이때, 함수 $u$의 전미분은 다음과 같이 정의된다. 

$$
du(x,~y) = \frac{\partial u }{\partial x}dx + \frac{\partial u }{\partial y}dy
$$

다음과 같은 **전미분식**의 일부를 함수로 표현해보자. $M(x,~ y) = \frac{\partial u}{\partial x}$라 하고,  $N(x,~ y) = \frac{\partial u}{\partial y}$라 하자. 이때, $M$과 $N$모두 $u$함수를 각각 $x,~y$로 편미분한 식이므로 각각을 다시 $y, ~x$로 편미분하게 되면 다음과 같은 등식이 성립하게 된다. 

$$
\frac{\partial M}{\partial y} = \frac{\partial N}{\partial x}
$$

즉 다음과 같은 식이 성립하면 완전 미분 방정식이라 하며, 원래 식은 $u$를 구하기 위해서는 $M, ~N$을 각각 역으로 적분하여 두 식이 같다는 논리로 풀이하면 된다. 

## integrating factor

$$
\frac{\partial M}{\partial y} \not= \frac{\partial N}{\partial x}
$$

위와 같은 식으로 나올 수도 있는 것이다. 이럴 때 풀이는 어떻게 해야 할까? 소제목에서 언급한 integrating factor라는 개념에 대해 볼 것이다. 위의 등식이 같아지도록 만드는 임의의 함수 $F$를 생각해보자. 해당 함수는 원래 $F(x,~y)$이지만, 편의를 위해 앞으로는 $x$로만 이루어진 함수로 생각할 것이다. $y$로 생각해도 다를 것은 없다. 기본 원리를 생각하기 위해 $x$를 생각한 것이고, 문제를 풀다가 식이 복잡해지면 $y$로 고쳐 풀어도 좋다. 

$F(x)$로 상정했으니, $y$로 미분하게 된다면 $0$이 된다는 것은 너무나 자명한 사실이다. 이를 이용해서 각각을 편미분하는 식에 $F$를 넣어 정리하면 다음과 같은 식이 나온다.

$$
\frac{\partial}{\partial y}(MF) = \frac{\partial}{\partial x} (NF)
$$

위에서 적분 요소의 개념이 등식을 같도록 만들어주는 요소이니, 다음과 같이 등식이 성립하게 됨을 알 수 있다. 이를 이용해서 식을 정리해보자. 

$$
M_y F + MF_y = N_x F + NF_x
$$

위에서 언급한 대로 $F$를 $y$로 미분하면 $0$이 됨을 보였으니 $MF_y = 0$이다. 위의 식을 좀 더 정리하자.

$$
M_y F = N_x F + NF_x
$$

위의 식을 각각 $F, ~x$로 식을 넘겨주자.

$$
(M_y-N_x) F = NF_x 
$$

$$
(M_y - N_x)/N = \frac{1}{F} \cdot F_x
$$

$$
\ln(F) = 정리된 식
$$

즉, $F$에 대한 식을 다음과 같은 과정을 통해 구해줄 수 있으며, 해당 식을 곱해주어 쉽게 식을 구할 수 있게 된다.

⇒ 이 방법은 전미분의 형태로 문제가 주어졌을 때, 풀이하는 방식이다. 

---

$$
y' + p(x) y = r(x) 
$$

## Linear ODEs인 경우
### Homogeneous ODEs인 경우

위의 식에서 $r(x)$가 $0$인 경우를 Homogeneous하다고 한다. 이때 $y(x)$를 쉽게 구하는 방법이 있다. 다음과 같이 구하면 된다.

$$
y(x) = ce^{ - h}, ~ h(x) = \int p(x) dx
$$

### Nonhomogeneous ODEs인 경우

위의 식에서 $r(x)$가 $0$이 아닌 경우를 Nonhomogeneous하다고 한다. 이때 $y(x)$를 쉽게 구하는 방법이 있다. 다음과 같이 구하면 된다. 

$$
y(x) = e^{-h} \left( \int e^{h}r dx + c \right) , ~h(x) = \int p(x) dx
$$

## Non-Linear ODEs인 경우

베르누이 방법을 사용하자. 예를 들어 위의 식에서 일부를 변형해서 보자. 

$$
y' + p(x) y = r(x) y^a
$$

여기서 $a$가 $1$이거나 $0$이면 위에서 다룬 방식이다. 그 외적으로는 전부 linear하지 않은 ODEs이다. 여기서 $j = [y]^{1-a}$로 두면 된다. 이후 $j'$를 구한뒤 위의 $y$들로 표현된 식들을 전부 $j$로 표현 된 식으로 정리하면 된다. 베르누이 방법을 사용하면 Non-Linear ODEs도 Linear하게 바꿀 수 있게 된다. 즉 이렇게 변경하여 위의 식들을 이용해서 구하면 된다.
