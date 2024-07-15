[in English]

# Laplace Transform

There is a reason I didn't explain much in the previous chapters. This is because once we deal with the Laplace transform, the previous concepts might seem less significant due to the powerful nature of the Laplace transform.

First, before dealing with the Laplace transform, we need to think fundamentally. Have we ever predicted the form of the roots and solved the problem in mathematics before? For instance, consider the equation:

$$ y'' + ay' + by = r $$

When we see this equation, we know it takes the form of $e^{\lambda x}$. By substituting this form, we solved the characteristic equation. Is this the same way we've been solving problems? Not exactly. We used a specific method to neatly find the answer, but this method involved prediction.

The Laplace transform, however, solves without prediction. So, what method is this? Let's look into it.

But before we delve into it, let's establish a few basic premises:

1. We live in a world where 'time' is fundamental. Most physical equations are fundamentally based on time. Therefore, we will use the variable $t$ to represent time, instead of the mathematical variable $x$.
2. The basic idea of the Laplace transform is to change dimensions. Laplace Transform: $t \rightarrow s$ Inverse Laplace Transform: $s \rightarrow t$ It is an interaction between the time dimension $t$ of our world and the dimension $s$ which has no particular meaning.
3. The formula for the Laplace transform is as follows:

$$
\mathcal{L} \{ f(t) \} = \int_{0}^{\infty} e^{-st} f(t) \, dt
$$

4. You must memorize the transform forms of famous functions. The forms are as follows:

    |              $t$ |               $s$ |
    | ---------------- | ----------------- |
    |            $e^{at}$ |              $\frac{1}{s - a}$ |
    |             $1$ |                 $\frac{1}{s}$ |
    |              $t$ |               $\frac{1}{s^2}$ |
    |             $t^2$ |                $\frac{2}{s^3}$ |
    |              $t^n$ |             $\frac{n!}{s^{n+1}}$ |
    |        $\sin (kt)$ |           $\frac{k}{k^2 + s^2}$ |
    |        $\cos (kt)$ |           $\frac{s}{s^2 + k^2}$ |
    |        $\sinh (kt)$ |          $\frac{k}{s^2 - k^2}$ |
    |        $\cosh (kt)$ |          $\frac{s}{s^2 - k^2}$ |

5. The Laplace transform is linear. This is possible because it is defined as an integral. Let's see the following:

$$
\mathcal{L}\{ af(t) + bg(t)\} = a \mathcal{L} \{ f(t)\} + b \mathcal{L} \{ g(t) \} = a F(s) + b G(s)
$$

These five principles are essential. We will use them to organize more advanced concepts.

## The 1st Push Method

This is a name I came up with. If you think about the meaning of the word "push," it implies to push out. Consider the following concept.

$$ e^{ax} \sin x $$

It would be very complicated to calculate the Laplace transform of the above product function using the formula. It would involve integration by parts, which can be tedious. If you master the method I introduce and use it appropriately, it will be helpful.

$$ \mathcal{L} \{ e^{ax} f(t) \} $$

In cases where it is arranged in this form, it can be simplified as follows:

$$ \mathcal{L} \{e^{ax} f(x)\} = F(s-a) $$

This is an obvious logic, but you may not have thought of it. I will not prove this method separately. Just remember the concept of "pushing out." We will apply this method in problem-solving later.

## The 2nd Push Method

This method uses the unit step function. Let's first look at the concept of the unit step function.

$$
u(t) = \begin{cases} 
0 & (t < 0) \\ 
1 & (t \geq 0) 
\end{cases}
$$

The shifted form is as follows:

$$
u(t-a) = \begin{cases} 
0 & (t < a) \\ 
1 & (t \geq a) 
\end{cases}
$$

The Laplace transforms of these functions are:

$$
\mathcal{L} \{ u(t) \} = \frac{1}{s}, \quad \mathcal{L} \{ u(t-a) \} = \frac{e^{-as}}{s}
$$

Using this function, the 2nd Push Method is applied as follows:

