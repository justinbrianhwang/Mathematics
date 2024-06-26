# Differential Equations Solutions

1. $2xy   dx + x^2   dy = 0$
    
    Let $M(x, y) = 2xy$ and $N(x, y) = x^2$.
    
    $M_y = 2x$,  $N_x = 2x$
    
    Therefore, $M_y = N_x$ holds, making it an exact equation!
    
    $\int M(x, y)   dx + c(y) = \int N(x, y)   dy + c(x) = c^*$
    
    $x^2 y + c(y) = x^2y + c(x) = c^*$
    
    $x^2 y = c$
    
    Hence, $y = \frac{c}{x^2}$.

2. $x^3   dx + y^3   dy = 0$
    
    Let $M(x, y) = x^3$ and $N(x, y) = y^3$.
    
    $M_y (x, y) = 0$, $N_x (x, y) = 0$, so $M_y = N_x$ holds, making it an exact equation!
    
    $\int M(x, y)   dx + c(y) = \int N(x, y)   dy + c(x) = c^*$
    
    $\frac{1}{4} x^4 + c(y) = \frac{1}{4} y^4 + c(x) = c^*$
    
    Therefore, $x^4 + y^4 = c$.

3. $\sin x \cos y   dx + \cos x \sin y   dy = 0$
    
    Let $M(x, y) = \sin x \cos y$ and $N(x, y) = \cos x \sin y$.
    
    $M_y = \sin x (- \sin y )$, $N_x = -\sin x \sin y$, so $M_y = N_x$ holds, making it an exact equation!
    
    $\int M(x, y)   dx + c(y) = \int N(x, y)   dy + c(x) = c^*$
    
    $-\cos x \cos y + c(y) = -\cos x \cos y + c(x) = c^*$
    
    Therefore, $\cos x \cos y = c$.

4. $e^{3 \theta} (dr + 3r d\theta) = 0$
    
    $e^{3 \theta} dr + 3re^{3 \theta} d\theta = 0$
    
    Therefore, let $M(\theta, r) = e^{3\theta}$ and $N(\theta, r) = 3r e^{3 \theta}$.
    
    $M_{\theta} = 3e^{3 \theta}$, $N_{r} = 3e^{3 \theta}$, so $M_{\theta} = N_r$ holds, making it an exact equation!
    
    $\int M(\theta, r)   dr + c(\theta) = \int N(\theta, r)   d\theta + c(r) = c^*$
    
    $e^{3 \theta} r + c(\theta) = e^{3 \theta} r + c(r) = c^*$
    
    Therefore, $r = c e^{-3\theta}$.

5. $(x^2 + y^2)   dx - 2xy   dy = 0$
    
    Let $M(x, y) = x^2 + y^2$ and $N(x, y) = -2xy$.
    
    $M_y = 2y$, $N_x = -2y$, so $M_y \neq N_x$; thus, an integrating factor is needed. Let the integrating factor be $J(x)$. Since $J$ is the integrating factor, the following holds:
    
    $\frac{\partial}{\partial y} (MJ) = \frac{\partial}{\partial x} (NJ)$
    
    Simplifying the equation:
    
    $M_y J + MJ_y = N_x J + NJ_x$
    
    Solving for $J$:
    
    $2y J + (x^2 + y^2) \times 0 = (-2y)J + (-2xy) J'$
    
    $4y J = -2xyJ'$
    
    $- \frac{2}{x} = \frac{1}{J} J'$
    
    $-\frac{2}{x}   dx = \frac{1}{J}   dJ$
    
    $\int -\frac{2}{x}   dx = \int \frac{1}{J}   dJ$
    
    $-2 \ln x = \ln J$
    
    $J = \frac{1}{x^2}$
    
    Multiplying by the integrating factor and solving:
    
    $MJ = 1 + \left(\frac{y}{x}\right)^2$
    
    $NJ = -2 \frac{y}{x}$
    
    $\int MJ   dx + c(y) = \int NJ   dy + c(x) = c^*$
    
    $x - \frac{y^2}{x} + c(y) = -\frac{y^2}{x} + c(x) = c^*$
    
    $x - \frac{y^2}{x} = c$
    
    $x^2 - y^2 = cx$
    
    $y^2 = x^2 + cx$
    
    Therefore, $y = \sqrt{x^2 + cx}$.

6. $3(y+1)   dx = 2x   dy$
    
    $3(y+1)   dx - 2x   dy = 0$
    
    Let $M(x, y) = 3y+3$ and $N(x, y) = -2x$.
    
    $M_y = 3$, $N_x = -2$, so $M_y \neq N_x$; an integrating factor is needed.
    
    Solving for $J$:
    
    $3J + (3y + 3) \times 0 = -2J + (-2x) J'$
    
    $5J = -2xJ'$
    
    $-\frac{5}{2} \frac{1}{x} = \frac{1}{J} J'$
    
    $-\frac{5}{2} \frac{1}{x}   dx = \frac{1}{J}   dJ$
    
    $\int -\frac{5}{2} \frac{1}{x}   dx = \int \frac{1}{J}   dJ$
    
    $-\frac{5}{2} \ln x = \ln J$
    
    $J = x^{-\frac{5}{2}}$
    
    Solving the equation:
    
    $\int MJ   dx + c(y) = \int NJ   dy + c(x) = c^*$
    
    $3(y+1) \int x^{-\frac{5}{2}}   dx + c(y) = -2 x^{-\frac{3}{2}} \int   dy + c(x) = c^*$
    
    $-2 (y+1) x^{-\frac{3}{2}} = c$
    
    $y + 1 = c x^{\frac{3}{2}}$
    
    Therefore, $y = cx^{\frac{3}{2}} - 1$.

