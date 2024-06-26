# Differential Equations Solutions

1. $2xy dx + x^2 dy = 0$
    
    이 때, $M(x, ~y) = 2xy$라 하고, $N(x,~y) = x^2$ 라 하자. 
    
    $M_y = 2x$,  $N_x = 2x$
    
    ∴ $M_y = N_x$ 가 성립하므로 exact equation 풀이가 가능하다! 
    
    $\int M(x, ~y) dx + c(y) = \int N(x, ~y) dy + c(x) = c^*$
    
    $x^2 y + c(y) = x^2y + c(x) = c^*$
    
    $x^2 y = c$
    
    ∴ $y = {c \over x^2 }$이다! 
    

2. $x^3 dx + y^3 dy = 0$
    
    $M(x,~y) = x^3$라 하고, $N(x,~y) = y^3$라 하자. 
    
    $M_y (x, ~y) = 0$, $N_x (x, ~y) = 0$ 이므로, $M_y = N_x$ 가 성립하므로 exact equation 풀이가 가능하다!
    
    $\int M(x,~y) dx + c(y) = \int N(x,~y) dy + c(x)  = c^*$
    
    ${1 \over 4} x^4 + c(y) = {1\over4} y^4 + c(x) = c^*$
    
    ∴ $x^4 + y^4 = c$이다. 
    

3. $\sin x \cos y dx  + \cos x  \sin y dy = 0$
    
    $M(x, ~y) = \sin x \cos y$ 라 하고, $N(x,~y) = \cos x \sin y$라 하자. 
    
    $M_y = \sin x (- \sin y )$, $N_x = -\sin x \sin y$이므로, $M_y = N_x$ 가 성립하므로 exact equation 풀이가 가능하다!
    
    $\int M(x, ~y) dx + c(y) = \int N(x, ~y) dy + c(x) = c^*$
    
    $-\cos x \cos y + c(y) = -\cos x  \cos y + c(x) = c^*$
    
    ∴ $\cos x \cos y = c$이다.
    
4. $e^{3 \theta} (dr + 3r d \theta ) = 0$
    
    $e^{3 \theta} dr + 3re^{3 \theta} d \theta = 0$
    
    ∴ $M(\theta,~r) = e^{3\theta}$라 하고, $N( \theta, r ) = 3r e^{3 \theta}$라 하자. 
    
    $M_{\theta} = 3e^{3 \theta}$, $N_{r} = 3e^{3 \theta}$이므로, $M_{\theta} = N_r$ 가 성립하므로 exact equation 풀이가 가능하다! 
    
    $\int M(\theta,~r) dr + c(\theta) = \int N(\theta, ~r) + c(r) = c^*$
    
    $e^{3 \theta} r + c(\theta) = e^{3 \theta} r + c(r) = c^*$
    
    ∴ $r = c e^{-3\theta}$이다. 
    
5. $(x^2 + y^2 ) dx - 2xy dy = 0$
    
    $M(x,~y) = x^2 + y^2$ 라 하고,  $N(x, ~y) = -2xy$라 하자. 
    
    $M_y = 2y$,  $N_x = -2y$ 이므로, $M_y \not= N_x$이므로, exact equation풀이가 불가능한 상황이다. 이때는 적분 요소가 필요하다. 적분요소를 $J(x)$라 하자. $J$가 적분 요소이므로 다음이 성립한다. 
    
    ${\partial \over \partial y} (MJ) = {\partial \over \partial y} (NJ)$
    
    즉 위의 식을 정리하면 다음과 같다. 
    
    $M_y J  + MJ_y = N_x J + NJ_x$  이다. 이때 $J$를 구해보자. 
    
    $2y J + (x^2 + y^2) \times 0 =  (-2y)J + (-2xy) J'$
    
    $4y J = -2xyJ'$
    
    $- {2\over x} = {1\over J } J'$
    
    $-{2\over x} dx = {1 \over J} dJ$ 
    
    $\int -{2\over x} dx = \int {1 \over J} dJ$ 
    
    $-2 \ln x = \ln J$
    
    $J = {1\over x^2 }$이다. 이제 적분 요소를 곱한 값을 적분해보자. 
    
    $MJ = 1 + ({y \over x})^2$
    
    $NJ = -2 {y \over x}$
    
    $\int MJ dx + c(y) = \int NJ dy + c(x)  = c^*$
    
    $x - {y^2 \over x} + c(y) = -{y^2 \over x} +c(x) = c^*$
    
    $x- {y^2 \over x} = c$
    
    $x^2 - y^2 = cx$
    
    $y^2 = x^2 + cx$ 
    
    ∴ $y = \sqrt{x^2 + cx}$이다. 
    
6. $3(y+1) dx = 2x dy$ 
    
    $3(y+1)dx -2x dy = 0$
    
    $M(x,~y) = 3y+3$라 하고, $N(x,~y) = -2x$라 하자.
    
    $M_y = 3 ,~N_x = -2$이므로 $M_y \not= N_x$이다. 적분 요소가 필요하므로 적분 요소부터 구해보자. 
    
    $3J + (3y + 3) \times 0 = -2J + (-2x) J'$
    
    $5J = -2xJ'$
    
    $-{5\over2} {1\over x}  = {1 \over J} J'$
    
    $-{5\over2} {1\over x} dx  = {1 \over J} dJ$
    
    $\int -{5\over2} {1\over x}  = \int {1 \over J} J'$
    
    $-{5\over2} \ln x = \ln J$
    
    $J = x^{-{5\over2}}$이다. 적분을 해보자. 
    
    $\int MJ dx + c(y) = \int NJ + c(x) = c^*$
    
    $3(y+1) \int x^{- {5\over2}}dx + c(y) = -2 x^{-{3\over2}} \int dy + c(x) = c^*$
    
    $- 2 (y+1 ) x^{- {3\over2}} = c$
    
    $y + 1 = c x^{3\over2}$
    
    ∴ $y = cx^{3\over2} - 1$
    
