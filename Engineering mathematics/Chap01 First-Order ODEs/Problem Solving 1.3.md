# Kreyszig P8. Problem Set 1.3


2. $y^3 y' + x^3 = 0$
    
    ↔ $y^3 \frac{dy}{dx} = -x^3$
    
    ↔ $y^3 dy = -x^3 dx$
    
    ↔ $\int y^3 dy = \int -x^3 dx$
    
    ↔ $\frac{1}{4} y^4 + c_1 = -\frac{1}{4} x^4 + c_2$
    
    ↔ $\frac{1}{4} y^4 + \frac{1}{4} x^4 = c_3$
    
    ⇒ $x^4 + y^4 = c$
    
3. $y' = \sec^2 y$
    
    ↔ $\frac{dy}{dx} = \frac{1}{\cos^2 y}$
    
    ↔ $\cos^2 y dy = dx$
    
    ↔ $\int \cos^2 y dy = \int dx$
    
    ∴ $\cos 2y = 2\cos^2 y - 1$
    
    $\cos^2 y = \frac{\cos 2y + 1}{2}$
    
    ↔ $\int \frac{1}{2} \cos 2y + \frac{1}{2} dy = \int dx$
    
    ⇒ $\frac{1}{4} \sin 2y + \frac{1}{2}y = x + c$
    
4. $y' \sin 2 \pi x = \pi y \cos 2 \pi x$
    
    ↔ $\frac{dy}{dx} = \pi y \cot 2 \pi x$
    
    ↔ $\frac{1}{y} dy = \pi \cot 2 \pi x dx$
    
    ↔ $\ln y = \frac{1}{2} (-\csc^2 (2 \pi x)) + c$
    
    ⇒ $y = c e^{\frac{1}{2} (-\csc^2 (2\pi x))}$
    
5. $yy' + 36x = 0$
    
    ↔ $y \frac{dy}{dx} = -36x$
    
    ↔ $y dy = -36x dx$
    
    ↔ $\frac{1}{2} y^2 = -18 x^2 + c$
    
    ↔ $y^2 = -36x^2 + c$
    
    ⇒ $36x^2 + y^2 = c$
    
6. $y' = e^{2x-1} y^2$
    
    ↔ $\frac{dy}{dx} = e^{2x-1} y^2$
    
    ↔ $\frac{1}{y^2} dy = e^{2x-1} dx$
    
    ↔ $\int \frac{1}{y^2} dy = \int e^{2x-1} dx$
    
    ↔ $-\frac{1}{y} = \frac{1}{2} e^{2x-1} + c$
    
    ↔ $y = \frac{1}{-\frac{1}{2} e^{2x-1} + c}$
    
    ⇒ $y = \frac{1}{c - \frac{1}{2} e^{2x-1}}$
    
7. $xy' = y + 2x^3 \sin^2 \frac{y}{x}$
    
    ↔ $y' = \frac{y}{x} + 2x^2 \sin^2 \frac{y}{x}$
    
    ∴ $\frac{y}{x} = u$ 치환
    
    $y = ux$
    
    $y' = u'x + u$
    
    ↔ $u'x + u = u + 2x^2 \sin^2 u$
    
    ↔ $u'x = 2x^2 \sin^2 u$
    
    ↔ $u' = 2x \sin^2 u$
    
    ↔ $\csc^2 u du = 2x dx$
    
    ↔ $\int \csc^2 u du = \int 2x dx$
    
    ↔ $-\cot u = x^2 + c$
    
    ↔ $\cot u = -x^2 + c$
    
    ↔ $u = \cot^{-1} (-x^2 + c)$
    
    ↔ $\frac{y}{x} = \cot^{-1} (-x^2 + c)$
    
    ⇒ $y = x \cot^{-1} (-x^2 + c)$
    
8. $y' = (y + 4x)^2$
    
    ∴ $y + 4x = u$로 치환
    
    $y' + 4 = u'$
    
    $y' = u' - 4$
    
    ↔ $u' - 4 = u^2$
    
    ↔ $u' = u^2 + 4$
    
    ↔ $\frac{u'}{u^2 + 4} = 1$
    
    ↔ $\frac{1}{u^2 + 4} du = dx$
    
    ↔ $\int \frac{1}{u^2 + 4} du = \int dx$
    
    ↔ $\int \frac{1}{(\frac{u}{2})^2 + 1} du = \int 4 dx$
    
    ↔ $2 \tan^{-1} (\frac{u}{2}) = 4x + c$
    
    ↔ $\frac{u}{2} = \tan (2x + c)$
    
    ↔ $u = 2 \tan (2x + c)$
    
    $u = y + 4x$ 이므로,
    
    $y = -4x + 2 \tan (2x + c)$
    
9. $xy' = y^2 + y$
    
    $y' = \frac{y}{x} y + \frac{y}{x}$
    
    ∴ $\frac{y}{x} = u$로 치환
    
    $y = ux$
    
    $y' = u'x + u$
    
    ↔ $u + u'x = u(ux) + u$
    
    ↔ $u'x = u^2 x$
    
    ↔ $u' = u^2$
    
    ↔ $\frac{1}{u^2} du = dx$
    
    ↔ $\int \frac{1}{u^2} du = \int dx$
    
    ↔ $-\frac{1}{u} = c + x$
    
    ↔ $u = \frac{1}{c - x}$
    
    ∴ $u = \frac{y}{x}$이므로
    
    ↔ $\frac{y}{x} = \frac{1}{c - x}$
    
    ⇒ $y = \frac{x}{c - x}$
    
10. $xy' = x + y$
    
    ↔ $y' = 1 + \frac{y}{x}$
    
    ∴ $\frac{y}{x} = u$로 치환
    
    $y = ux$
    
    $y' = u + u'x$
    
    ↔ $u'x + u = 1 + u$
    
    ↔ $u'x = 1$
    
    ↔ $du = \frac{1}{x} dx$
    
    ↔ $\int du = \int \frac{1}{x} dx$
    
    ↔ $u = \ln x + c$
    
    ↔ $\frac{y}{x} = \ln x + c$
    
    ⇒ $y = x \ln x + cx$

