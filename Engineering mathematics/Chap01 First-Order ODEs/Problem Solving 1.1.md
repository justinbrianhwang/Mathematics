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
    
    ↔ $y = \int \cosh (5.13x) dx$
    
    $= \frac{1}{5.13} \sinh (5.13x) + C$
    
    ⇒ $y= \frac{1}{5.13} \sinh (5.13x) + C$
    
8. $y''' = e^{-0.2x}$
    
    ↔ $y'' = -5 e^{0.2x} + C_1$ 
    
    ↔ $y' = 25e^{0.2x} + C_1 x + C_2$ 
    
    ↔ $y = -125 e^{0.2x} + \frac{1}{2} C_1 x^2 + C_2 x + C_3$ 
    
    ⇒ $y = -125 e^{-0.2x} + Cx^2 + C^* x + C^{**}$

9. Differential Equation Solution Verification and Initial Value Problem

    Given Differential Equation
    $y' + 4y = 1.4$

    Proposed Solution
    $y = ce^{-4x} + 0.35$

    Verification
    First, let's verify if the proposed solution satisfies the differential equation

    Given:
    $y = ce^{-4x} + 0.35$

    Taking the derivative of $y$:
    $y' = -4ce^{-4x}$

    Now, substitute $y$ and $y'$ back into the differential equation $y' + 4y$
    $y' + 4y = -4ce^{-4x} + 4(ce^{-4x} + 0.35)$
    $y' + 4y = -4ce^{-4x} + 4ce^{-4x} + 1.4$
    $y' + 4y = 1.4$

    Thus, the proposed solution satisfies the differential equation.

    Initial Value Problem (IVP)
    Given the initial condition $y(0) = 2$, we can find the constant $c$

    $y(0) = 2$
    $2 = c \cdot 1 + 0.35$
    $2 = c + 0.35$
    $c = 1.65$

    Final Solution
    Therefore, the solution to the IVP is:
    $y = 1.65e^{-4x} + 0.35$

    ![function1.1.9](https://i.imgur.com/kkO33Zb.png)
    
    
10. Differential Equation Solution Verification and Initial Value Problem

    Given Differential Equation
    $y' + 5xy = 0$

    Proposed Solution
    $y = ce^{-2.5x^2}$

    Verification
    First, let's verify if the proposed solution satisfies the differential equation:

    Given:
    $y = ce^{-2.5x^2}$

    Taking the derivative of $y$:
    $y' = -5x c e^{-2.5x^2}$

    Now, substitute $y$ and $y'$ back into the differential equation $y' + 5xy$:
    $y' + 5xy = -5x ce^{-2.5x^2} + 5x ce^{-2.5x^2}$
    $y' + 5xy = -5x ce^{-2.5x^2} + 5x ce^{-2.5x^2} = 0$

    Thus, the proposed solution satisfies the differential equation.

    Initial Value Problem (IVP)
    Given the initial condition $y(0) = \pi$, we can find the constant $c$:

    $y(0) = \pi$
    $\pi = c \cdot 1$
    $c = \pi$

    Final Solution
    Therefore, the solution to the IVP is:
    $y = \pi e^{-2.5x^2}$

    ![function1.1.10](https://i.imgur.com/ObCMYJV.png)
    
    

11. Differential Equation Solution Verification and Initial Value Problem

    Given Differential Equation
    $y' = y+e^{x}$

    Proposed Solution
    $y = (x+c) e^x$

    Verification
    First, let's verify if the proposed solution satisfies the differential equation:

    Given:
    $y = (x+c) e^x$

    Taking the derivative of $y$:
    $y' = e^x + (x+c)e^x = e^x (x+c + 1)$

    Now, substitute $y$ and $y'$ back into the differential equation $y + e^x$:
    $y + e^x = (x+c)e^x + e^x = e^x (x+c+ 1)$

    Thus, the proposed solution satisfies the differential equation.

    Initial Value Problem (IVP)
    Given the initial condition $y(0) = \frac{1}{2}$, we can find the constant $c$:

    $y(0) = \frac{1}{2}$
    $\frac{1}{2} = c \cdot 1$
    $c = \frac{1}{2}$

    Final Solution
    Therefore, the solution to the IVP is:
    $y = (x + \frac{1}{2})e^x$

    ![function1.1.11](https://i.imgur.com/FsFLGSm.png)

12. Differential Equation Solution Verification and Initial Value Problem

    Given Differential Equation
    $yy' = 4x$

    Proposed Solution
    $y^2 - 4x^2 = c$  ($y > 0$)

    Verification
    First, let's verify if the proposed solution satisfies the differential equation:

    Given:
    $y^2 = 4x^2 + c$

    Taking the derivative of $y^2$:
    $(y^2)' = (4x^2 + c)'$

    This results in:
    $2yy' = 8x$

    Simplifying, we get:
    $yy' = 4x$

    Thus, the proposed solution satisfies the differential equation.

    Initial Value Problem (IVP)
    Given the initial condition $y(1) = 4$, we can find the constant $c$:

    Substitute $x = 1$ and $y = 4$ into the proposed solution:
    $4^2 = 4 \cdot 1^2 + c$
    $16 = 4 + c$
    $c = 12$

    Final Solution
    Therefore, the solution to the IVP is:
    $y^2 - 4x^2 = 12$

    ![function1.1.12](https://i.imgur.com/1VRUJjW.png)
    

14. Differential Equation Solution Verification and Initial Value Problem

    Given Differential Equation
    $y' = y - y^2$

    Proposed Solution
    $y = \frac{1}{1 + ce^{-x}}$

    Verification
    First, let's verify if the proposed solution satisfies the differential equation:

    Given:
    $y = \frac{1}{1 + ce^{-x}}$

    Taking the derivative of $y$:
    $y' = \frac{-1 \cdot (-ce^{-x})}{(1 + ce^{-x})^2} = \frac{ce^{-x}}{(1 + ce^{-x})^2}$

    Now, substitute $y$ and $y'$ back into the differential equation $y' = y - y^2$:
    $y - y^2 = \frac{1}{1 + ce^{-x}} - \left(\frac{1}{1 + ce^{-x}}\right)^2 = \frac{1}{1 + ce^{-x}} - \frac{1}{(1 + ce^{-x})^2} = \frac{ce^{-x}}{(1 + ce^{-x})^2}$

    Thus, the proposed solution satisfies the differential equation.

    Initial Value Problem (IVP)
    Given the initial condition $y(0) = 0.25$, we can find the constant $c$:

    Substitute $x = 0$ and $y = 0.25$ into the proposed solution:
    $\frac{1}{1 + c} = 0.25$
    $1 + c = 4$
    $c = 3$

    Final Solution
    Therefore, the solution to the IVP is:
    $y = \frac{1}{1 + 3e^{-x}}$

15. Differential Equation Solution Verification and Initial Value Problem

    Given Differential Equation
    $y' \tan x = 2y - 8$

    Proposed Solution
    $y = c \sin^2 x + 4$

    Verification
    First, let's verify if the proposed solution satisfies the differential equation:

    Given:
    $y = c \sin^2 x + 4$

    Taking the derivative of $y$:
    $y' = 2c \sin x \cos x$

    Now, substitute $y$ and $y'$ back into the differential equation $y' \tan x = 2y - 8$:
    $y' \tan x = 2c \sin x \cos x \cdot \frac{\sin x}{\cos x} = 2c \sin^2 x$

    For the right-hand side:
    $2y - 8 = 2(c \sin^2 x + 4) - 8 = 2c \sin^2 x + 8 - 8 = 2c \sin^2 x$

    Thus, the proposed solution satisfies the differential equation.

    Initial Value Problem (IVP)
    Given the initial condition $y\left(\frac{1}{2} \pi\right) = 0$, we can find the constant $c$:

    Substitute $x = \frac{1}{2} \pi$ and $y = 0$ into the proposed solution:
    $0 = c \sin^2 \left(\frac{1}{2} \pi\right) + 4$
    $0 = c \cdot 1 + 4$
    $c = -4$

    Final Solution
    Therefore, the solution to the IVP is:
    $y = -4\sin^2 x + 4$


