








# Differential Equations Solutions

3. $y' + ky = e^{-kx}$
    
    $y' +py = r$의 형태이다. 
    
    $y = e^{-h} \{ \int e^h r dx + c \}$ 가 위의 일차 미분방정식의 기본꼴이다. 
    
    이때, $h$는 $h = \int p   dx$로 정의된다. 
    
    $h = kx$
    
    $y = e^{-kx} \{ \int e^{kx} e^{-kx} dx + c \} = e^{-kx} \{ \int 1   dx + c \}$ 
    
    $y = (x + c) e^{-kx}$
    
    ∴ $y = (x + c) e^{-kx}$

4. $y' + 2y = 4 \cos 2x$, $y\left(\frac{\pi}{4}\right) = 3$
    
    $y' +py = r$의 형태이다. 
    
    $y = e^{-h} \{ \int e^h r dx + c \}$ 가 위의 일차 미분방정식의 기본꼴이다. 
    
    이때, $h$는 $h = \int p   dx$로 정의된다. 
    
    $h = 2x$
    
    $y = e^{-2x} \{ \int 4 e^{2x} \cos 2x   dx + c \}$ 
    
    $\int 4e^{2x} \cos 2x   dx = 2e^{2x} \cos 2x + \int 4 e^{2x} \sin 2x   dx$
    
    $= 2e^{2x} \cos 2x + 2e^{2x} \sin 2x - \int 4e^{2x} \cos 2x   dx$
    
    $\int 4e^{2x} \cos 2x   dx = e^{2x} (\cos 2x + \sin 2x)$
    
    $y = e^{-2x} \{ e^{2x} (\cos 2x + \sin 2x) + c \}$
    
    ∴ $y = \cos 2x + \sin 2x + ce^{-2x}$이며, IVP이므로 대입하여 $c$를 구하면 $c = 2 e^{\frac{\pi}{2}}$이다. 이를 대입하면
    
    ∴ $y = \cos 2x + \sin 2x + 2e^{\frac{\pi}{2}} e^{-2x}$

5. $xy' = 2y + x^3 e^x$
    
    $xy' - 2y = x^3 e^x$
    
    $y' - \frac{2}{x} y = x^2 e^x$
    
    $y' + py = r$의 형태이다. 
    
    $y = e^{-h} \{ \int e^h r   dx + c \}$ 가 위의 일차 미분방정식의 기본꼴이다. 
    
    이때, $h$는 $h = \int p   dx$로 정의된다. 
    
    $h = -2 \ln x$
    
    $y = x^2 \{ \int \frac{1}{x^2} x^2 e^x   dx + c \}$
    
    $= x^2 \{ \int e^x   dx + c \}$
    
    $= x^2 e^x + cx^2$
    
    ∴ $y = x^2 e^x + cx^2$

6. $y' + y \tan x = e^{-0.01x} \cos x$, $y(0) = 0$
    
    $y' + py = r$의 형태이다. 
    
    $y = e^{-h} \{ \int e^h r   dx + c \}$ 가 위의 일차 미분방정식의 기본꼴이다. 
    
    이때, $h$는 $h = \int p   dx$로 정의된다. 
    
    $h = - \ln |\cos x|$
    
    $y = \cos x \{ \int \frac{1}{\cos x} e^{-0.01x} \cos x   dx + c \}$
    
    $= \cos x \{ \int e^{-0.01x}   dx + c \}$
    
    $= \cos x \{ -100 e^{-0.01x} + c \}$
    
    IVP 이므로 $y(0) = 0$을 대입하면, $c = 100$이다.
    
    ∴ $y = \cos x \{ -100 e^{-0.01x} + 100 \}$

7. $y' + y \sin x = e^{\cos x}$, $y(0) = -2.5$
    
    $y' + py = r$의 형태이다. 
    
    $y = e^{-h} \{ \int e^h r   dx + c \}$ 가 위의 일차 미분방정식의 기본꼴이다. 
    
    이때, $h$는 $h = \int p   dx$로 정의된다. 
    
    $h = - \cos x$
    
    $y= e^{\cos x} \{ \int e^{-\cos x} e^{\cos x}   dx + c \}$
    
    $= e^{\cos x} \{ \int   dx + c \}$
    
    $= (x + c) e^{\cos x}$
    
    IVP 이므로, $y(0) = -2.5$ 대입
    
    $c = 2.5$
    
    $y = (x + 2.5) e^{\cos x}$
    
    ∴ $y = (x + 2.5) e^{\cos x}$

8. $y' \cos x + (3y - 1) \sec x = 0$
    
    $y' + (3y - 1) \sec x = 0$
    
    $y' + 3 \sec x y = \sec x$
    
    $y' + py = r$의 형태이다. 
    
    $y = e^{-h} \{ \int e^h r   dx + c \}$ 가 위의 일차 미분방정식의 기본꼴이다. 
    
    이때, $h$는 $h = \int p   dx$로 정의된다. 
    
    $h = \tan x$
    
    $y = e^{-\tan x} \{ e^{\tan x} \sec^2 x   dx + c \}$
    
    $y = e^{-\tan x} \{ e^{\tan x} + c \}$
    
    $y = c e^{-\tan x} + 1$
    
    IVP 이므로, $c$를 구하면, $c = \frac{e}{3}$
    
    ∴ $y = \frac{e}{3} e^{-\tan x} + 1$

9. $y' = (y - 2) \cot x$
    
    $y' - \cot x y = -2 \cot x$
    
    $y' + py = r$의 형태이다. 
    
    $y = e^{-h} \{ \int e^h r   dx + c \}$ 가 위의 일차 미분방정식의 기본꼴이다. 
    
    이때, $h$는 $h = \int p   dx$로 정의된다. 
    
    $h = - \ln |\sin x|$
    
    $y = \sin x \{ \int \frac{-2 \cos x}{\sin^2 x}   dx + c \}$
    
    $\sin x = t$로 치환
    
    $\cos x   dx = dt$
    
    $\int \frac{-2}{t^2}   dt = \frac{2}{t}$
    
    ∴ $y = \sin x \left( \frac{2}{\sin x} + c \right)$
    
    $y = 2 + c \sin x$
    
    ∴ $y = c \sin x + 2$

10. $xy' + 4y = 8x^4$, $y(1) = 2$
    
    $y' + \frac{4}{x} y = 8x^3$
    
    $y' + py = r$의 형태이다. 
    
    $y = e^{-h} \{ \int e^h r   dx + c \}$ 가 위의 일차 미분방정식의 기본꼴이다. 
    
    이때, $h$는 $h = \int p   dx$로 정의된다. 
    
    $h = 4 \ln x$
    
    $y = x^{-4} \{ \int 8x^7   dx + c \}$
    
    $y = x^{-4} \{ x^8 + c \}$
    
    ∴ $y = x^4 + cx^{-4}$

11. $y' = 6(y - 2.5) \tanh \left(\frac{3}{2} x\right)$
    
    이 문제의 경우는 공식을 이용한 풀이를 사용해도 괜찮으나, 손으로 풀기엔 많이 복잡한 모습을 보였다. 이를 훨씬 수월하게 해결하기 위해 separable 방법을 사용할 것이다.
    
    $\frac{1}{y - 2.5} y' = 6 \tanh \left(\frac{3}{2} x\right)$
    
    $\ln | y - 2.5 | = 4 \ln |\cosh \left(\frac{3}{2} x\right) | + c$
    
    $y - 2.5 = c \cosh^4 \left(\frac{3}{2} x\right)$
    
    ∴ $y = c \cosh^4 \left(\frac{3}{2} x\right) + 2.5$

