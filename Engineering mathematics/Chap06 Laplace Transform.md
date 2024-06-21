[in korean]

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Laplace Transform</title>
    <script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
    <script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            line-height: 1.6;
            margin: 20px;
        }
        h1, h2, h3 {
            font-family: 'Georgia', serif;
        }
        table {
            width: 100%;
            border-collapse: collapse;
        }
        table, th, td {
            border: 1px solid black;
        }
        th, td {
            padding: 8px;
            text-align: center;
        }
    </style>
</head>
<body>

# 라플라스 변환

내가 앞 챕터에서 많은 설명을 하지 않은 이유가 있다. 그 이유가 바로 라플라스 변환을 다루게 되면, 앞의 내용들이 큰 의미가 없어질 수 있을 정도로 강력한 개념이기 때문이다.

먼저, 라플라스 변환을 다루기 전, 기본적인 생각을 해야 한다. 우리가 그동안 풀어왔던 수학에서 과연 근의 형태를 예측하고 문제를 풀어왔던 경험이 있었는가? 예를 들어 이런 것이다.

\( y'' + ay' + by = r \)이라는 식을 봤을 때, 형태가 \( e^{\lambda x} \) 꼴이니, 이를 대입하여 특성 방정식을 풀었다. 이는 과연 우리가 풀어오던 방식과 동일한가? 그렇지 않다. 우리는 특정한 방법을 이용하여 답을 깔끔하게 구하였으나 이 풀이는 예측을 했다는 것이다.

라플라스 변환은 예측이 아닌 풀이를 하는 것이다. 그렇다면 어떤 방법인지 살펴보아야 한다.

하지만 살피기 전, 몇 가지 기본 전제를 깔아두고 시작하자.

1. 우리가 사는 세계는 ‘시간’을 기본적인 것으로 삼고 살아간다. 대부분의 물리적 방정식들의 기본적인 단위는 시간이다. 그렇기에 수학에서 사용하던 \( x \)라는 변수를 앞으로는 \( t \)라는 시간을 의미하는 변수들로 사용할 것이다.
2. 라플라스 변환의 기본 적인 생각은 차원을 바꾸는 것이다.
   라플라스 변환: \( t \rightarrow s \)
   라플라스 역변환: \( s \rightarrow t \)
   우리가 살고 있는 세계인 시간차원 \( t \)와 아무런 의미가 없는 차원 \( s \)간의 상호작용이다.
3. 라플라스 변환의 공식은 다음과 같다.

    \[
    \mathcal{L} \{ f(t) \} = \int_{0}^{\infty} e^{-st} f(t) \, dt
    \]

4. 유명한 함수들의 변환꼴은 전부 암기해야 한다. 변환꼴은 다음과 같다.

    |              \( t \) |               \( s \) |
    | --- | --- |
    |            \( e^{at} \) |              \( \frac{1}{s - a} \) |
    |             \( 1 \) |                 \( \frac{1}{s} \) |
    |              \( t \) |               \( \frac{1}{s^2} \) |
    |             \( t^2 \) |                \( \frac{2}{s^3} \) |
    |              \( t^n \) |             \( \frac{n!}{s^{n+1}} \) |
    |        \( \sin (kt) \) |           \( \frac{k}{k^2 + s^2} \) |
    |        \( \cos (kt) \) |           \( \frac{s}{s^2 + k^2} \) |
    |        \( \sinh (kt) \) |          \( \frac{k}{s^2 - k^2} \) |
    |        \( \cosh (kt) \) |          \( \frac{s}{s^2 - k^2} \) |

5. 라플라스 변환은 선형성이 성립한다. 라플라스 변환은 적분으로 정의된 식이므로 가능한 것이다. 다음을 보자.

    \[
    \mathcal{L}\{ af(t) + bg(t)\} = a \mathcal{L} \{ f(t)\} + b \mathcal{L} \{ g(t) \} = a F(s) + b G(s)
    \]

다음과 같은 5가지를 알아야만 한다. 이를 이용하여 심화 개념을 정리해볼 것이다.

## The 1st Push method

이는 내가 지어낸 이름이다. push라는 단어의 의미를 잘 생각해보면 밀어낸다라는 의미를 지닌다. 이 개념을 생각해서 다음 개념을 보자.

\( e^{ax} \sin x \)

위의 곱함수를 라플라스 변환시켜보자. 공식을 이용해서 계산하고자 하면 매우 복잡할 것이다. 항이 2개로 정리가 되겠으나, 부분 적분을 이용하여 정리해야 하는데 이는 귀찮음을 유발할 것이다. 내가 소개하는 방법을 잘 익혀두고 적절히 잘 써먹으면 좋을 것 같다.

\( \mathcal{L} \{ e^{ax} f(t) \} \)

와 같은 꼴로 정리가 되는 경우, 다음과 같이 정리 된다.

\( \mathcal{L} \{e^{ax} f(x)\} = F(s-a) \)

사실 당연한 논리이지만 생각하지 못했을 수도 있다. 이 방법에 대한 증명은 따로 하지 않을 것이다. 그냥 이런 개념이 있으니 “밀어낸다”라는 개념을 잘 떠올리면 될 것 같다. 이에 대한 적용은 따로 문제 풀이에서 진행할 것이다. 그때 익히자.

## The 2nd Push method

이는 단위 계단 함수를 이용할 것이다. 단위 계단 함수라는 개념을 먼저 살펴보자.

\( u(t) = \begin{cases} 0 & (t < 0) \\ 1 & (t \geq 0) \end{cases} \)

로 정의한다. 평행이동한 꼴은 다음과 같다.

\( u(t-a) = \begin{cases} 0 & (t < a) \\ 1 & (t \geq a) \end{cases} \)

이를 각각 라플라스 변환시키면 다음과 같다.

\( \mathcal{L} \{ u(t) \} = \frac{1}{s}, \quad \mathcal{L} \{ u(t-a) \} = \frac{e^{-as}}{s} \)

이 함수를 이용해서 제2 Push method를 사용하면 다음과 같다.

\( \mathcal{L} \{ f(t-a)u(t-a) \} = e^{-as} F(s) \)

## 함수의 라플라스 변환

이제 본격적으로 함수를 라플라스 변환시킬 것이다. 다음을 보자.

\( \mathcal{L} \{ f(t) \} = \int_{0}^{\infty} e^{-st} f(t) \, dt = F(s) \)

로 정의됨은 이제 알 것이다. 그렇다면

\( \mathcal{L} \{ f'(t) \} = \int_{0}^{\infty} e^{-st} f'(t) \, dt \)

는 어떻게 될까? 이는 부분 적분을 이용하여 증명할 수 있다. 증명은 과감히 생략

