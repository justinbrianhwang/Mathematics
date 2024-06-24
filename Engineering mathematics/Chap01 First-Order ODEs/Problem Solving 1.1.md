# Kreyszig P8. Problem Set 1.1

1. $y' + 2\sin 2\pi x = 0$
    
    ↔ $y' = -2\sin 2 \pi x$
    
    ↔ $y = -2 \int \sin 2\pi x dx$
    
    ↔ $y = -2 \left[ -\frac{1}{2 \pi} \cos 2 \pi x +C \right]$
    
    ⇒ $y = \frac{1}{\pi} \cos 2 \pi x + C$
    
2. $y' + x e^{-x^2 / 2} = 0$
    
    ↔ $y' = -x e^{-x^2 / 2}$
    
    ↔ $y = - \int x e^{-x^2 / 2}  dx$
    
    ↔ $y = - \left[ -e^{-x^2 / 2} + C \right]$
    
    ⇒ $y = e^{-x^2 / 2} + C$
    
3. $y' = y$
    
    ↔ $\frac{dy}{dx} = y$
    
    ↔ $\frac{1}{y}  dy = dx$
    
    ↔ $\int \frac{1}{y}  dy = \int  dx$
    
    ↔ $\ln |y| = x + C$
    
    ↔ $y = e^{x + C} = e^x \times e^C$
    
    ⇒ $y = C \times e^x$ 
    
4. $y' = -1.5 y$
    
    ↔ $\frac{dy}{dx} = -1.5 y$
    
    ↔ $\frac{1}{y}  dy = -1.5  dx$
    
    ↔ $\ln |y| = -1.5x + C$
    
    ↔ $y = e^{-1.5 x + C}$
    
    ⇒ $y = C e^{-1.5x}$
    
5. $y' = 4e^{-x} \cos x$
    
    ↔ $y = \int 4e^{-x } \cos x  dx$ 
    
    Consider $e^{-x}$ as the part to be integrated and $\cos x$ as the part to be differentiated.
    
    $\int 4 e^{-x} \cos x  dx = 4 \left[ -e^{-x} \cos x - \int -e^{-x} (-\sin x) dx \right]$
    
    ↔ $\int e^{-x} \sin x  dx = -e^{-x} \sin x - \int -e^{-x} \cos x  dx$ 
    
    $= -e^{-x} \sin x + \int e^{-x} \cos x  dx$  
    
    ∴ $4 \int e^{-x} \cos x dx = - 4e^{-x} \cos x -4 \left( -e^{-x} \sin x + \int e^{-x} \cos x dx  \right)$
    
    $-4e^{-x} \cos x + 4e^{-x} \sin x - 4 \int e^{-x} \cos x  dx + C$
    
    ↔ $8 \int e^{-x} \cos x  dx = 4 e^{-x} \left(\sin x  - \cos x\right) + C$
    
    ↔ $4 \int e^{-x} \cos x  dx = 2 e^{-x} \left(\sin x  - \cos x\right) + C$
    
    ⇒  $y = 2e^{-x} \left( \sin x - \cos x \right) + C$
    
6. $y'' = -y$
    
    ↔ $y'' y' = -y y'$
    
    ↔ $y' \frac{dy'}{dx} = -y \frac{dy}{dx}$
    
    ↔ $y'  dy' = - y dy$
    
    ↔ $\frac{1}{2} \left( y^2 + y'^2 \right) = C$
    
    ↔ $y^2 + y'^2 = C$
    
    $y = \sin x$ or $y = \cos x$ forms...
    
    ⇒ $y = C_1 \sin x + C_2 \cos x$
    
7. $y' = \cosh (5.13x)$
    
    ↔ $y = \int \cosh (5.13x) \, dx$
    
    $= \frac{1}{5.13} \sinh (5.13x) + C$
    
    ⇒ $y= \frac{1}{5.13} \sinh (5.13x) + C$
    
8. $y''' = e^{-0.2x}$
    
    ↔ $y'' = -5 e^{0.2x} + C_1$ 
    
    ↔ $y' = 25e^{0.2x} + C_1 x + C_2$ 
    
    ↔ $y = -125 e^{0.2x} + \frac{1}{2} C_1 x^2 + C_2 x + C_3$ 
    
    ⇒ $y = -125 e^{-0.2x} + Cx^2 + C^* x + C^{**}$
