# In English

1. $y' - y = 5.2$
    
    This is in the form $y' + py = r$.
    
    The general solution for this first-order differential equation is:
    
    $y = e^{-h} \left( \int e^h r   dx + c \right)$
    
    Here, $h$ is defined as $h = \int p   dx$.
    
    $h = -x$
    
    $y = e^{x} \left( \int e^{-x} (5.2)   dx + c \right)$
    
    $y = e^x \left( -5.2e^{-x} + c \right)$
    
    $y = c e^x - 5.2$
    
    Hence, $y = ce^x - 5.2$.

2. $y' = 2y - 4x$
    
    This is in the form $y' + py = r$.
    
    The general solution for this first-order differential equation is:
    
    $y = e^{-h} \left( \int e^h r   dx + c \right)$
    
    Here, $h$ is defined as $h = \int p   dx$.
    
    $h = -2x$
    
    $y = e^{2x} \left( \int e^{-2x} (4x)   dx + c \right)$
    
    $y = e^{2x} \left( 2x e^{-2x} + c \right)$
    
    $y = ce^{2x} + 2x$
    
    Hence, $y = ce^{2x} + 2x$.

3. $y' + ky = e^{-kx}$
    
    This is in the form $y' + py = r$.
    
    The general solution for this first-order differential equation is:
    
    $y = e^{-h} \left( \int e^h r   dx + c \right)$
    
    Here, $h$ is defined as $h = \int p   dx$.
    
    $h = kx$
    
    $y = e^{-kx} \left( \int e^{kx} e^{-kx}   dx + c \right) = e^{-kx} \left( \int 1   dx + c \right)$
    
    $y = (x + c)e^{-kx}$
    
    Hence, $y = (x + c)e^{-kx}$.

4. $y' + 2y = 4 \cos 2x$, $y\left(\frac{\pi}{4}\right) = 3$
    
    This is in the form $y' + py = r$.
    
    The general solution for this first-order differential equation is:
    
    $y = e^{-h} \left( \int e^h r   dx + c \right)$
    
    Here, $h$ is defined as $h = \int p   dx$.
    
    $h = 2x$
    
    $y = e^{-2x} \left( \int 4 e^{2x} \cos 2x   dx + c \right)$
    
    $\int 4e^{2x} \cos 2x   dx = 2e^{2x} \cos 2x + \int 4 e^{2x} \sin 2x   dx$
    
    $= 2e^{2x} \cos 2x + 2e^{2x} \sin 2x - \int 4e^{2x} \cos 2x   dx$
    
    $\int 4e^{2x} \cos 2x   dx = e^{2x} (\cos 2x + \sin 2x)$
    
    $y = e^{-2x} \left( e^{2x} (\cos 2x + \sin 2x) + c \right)$
    
    Hence, $y = \cos 2x + \sin 2x + ce^{-2x}$. Since this is an IVP, substitute the given initial condition to find $c$:
    
    $3 = \cos\left(2 \cdot \frac{\pi}{4}\right) + \sin\left(2 \cdot \frac{\pi}{4}\right) + c e^{-2 \cdot \frac{\pi}{4}}$
    
    $3 = \cos\left(\frac{\pi}{2}\right) + \sin\left(\frac{\pi}{2}\right) + c e^{-\frac{\pi}{2}}$
    
    $3 = 0 + 1 + c e^{-\frac{\pi}{2}}$
    
    $c = 2 e^{\frac{\pi}{2}}$
    
    Substituting $c$ back, we get:
    
    Hence, $y = \cos 2x + \sin 2x + 2e^{\frac{\pi}{2}} e^{-2x}$.

5. $xy' = 2y + x^3 e^x$
    
    $xy' - 2y = x^3 e^x$
    
    $y' - \frac{2}{x} y = x^2 e^x$
    
    This is in the form $y' + py = r$.
    
    The general solution for this first-order differential equation is:
    
    $y = e^{-h} \left( \int e^h r   dx + c \right)$
    
    Here, $h$ is defined as $h = \int p   dx$.
    
    $h = -2 \ln x$
    
    $y = x^2 \left( \int \frac{1}{x^2} x^2 e^x   dx + c \right)$
    
    $= x^2 \left( \int e^x   dx + c \right)$
    
    $= x^2 e^x + cx^2$
    
    Hence, $y = x^2 e^x + cx^2$.