7. $2x \tan y dx + \sec^2 y dy = 0$
    
    $M  = 2x \tan y$라 하고, $N = \sec^2 y$ 라 하자. 
    
    $M_y = 2x \sec^2 y ,~N_x = 0$이므로 $M_y \not= N_x$ 이므로 적분 요소가 필요하다. 
    
    $(2x \sec^2 y) J + (x^2 \sec^2 y) \times 0 =  0 \times J + \sec^2 J'$
    
    $J = e^{x^2}$이다. 
    
    ∴ $\tan y \times e^{x^2} = c$
    
8. $e^x (\cos y dx - \sin y dy ) = 0$
    
    $M = e^x \cos y$라 하고, $N = -e^x \sin y$라 하자.
    
    $M_y = N_x$ 이므로 exact equation 풀이가 가능하다. 
    
    $\int M(x,~y) dx + c(y) = \int N(x, ~y) + c(x) = c^*$ 
    
    $e^x \cos y = c$
    
9. $e^{2x} (2 \cos y dx - \sin y dy ) = 0, ~~y(0) = 0$ 
    
    $2e^{2x} \cos y dx - e^{2x}\sin y dy =0$
    
    $M = 2e^{2x}\cos y$라 하고, $N = -e^{2x} \sin y$라 하자. 
    
    $M_y = -2e^{2x}\sin y$ 이고, $N_x = -2e^{2x} \sin y$ 이므로 $M_y = N_x$ 가 성립한다. 
    
    $\int M(x,~y) dx + c(y) = \int N(x, ~y) + c(x) = c^*$ 
    
    $\cos y \int 2e^{2x} dx +c(y) = e^x \int \sin y dy + c(x) = c^*$
    
    ∴ $e^{2x} \cos y = c$
    
    $y(0) = 0$
    
    $c = 1$
    
    ∴ $e^{2x} \cos y  =1$
    
# Differential Equations Solutions

10. $y dx + [y + \tan (x+y)]dy = 0$
    
    적분 요소가 주어졌으므로 
    
    $J = \cos(x+y)$를 곱하여 풀어보자. 
    
    $M = y$, $N= y + \tan (x+y)$라 할 때, 
    
    $MJ = y\cos(x+y)$, $NJ = y\cos(x+y) +\sin(x+y)$이다. 
    
    $y \int \cos (x+y) dx +c(y) = \int y \cos (x+y) dy + \int \sin(x+y) dy +c(x) = c$ 
    
    ∴ $y\sin (x+y) + \cos(x+y) = c$

11. $2 \cosh x \cos y dx = \sinh x \sin y dy$
    
    $2 \cosh x \cos y dx - \sinh x \sin y dy = 0$
    
    $M(x,~y) = 2 \cosh x \cos y$
    
    $N(x,~y) = -\sinh x \sin y$
    
    $M_y = -2 \cosh x \sin y$
    
    $N_x = - \cosh x \sin y$
    
    $M_y \not= N_x$이므로 적분요소 $J$가 필요하다.
    
    $\coth x  =  \frac{1}{J} J'$
    
    $\coth x dx = \frac{1}{J} dJ$
    
    ∴ $J = \sinh x$ 이다.
    
    $MJ = 2 \cosh x \sinh x \cos y$
    
    $NJ = -\sinh^2 x \sin y$
    
    $\int M(x,~y)J(x) dx + c(y) = \int N(x, ~y)J(x) + c(x) = c^*$
    
    ∴ $\sinh^2 x \cos y =c$이다.

12. $(2xy dx + dy ) e^{x^2 } = 0$, $y(0) = 2$
    
    $2x e^{x^2 } y dx + e^{x^2} dy = 0$
    
    $M = 2x e^{x^2 } y$
    
    $N = e^{x^2}$
    
    $M_y = 2x e^{x^2}$
    
    $N_x = 2xe^{x^2}$
    
    $M_y = N_x$ 가 성립하므로 exact equation이 가능한 상황이다.
    
    $\int M(x,~y) dx + c(y) = \int N(x, ~y) + c(x) = c^*$
    
    $e^{x^2 } y = c$
    
    $1 \times 2 = c$
    
    ∴ $y = 2 e^{-x^2}$이다.

13. $e^{-y} dx + e^{-x} (-e^{-y} + 1)dy = 0$, $F = e^{x+y}$
    
    적분 요소가 주어졌으므로, 바로 식을 구하면,
    
    $e^{x} dx + e^{y} (-e^{-y} + 1)dy = 0$
    
    $\int e^{x} dx + c(y) = \int e^{y} (-e^{-y} + 1)dy + c(x) = c^*$
    
    $e^x + e^y - y =c$

14. $(a+1)y + (b+1)x dy = 0$, $y(1) = 1$, $F = x^a y^b$
    
    적분 요소가 주어졌으므로 다음을 바로 계산하자.
    
    $(a + 1) x^a y^{b+1} + (b + 1) x^{a+ 1} y^b dy = 0$
    
    $x^{a+1} y^{b+1} = 1$이다.


