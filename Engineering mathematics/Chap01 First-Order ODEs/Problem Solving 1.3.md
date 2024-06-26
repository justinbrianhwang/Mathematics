# Kreyszig P18. Problem Set 1.3

2. 
    $y^3 y' + x^3 = 0$
    
    $\leftrightarrow y^3 \frac{dy}{dx} = -x^3$
    
    $\leftrightarrow y^3 dy = -x^3 dx$
    
    $\leftrightarrow \int y^3 dy = \int -x^3 dx$
    
    $\leftrightarrow \frac{1}{4} y^4 + c_1 = -\frac{1}{4} x^4 + c_2$
    
    $\leftrightarrow \frac{1}{4} y^4 + \frac{1}{4} x^4 = c_3$
    
    $\Rightarrow x^4 + y^4 = c$

3. 
    $y' = \sec^2 y$
    
    $\leftrightarrow \frac{dy}{dx} = \frac{1}{\cos^2 y}$
    
    $\leftrightarrow \cos^2 y \, dy = dx$
    
    $\leftrightarrow \int \cos^2 y \, dy = \int dx$
    
    ∴ $\cos 2y = 2\cos^2 y - 1$
    
    $\cos^2 y = \frac{\cos 2y + 1}{2}$
    
    $\leftrightarrow \int \frac{1}{2} \cos 2y + \frac{1}{2} dy = \int dx$
    
    $\Rightarrow \frac{1}{4} \sin 2y + \frac{1}{2} y = x + c$

4. 
    $y' \sin 2 \pi x = \pi y \cos 2 \pi x$
    
    $\leftrightarrow \frac{dy}{dx} = \pi y \cot 2 \pi x$
    
    $\leftrightarrow \frac{1}{y} dy = \pi \cot 2 \pi x dx$
    
    $\leftrightarrow \ln y = \frac{1}{2} (-\csc^2 (2 \pi x)) + c$
    
    $\Rightarrow y = c e^{\frac{1}{2} (-\csc^2 (2\pi x))}$

5. 
    $yy' + 36x = 0$
    
    $\leftrightarrow y \frac{dy}{dx} = -36x$
    
    $\leftrightarrow y dy = -36x dx$
    
    $\leftrightarrow \frac{1}{2} y^2 = -18 x^2 + c$
    
    $\leftrightarrow y^2 = -36x^2 + c$
    
    $\Rightarrow 36x^2 + y^2 = c$

6. 
    $y' = e^{2x-1} y^2$
    
    $\leftrightarrow \frac{dy}{dx} = e^{2x-1} y^2$
    
    $\leftrightarrow \frac{1}{y^2} dy = e^{2x-1} dx$
    
    $\leftrightarrow \int \frac{1}{y^2} dy = \int e^{2x-1} dx$
    
    $\leftrightarrow -\frac{1}{y} = \frac{1}{2} e^{2x-1} + c$
    
    $\leftrightarrow y = \frac{1}{-\frac{1}{2} e^{2x-1} + c}$
    
    $\Rightarrow y = \frac{1}{c - \frac{1}{2} e^{2x-1}}$

7. 
    $xy' = y + 2x^3 \sin^2 \frac{y}{x}$
    
    $\leftrightarrow y' = \frac{y}{x} + 2x^2 \sin^2 \frac{y}{x}$
    
    ∴ $\frac{y}{x} = u$ substitution
    
    $y = ux$
    
    $y' = u'x + u$
    
    $\leftrightarrow u'x + u = u + 2x^2 \sin^2 u$
    
    $\leftrightarrow u'x = 2x^2 \sin^2 u$
    
    $\leftrightarrow u' = 2x \sin^2 u$
    
    $\leftrightarrow \csc^2 u du = 2x dx$
    
    $\leftrightarrow \int \csc^2 u du = \int 2x dx$
    
    $\leftrightarrow -\cot u = x^2 + c$
    
    $\leftrightarrow \cot u = -x^2 + c$
    
    $\leftrightarrow u = \cot^{-1} (-x^2 + c)$
    
    $\leftrightarrow \frac{y}{x} = \cot^{-1} (-x^2 + c)$
    
    $\Rightarrow y = x \cot^{-1} (-x^2 + c)$

8. 
    $y' = (y + 4x)^2$
    
    ∴ $y + 4x = u$ substitution
    
    $y' + 4 = u'$
    
    $y' = u' - 4$
    
    $\leftrightarrow u' - 4 = u^2$
    
    $\leftrightarrow u' = u^2 + 4$
    
    $\leftrightarrow \frac{u'}{u^2 + 4} = 1$
    
    $\leftrightarrow \frac{1}{u^2 + 4} du = dx$
    
    $\leftrightarrow \int \frac{1}{u^2 + 4} du = \int dx$
    
    $\leftrightarrow \int \frac{1}{(\frac{u}{2})^2 + 1} du = \int 4 dx$
    
    $\leftrightarrow 2 \tan^{-1} (\frac{u}{2}) = 4x + c$
    
    $\leftrightarrow \frac{u}{2} = \tan (2x + c)$
    
    $\leftrightarrow u = 2 \tan (2x + c)$
    
    $u = y + 4x$, therefore,
    
    $y = -4x + 2 \tan (2x + c)$

9. 
    $xy' = y^2 + y$
    
    $y' = \frac{y}{x} y + \frac{y}{x}$
    
    ∴ $\frac{y}{x} = u$ substitution
    
    $y = ux$
    
    $y' = u'x + u$
    
    $\leftrightarrow u + u'x = u(ux) + u$
    
    $\leftrightarrow u'x = u^2 x$
    
    $\leftrightarrow u' = u^2$
    
    $\leftrightarrow \frac{1}{u^2} du = dx$
    
    $\leftrightarrow \int \frac{1}{u^2} du = \int dx$
    
    $\leftrightarrow -\frac{1}{u} = c + x$
    
    $\leftrightarrow u = \frac{1}{c - x}$
    
    ∴ $u = \frac{y}{x}$, therefore,
    
    $\leftrightarrow \frac{y}{x} = \frac{1}{c - x}$
    
    $\Rightarrow y = \frac{x}{c - x}$

10. 
    $xy' = x + y$
    
    $\leftrightarrow y' = 1 + \frac{y}{x}$
    
    ∴ $\frac{y}{x} = u$ substitution
    
    $y = ux$
    
    $y' = u + u'x$
    
    $\leftrightarrow u'x + u = 1 + u$
    
    $\leftrightarrow u'x = 1$
    
    $\leftrightarrow du = \frac{1}{x} dx$
    
    $\leftrightarrow \int du = \int \frac{1}{x} dx$
    
    $\leftrightarrow u = \ln x + c$
    
    $\leftrightarrow \frac{y}{x} = \ln x + c$
    
    $\Rightarrow y = x \ln x + cx$


11. $x y' + y = 0$, $y(4) = 6$

    $x y' = -y$

    $y' = -\frac{y}{x}$

    $\frac{1}{y} \, dy = - \frac{1}{x} \, dx$

    $\int \frac{1}{y} \, dy = - \int \frac{1}{x} \, dx$

    $\ln y = -\ln x + c$

    $y = e^{-\ln x} \times e^c$

    $y = c \times \frac{1}{x}$

    $y = \frac{c}{x}$

    $6 = \frac{c}{4}$

    $c = 24$

    $y = \frac{24}{x}$