6. $y' + \tan x y = e^{-0.01x} \cos x$, $y(0) = 0$
    
    This is in the form $y' + py = r$.
    
    The general solution for this first-order differential equation is:
    
    $y = e^{-h} \left( \int e^h r   dx + c \right)$
    
    Here, $h$ is defined as $h = \int p   dx$.
    
    $h = - \ln |\cos x|$
    
    $y = \cos x \left( \int \frac{1}{\cos x} e^{-0.01x} \cos x   dx + c \right)$
    
    $= \cos x \left( \int e^{-0.01x}   dx + c \right)$
    
    $= \cos x \left( -100 e^{-0.01x} + c \right)$
    
    Since this is an IVP, substitute the given initial condition to find $c$:
    
    $0 = \cos(0) \left( -100 e^{-0.01 \cdot 0} + c \right)$
    
    $0 = 1 \left( -100 + c \right)$
    
    $c = 100$
    
    Hence, $y = \cos x \left( -100 e^{-0.01x} + 100 \right)$.

7. $y' + y \sin x = e^{\cos x}$, $y(0) = -2.5$
    
    This is in the form $y' + py = r$.
    
    The general solution for this first-order differential equation is:
    
    $y = e^{-h} \left( \int e^h r   dx + c \right)$
    
    Here, $h$ is defined as $h = \int p   dx$.
    
    $h = - \cos x$
    
    $y = e^{\cos x} \left( \int e^{-\cos x} e^{\cos x}   dx + c \right)$
    
    $= e^{\cos x} \left( \int   dx + c \right)$
    
    $= (x + c) e^{\cos x}$
    
    Since this is an IVP, substitute the given initial condition to find $c$:
    
    $-2.5 = (0 + c) e^{\cos 0}$
    
    $-2.5 = c e^1$
    
    $c = -2.5/e$
    
    Hence, $y = (x - \frac{2.5}{e}) e^{\cos x}$.

8. $y' \cos x + (3y - 1) \sec x = 0$
    
    $y' + (3y - 1) \sec x = 0$
    
    $y' + 3 \sec x y = \sec x$
    
    This is in the form $y' + py = r$.
    
    The general solution for this first-order differential equation is:
    
    $y = e^{-h} \left( \int e^h r   dx + c \right)$
    
    Here, $h$ is defined as $h = \int p   dx$.
    
    $h = \tan x$
    
    $y = e^{-\tan x} \left( \int e^{\tan x} \sec x   dx + c \right)$
    
    $y = e^{-\tan x} \left( \int e^{\tan x}   dx + c \right)$
    
    $y = c e^{-\tan x} + 1$
    
    Since this is an IVP, substitute the given initial condition to find $c$:
    
    Hence, $c = \frac{e}{3}$
    
    Therefore, $y = \frac{e}{3} e^{-\tan x} + 1$.

9. $y' = (y - 2) \cot x$
    
    $y' - \cot x y = -2 \cot x$
    
    This is in the form $y' + py = r$.
    
    The general solution for this first-order differential equation is:
    
    $y = e^{-h} \left( \int e^h r   dx + c \right)$
    
    Here, $h$ is defined as $h = \int p   dx$.
    
    $h = - \ln |\sin x|$
    
    $y = \sin x \left( \int \frac{-2 \cos x}{\sin^2 x}   dx + c \right)$
    
    Let $\sin x = t$ for substitution:
    
    $\cos x   dx = dt$
    
    $\int \frac{-2}{t^2}   dt = \frac{2}{t}$
    
    Hence, $y = \sin x \left( \frac{2}{\sin x} + c \right)$
    
    $y = 2 + c \sin x$
    
    Therefore, $y = c \sin x + 2$.

10. $xy' + 4y = 8x^4$, $y(1) = 2$
    
    $y' + \frac{4}{x} y = 8x^3$
    
    This is in the form $y' + py = r$.
    
    The general solution for this first-order differential equation is:
    
    $y = e^{-h} \left( \int e^h r   dx + c \right)$
    
    Here, $h$ is defined as $h = \int p   dx$.
    
    $h = 4 \ln x$
    
    $y = x^{-4} \left( \int 8x^7   dx + c \right)$
    
    $y = x^{-4} \left( x^8 + c \right)$
    
    Hence, $y = x^4 + cx^{-4}$.