$$
\mathcal{L} \{ f(t-a)u(t-a) \} = e^{-as} F(s)
$$

## Laplace Transform of Functions

Now we will transform functions using the Laplace transform. Let's look at the following:

$$
\mathcal{L} \{ f(t) \} = \int_{0}^{\infty} e^{-st} f(t) \, dt = F(s)
$$

Now consider

$$
\mathcal{L} \{ f'(t) \} = \int_{0}^{\infty} e^{-st} f'(t) \, dt
$$

What happens here? This can be proved using integration by parts. Skipping the proof, the result is as follows:

$$
\mathcal{L} \{ f'(t) \} = sF(s) - f(0)
$$

This formula can be derived through integration by parts. Generalizing this gives us:

$$
\mathcal{L} \{ f^{(n)}(t) \} = s^{n}F(s) - s^{n-1}f(0) - s^{n-2} f'(0) - \cdots - sf^{(n-1)} (0) - f^{(n-1)}(0)
$$

Using these methods, we can solve problems. It is essential to see the process of solving problems, as just understanding the concepts is not enough.


[in korean]

# 라플라스 변환

내가 앞 챕터에서 많은 설명을 하지 않은 이유가 있다. 그 이유가 바로 라플라스 변환을 다루게 되면, 앞의 내용들이 큰 의미가 없어질 수 있을 정도로 강력한 개념이기 때문이다.

먼저, 라플라스 변환을 다루기 전, 기본적인 생각을 해야 한다. 우리가 그동안 풀어왔던 수학에서 과연 근의 형태를 예측하고 문제를 풀어왔던 경험이 있었는가? 예를 들어 이런 것이다.

$y'' + ay' +by = r$ 이라는 식을 봤을 때, 형태가 $e^{\lambda x}$ 꼴이니, 이를 대입하여 특성 방정식을 풀었다. 이는 과연 우리가 풀어오던 방식과 동일한가? 그렇지 않다. 우리는 특정한 방법을 이용하여 답을 깔끔하게 구하였으나 이 풀이는 예측을 했다는 것이다.

라플라스 변환은 예측이 아닌 풀이를 하는 것이다. 그렇다면 어떤 방법인지 살펴보아야 한다.

하지만 살피기 전, 몇 가지 기본 전제를 깔아두고 시작하자.

1. 우리가 사는 세계는 ‘시간’을 기본적인 것으로 삼고 살아간다. 대부분의 물리적 방정식들의 기본적인 단위는 시간이다. 그렇기에 수학에서 사용하던 $x$라는 변수를 앞으로는 $t$라는 시간을 의미하는 변수들로 사용할 것이다.
2. 라플라스 변환의 기본 적인 생각은 차원을 바꾸는 것이다.
   라플라스 변환: $t \rightarrow s$
   라플라스 역변환: $s \rightarrow t$
   우리가 살고 있는 세계인 시간차원 $t$와 아무런 의미가 없는 차원 $s$간의 상호작용이다.
3. 라플라스 변환의 공식은 다음과 같다.

$$
\mathcal{L} \{ f(t) \} = \int_{0}^{\infty} e^{-st} f(t) \, dt
$$

4. 유명한 함수들의 변환꼴은 전부 암기해야 한다. 변환꼴은 다음과 같다.

    |              $t$ |               $s$ |
    | ---------------- | ----------------- |
    |            $e^{at}$ |              $\frac{1}{s - a}$ |
    |             $1$ |                 $\frac{1}{s}$ |
    |              $t$ |               $\frac{1}{s^2}$ |
    |             $t^2$ |                $\frac{2}{s^3}$ |
    |              $t^n$ |             $\frac{n!}{s^{n+1}}$ |
    |        $\sin (kt)$ |           $\frac{k}{k^2 + s^2}$ |
    |        $\cos (kt)$ |           $\frac{s}{s^2 + k^2}$ |
    |        $\sinh (kt)$ |          $\frac{k}{s^2 - k^2}$ |
    |        $\cosh (kt)$ |          $\frac{s}{s^2 - k^2}$ |

5. 라플라스 변환은 선형성이 성립한다. 라플라스 변환은 적분으로 정의된 식이므로 가능한 것이다. 다음을 보자.

$$
\mathcal{L}\{ af(t) + bg(t)\} = a \mathcal{L} \{ f(t)\} + b \mathcal{L} \{ g(t) \} = a F(s) + b G(s)
$$

다음과 같은 5가지를 알아야만 한다. 이를 이용하여 심화 개념을 정리해볼 것이다.

## The 1st Push method

이는 내가 지어낸 이름이다. push라는 단어의 의미를 잘 생각해보면 밀어낸다라는 의미를 지닌다. 이 개념을 생각해서 다음 개념을 보자.

$e^{ax} \sin x$

위의 곱함수를 라플라스 변환시켜보자. 공식을 이용해서 계산하고자 하면 매우 복잡할 것이다. 항이 2개로 정리가 되겠으나, 부분 적분을 이용하여 정리해야 하는데 이는 귀찮음을 유발할 것이다. 내가 소개하는 방법을 잘 익혀두고 적절히 잘 써먹으면 좋을 것 같다.

$\mathcal{L} \{ e^{ax} f(t) \}$

와 같은 꼴로 정리가 되는 경우, 다음과 같이 정리 된다.

$\mathcal{L} \{e^{ax} f(x)\} = F(s-a)$

사실 당연한 논리이지만 생각하지 못했을 수도 있다. 이 방법에 대한 증명은 따로 하지 않을 것이다. 그냥 이런 개념이 있으니 “밀어낸다”라는 개념을 잘 떠올리면 될 것 같다. 이에 대한 적용은 따로 문제 풀이에서 진행할 것이다. 그때 익히자.

## The 2nd Push method

이는 단위 계단 함수를 이용할 것이다. 단위 계단 함수라는 개념을 먼저 살펴보자.

$$
u(t) = \begin{cases} 0 & (t < 0) \\ 1 & (t \geq 0) \end{cases}
$$

로 정의한다. 평행이동한 꼴은 다음과 같다.

$$
u(t-a) = \begin{cases} 0 & (t < a) \\ 1 & (t \geq a) \end{cases}
$$

이를 각각 라플라스 변환시키면 다음과 같다.

$$
\mathcal{L} \{ u(t) \} = \frac{1}{s}, \quad \mathcal{L} \{ u(t-a) \} = \frac{e^{-as}}{s}
$$

이 함수를 이용해서 제2 Push method를 사용하면 다음과 같다.

$$
\mathcal{L} \{ f(t-a)u(t-a) \} = e^{-as} F(s)
$$

## 함수의 라플라스 변환

이제 본격적으로 함수를 라플라스 변환시킬 것이다. 다음을 보자.

$$
\mathcal{L} \{ f(t) \} = \int_{0}^{\infty} e^{-st} f(t) \, dt = F(s)
$$

로 정의됨은 이제 알 것이다. 그렇다면

$$
\mathcal{L} \{ f'(t) \} = \int_{0}^{\infty} e^{-st} f'(t) \, dt
$$

는 어떻게 될까? 이는 부분 적분을 이용하여 증명할 수 있다. 증명은 과감히 생략하고, 결론만 보면 다음과 같다.

$$
\mathcal{L} \{ f'(t) \} = sF(s) - f(0)
$$

이와 같은 공식은 부분 적분을 통해 증명할 수 있다. 이를 이용하여 일반화 시키면 다음과 같다.

$$
\mathcal{L} \{ f^{(n)}(t) \} = s^{n}F(s) - s^{n-1}f(0) - s^{n-2} f'(0) - \cdots - sf^{(n-1)} (0) - f^{(n-1)}(0)
$$

이와 같은 방법들을 이용하여 문제를 풀어나가면 된다. 개념만 보면 문제를 풀 수 없으니 반드시 문제를 푸는 과정을 보자.