7. $2x \tan y   dx + \sec^2 y   dy = 0$
    
    Let $M = 2x \tan y$ and $N = \sec^2 y$.
    
    $M_y = 2x \sec^2 y$, $N_x = 0$, so $M_y \neq N_x$; an integrating factor is needed.
    
    Solving for $J$:
    
    $(2x \sec^2 y) J + (x^2 \sec^2 y) \times 0 = 0 \times J + \sec^2 J'$
    
    $J = e^{x^2}$
    
    Therefore, $\tan y \times e^{x^2} = c$.

8. $e^x (\cos y   dx - \sin y   dy) = 0$
    
    Let $M = e^x \cos y$ and $N = -e^x \sin y$.
    
    Since $M_y = N_x$, it is an exact equation.
    
    $\int M(x, y)   dx + c(y) = \int N(x, y)   dy + c(x) = c^*$
    
    Therefore, $e^x \cos y = c$.

9. $e^{2x} (2 \cos y   dx - \sin y   dy) = 0, \quad y(0) = 0$
    
    $2e^{2x} \cos y   dx - e^{2x} \sin y   dy = 0$
    
    Let $M = 2e^{2x} \cos y$ and $N = -e^{2x} \sin y$.
    
    $M_y = -2e^{2x} \sin y$, $N_x = -2e^{2x} \sin y$, so $M_y = N_x$ holds.
    
    $\int M(x, y)   dx + c(y) = \int N(x, y)   dy + c(x) = c^*$
    
    $\cos y \int 2e^{2x}   dx + c(y) = e^x \int \sin y   dy + c(x) = c^*$
    
    Therefore, $e^{2x} \cos y = c$.
    
    Given $y(0) = 0$:
    
    $c = 1$
    
    Therefore, $e^{2x} \cos y = 1$.

10. $y   dx + [y + \tan(x+y)]   dy = 0$
    
    Given the integrating factor $J = \cos(x+y)$:
    
    Let $M = y$ and $N = y + \tan(x+y)$.
    
    $MJ = y\cos(x+y)$, $NJ = y\cos(x+y) + \sin(x+y)$.
    
    $y \int \cos(x+y)   dx + c(y) = \int y \cos(x+y)   dy + \int \sin(x+y)   dy + c(x) = c$
    
    Therefore, $y \sin(x+y) + \cos(x+y) = c$.

11. $2 \cosh x \cos y   dx = \sinh x \sin y   dy$
    
    $2 \cosh x \cos y   dx - \sinh x \sin y   dy = 0$
    
    Let $M(x, y) = 2 \cosh x \cos y$ and $N(x, y) = -\sinh x \sin y$.
    
    $M_y = -2 \cosh x \sin y$
    
    $N_x = - \cosh x \sin y$
    
    Since $M_y \neq N_x$, an integrating factor $J$ is needed.
    
    Solving for $J$:
    
    $\coth x = \frac{1}{J} J'$
    
    $\coth x   dx = \frac{1}{J}   dJ$
    
    Therefore, $J = \sinh x$.
    
    $MJ = 2 \cosh x \sinh x \cos y$
    
    $NJ = -\sinh^2 x \sin y$
    
    $\int M(x, y)J(x)   dx + c(y) = \int N(x, y)J(x)   dy + c(x) = c^*$
    
    Therefore, $\sinh^2 x \cos y = c$.

12. $(2xy   dx + dy) e^{x^2} = 0$, $y(0) = 2$
    
    $2x e^{x^2} y   dx + e^{x^2}   dy = 0$
    
    Let $M = 2x e^{x^2} y$ and $N = e^{x^2}$.
    
    $M_y = 2x e^{x^2}$, $N_x = 2xe^{x^2}$, so $M_y = N_x$ holds, making it an exact equation.
    
    $\int M(x, y)   dx + c(y) = \int N(x, y)   dy + c(x) = c^*$
    
    Therefore, $e^{x^2} y = c$
    
    Given $y(0) = 2$:
    
    $1 \times 2 = c$
    
    Therefore, $y = 2 e^{-x^2}$.

13. $e^{-y}   dx + e^{-x} (-e^{-y} + 1)   dy = 0$, $F = e^{x+y}$
    
    Given the integrating factor $F = e^{x+y}$:
    
    $e^x   dx + e^y (-e^{-y} + 1)   dy = 0$
    
    $\int e^x   dx + c(y) = \int e^y (-e^{-y} + 1)   dy + c(x) = c^*$
    
    Therefore, $e^x + e^y - y = c$.

14. $(a+1)y + (b+1)x   dy = 0$, $y(1) = 1$, $F = x^a y^b$
    
    Given the integrating factor $F = x^a y^b$:
    
    $(a + 1) x^a y^{b+1} + (b + 1) x^{a+ 1} y^b   dy = 0$
    
    Therefore, $x^{a+1} y^{b+1} = 1$.