11. $y' = 6(y - 2.5) \tanh \left(\frac{3}{2} x\right)$

    While it's possible to solve this using the general form solution, it's simpler to use the separable method here:
    
    $\frac{1}{y - 2.5} y' = 6 \tanh \left(\frac{3}{2} x\right)$
    
    $\ln | y - 2.5 | = 4 \ln |\cosh \left(\frac{3}{2} x\right) | + c$
    
    $y - 2.5 = c \cosh^4 \left(\frac{3}{2} x\right)$
    
    Hence, $y = c \cosh^4 \left(\frac{3}{2} x\right) + 2.5$.

12. $y' + y \tan x = e^{-0.01x} \cos x$, $y(0) = 0$
    
    This is in the form $y' + py = r$.
    
    The general solution for this first-order differential equation is:
    
    $y = e^{-h} \left( \int e^h r   dx + c \right)$
    
    Here, $h$ is defined as $h = \int p   dx$.
    
    $h = -\ln | \cos x |$
    
    $y = \cos x \left( \int \frac{1}{\cos x} e^{-0.01x} \cos x   dx + c \right)$
    
    $= \cos x \left( \int e^{-0.01x}   dx + c \right)$
    
    $= \cos x \left( -100 e^{-0.01x} + c \right)$
    
    Since this is an IVP, substitute the given initial condition to find $c$:
    
    $0 = \cos(0) \left( -100 e^{-0.01 \cdot 0} + c \right)$
    
    $0 = 1 \left( -100 + c \right)$
    
    $c = 100$
    
    Hence, $y = \cos x \left( -100 e^{-0.01x} + 100 \right)$.

13. $y' + y \sin x = e^{\cos x}$, $y(0)=-2.5$
    
    This is in the form $y' + py = r$.
    
    The general solution for this first-order differential equation is:
    
    $y = e^{-h} \left( \int e^h r   dx + c \right)$
    
    Here, $h$ is defined as $h = \int p   dx$.
    
    $h = -\cos x$
    
    $y = e^{\cos x} \left( \int e^{-\cos x} e^{\cos x}   dx + c \right)$
    
    $= e^{\cos x} \left( \int   dx + c \right)$
    
    $= (x + c) e^{\cos x}$
    
    Since this is an IVP, substitute the given initial condition to find $c$:
    
    $-2.5 = (0 + c) e^{\cos 0}$
    
    $-2.5 = c e^1$
    
    $c = -2.5/e$
    
    Hence, $y = (x - \frac{2.5}{e}) e^{\cos x}$.





# In korean

1. $y' - y = 5.2$
    
    $y' + py = r$의 형태이다. 
    
    $y = e^{-h} \left\{ \int e^h r   dx + c \right\}$ 가 위의 일차 미분방정식의 기본꼴이다. 
    
    이때, $h$는 $h = \int p   dx$로 정의된다. 
    
    $h = -x$
    
    $y = e^{x} \left\{ \int e^{-x} (5.2)   dx + c \right\}$ 
    
    $y = e^x \left\{-5.2e^{-x} + c \right\}$
    
    $y = c e^x - 5.2$
    
    ∴ $y = ce^x - 5.2$

2. $y' = 2y - 4x$
    
    $y' + py = r$의 형태이다. 
    
    $y = e^{-h} \left\{ \int e^h r   dx + c \right\}$ 가 위의 일차 미분방정식의 기본꼴이다. 
    
    이때, $h$는 $h = \int p   dx$로 정의된다. 
    
    $h = -2x$
    
    $y = e^{2x} \left\{ \int -2e^{-2x} x   dx + c \right\}$
    
    $y = e^{2x} \left\{ c + 2x e^{-2x} + e^{-2x} \right\}$
    
    $y = ce^{2x} + 2x + 1$
    
    ∴ $y = ce^{2x} + 2x + 1$

3. $y' + ky = e^{-kx}$
    
    $y' + py = r$의 형태이다. 
    
    $y = e^{-h} \left\{ \int e^h r   dx + c \right\}$ 가 위의 일차 미분방정식의 기본꼴이다. 
    
    이때, $h$는 $h = \int p   dx$로 정의된다. 
    
    $h = kx$
    
    $y = e^{-kx} \left\{ \int e^{kx} e^{-kx}   dx + c \right\} = e^{-kx} \left\{ \int 1   dx + c \right\}$ 
    
    $y = (x + c)e^{-kx}$
    
    ∴ $y = (x + c)e^{-kx}$

4. $y' + 2y = 4 \cos 2x$, $y\left(\frac{\pi}{4}\right) = 3$
    
    $y' + py = r$의 형태이다. 
    
    $y = e^{-h} \left\{ \int e^h r   dx + c \right\}$ 가 위의 일차 미분방정식의 기본꼴이다. 
    
    이때, $h$는 $h = \int p   dx$로 정의된다. 
    
    $h = 2x$
    
    $y = e^{-2x} \left\{ \int 4 e^{2x} \cos 2x   dx + c \right\}$ 
    
    $\int 4e^{2x} \cos 2x   dx = 2e^{2x} \cos 2x + \int 4 e^{2x} \sin 2x   dx$
    
    $= 2e^{2x} \cos 2x + 2e^{2x} \sin 2x - \int 4e^{2x} \cos 2x   dx$
    
    $\int 4e^{2x} \cos 2x   dx = e^{2x} (\cos 2x + \sin 2x)$
    
    $y = e^{-2x} \left\{ e^{2x} (\cos 2x + \sin 2x) + c \right\}$
    
    ∴ $y = \cos 2x + \sin 2x + ce^{-2x}$이며, IVP이므로 대입하여 $c$를 구하면 $c = 2 e^{\frac{\pi}{2}}$이다. 이를 대입하면
    
    ∴ $y = \cos 2x + \sin 2x + 2e^{\frac{\pi}{2}} e^{-2x}$

5. $xy' = 2y + x^3 e^x$
    
    $xy' - 2y = x^3 e^x$
    
    $y' - \frac{2}{x} y = x^2 e^x$
    
    $y' + py = r$의 형태이다. 
    
    $y = e^{-h} \left\{ \int e^h r   dx + c \right\}$ 가 위의 일차 미분방정식의 기본꼴이다. 
    
    이때, $h$는 $h = \int p   dx$로 정의된다. 
    
    $h = -2 \ln x$
    
    $y = x^2 \left\{ \int \frac{1}{x^2} x^2 e^x   dx + c \right\}$
    
    $= x^2 \left\{ \int e^x   dx + c \right\}$
    
    $= x^2 e^x + cx^2$
    
    ∴ $y = x^2 e^x + cx^2$

6. $y' + \tan x e^{-0.01x} \cos x$, $y(0) = 0$
    
    $y' + \tan x y = e^{-0.01x} \cos x$ 
    
    $y' + py = r$의 형태이다. 
    
    $y = e^{-h} \left\{ \int e^h r   dx + c \right\}$ 가 위의 일차 미분방정식의 기본꼴이다. 
    
    이때, $h$는 $h = \int p   dx$로 정의된다. 
    
    $h = - \ln |\cos x|$
    
    $y = \cos x \left\{ \int \frac{1}{\cos x} e^{-0.01x} \cos x   dx + c \right\}$
    
    $= \cos x \left\{ \int e^{-0.01x}   dx + c \right\}$
    
    $= \cos x \left\{ -100 e^{-0.01x} + c \right\}$
    
    IVP 이므로 $y(0) = 0$을 대입하면, $c = 100$이다.
    
    ∴ $y = \cos x \left\{ -100 e^{-0.01x} + 100 \right\}$

7. $y' + y \sin x = e^{\cos x}$, $y(0) = -2.5$
    
    $y' + py = r$의 형태이다. 
    
    $y = e^{-h} \left\{ \int e^h r   dx + c \right\}$ 가 위의 일차 미분방정식의 기본꼴이다. 
    
    이때, $h$는 $h = \int p   dx$로 정의된다. 
    
    $h = - \cos x$
    
    $y = e^{\cos x} \left\{ \int e^{-\cos x} e^{\cos x}   dx + c \right\}$
    
    $= e^{\cos x} \left\{ \int   dx + c \right\}$
    
    $= (x + c) e^{\cos x}$
    
    IVP 이므로, $y(0) = -2.5$ 대입
    
    $c = 2.5$
    
    $y = (x + 2.5) e^{\cos x}$
    
    ∴ $y = (x + 2.5) e^{\cos x}$

8. $y' \cos x + (3y - 1) \sec x = 0$
    
    $y' + (3y - 1) \sec x = 0$
    
    $y' + 3 \sec x y = \sec x$
    
    $y' + py = r$의 형태이다. 
    
    $y = e^{-h} \left\{ \int e^h r   dx + c \right\}$ 가 위의 일차 미분방정식의 기본꼴이다. 
    
    이때, $h$는 $h = \int p   dx$로 정의된다. 
    
    $h = \tan x$
    
    $y = e^{-\tan x} \left\{ e^{\tan x} \sec^2 x   dx + c \right\}$
    
    $y = e^{-\tan x} \left\{ e^{\tan x} + c \right\}$
    
    $y = c e^{-\tan x} + 1$
    
    IVP 이므로, $c$를 구하면, $c = \frac{e}{3}$
    
    ∴ $y = \frac{e}{3} e^{-\tan x} + 1$

9. $y' = (y - 2) \cot x$
    
    $y' - \cot x y = -2 \cot x$
    
    $y' + py = r$의 형태이다. 
    
    $y = e^{-h} \left\{ \int e^h r   dx + c \right\}$ 가 위의 일차 미분방정식의 기본꼴이다. 
    
    이때, $h$는 $h = \int p   dx$로 정의된다. 
    
    $h = - \ln |\sin x|$
    
    $y = \sin x \left\{ \int \frac{-2 \cos x}{\sin^2 x}   dx + c \right\}$
    
    $\sin x = t$로 치환
    
    $\cos x   dx = dt$
    
    $\int \frac{-2}{t^2}   dt = \frac{2}{t}$
    
    ∴ $y = \sin x \left( \frac{2}{\sin x} + c \right)$
    
    $y = 2 + c \sin x$
    
    ∴ $y = c \sin x + 2$

10. $xy' + 4y = 8x^4$, $y(1) = 2$
    
    $y' + \frac{4}{x} y = 8x^3$
    
    $y' + py = r$의 형태이다. 
    
    $y = e^{-h} \left\{ \int e^h r   dx + c \right\}$ 가 위의 일차 미분방정식의 기본꼴이다. 
    
    이때, $h$는 $h = \int p   dx$로 정의된다. 
    
    $h = 4 \ln x$
    
    $y = x^{-4} \left\{ \int 8x^7   dx + c \right\}$
    
    $y = x^{-4} \left\{ x^8 + c \right\}$
    
    ∴ $y = x^4 + cx^{-4}$

11. $y' = 6(y - 2.5) \tanh \left(\frac{3}{2} x\right)$
    
    이 문제의 경우는 공식을 이용한 풀이를 사용해도 괜찮으나, 손으로 풀기엔 많이 복잡한 모습을 보였다. 이를 훨씬 수월하게 해결하기 위해 separable 방법을 사용할 것이다.
    
    $\frac{1}{y - 2.5} y' = 6 \tanh \left(\frac{3}{2} x\right)$
    
    $\ln | y - 2.5 | = 4 \ln |\cosh \left(\frac{3}{2} x\right) | + c$
    
    $y - 2.5 = c \cosh^4 \left(\frac{3}{2} x\right)$
    
    ∴ $y = c \cosh^4 \left(\frac{3}{2} x\right) + 2.5$

12. $y' + y \tan x = e^{-0.01x} \cos x$, $y(0) = 0$
    
    $y' + py = r$의 형태이다.
    
    $y = e^{-h} \left\{ \int e^h r   dx + c \right\}$ 가 위의 일차 미분방정식의 기본꼴이다.
    
    이때, $h$는 $h = \int p   dx$로 정의된다.
    
    $h = -\ln | \cos x |$
    
    $y = \cos x \left\{ \int \frac{1}{\cos x} e^{-0.01x} \cos x   dx + c \right\}$
    
    $= \cos x \left\{ \int e^{-0.01x}   dx + c \right\}$
    
    $= \cos x \left\{ -100 e^{-0.01x} + c \right\}$
    
    IVP 이므로 $y(0) = 0$을 대입하면, $c = 100$이다.
    
    ∴ $y = \cos x \left\{ -100 e^{-0.01x} + 100 \right\}$

13. $y' + y \sin x = e^{\cos x}$, $y(0)=-2.5$
    
    $y' + py = r$의 형태이다.
    
    $y = e^{-h} \left\{ \int e^h r   dx + c \right\}$ 가 위의 일차 미분방정식의 기본꼴이다.
    
    이때, $h$는 $h = \int p   dx$로 정의된다.
    
    $h = -\cos x$
    
    $y = e^{\cos x} \left\{ \int e^{-\cos x} e^{\cos x}   dx + c \right\}$
    
    $= e^{\cos x} \left\{ \int   dx + c \right\}$
    
    $= (x + c) e^{\cos x}$
    
    IVP 이므로, $y(0) = -2.5$ 대입
    
    $c = 2.5$
    
    $y = (x + 2.5) e^{\cos x}$
    
    ∴ $y = (x + 2.5) e^{\cos x}$



