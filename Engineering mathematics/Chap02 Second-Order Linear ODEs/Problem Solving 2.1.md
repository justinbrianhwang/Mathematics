
3. $y'' + y' = 0$
    
    Since $y'' = -y'$, the solution is of the form $y = e^{-x}$.
    
    Therefore, $y = c_1 e^{-x} + c_2$.

4. $2xy'' = 3y'$
    
    Let $y' = u$.
    
    $2x u' = 3u$
    
    $\frac{1}{u} u' = \frac{3}{2} \frac{1}{x}$
    
    $\ln |u| = \frac{3}{2} \ln x + c$
    
    $u = c x^{\frac{3}{2}}$
    
    $y' = c x^{\frac{3}{2}}$
    
    Therefore, $y = c_1 x^{\frac{5}{2}} + c_2$.

5. $yy' = 3y'^2$
    
    Let $y' = u$.
    
    $yu' = 3y'u$
    
    $\frac{1}{u} u' = \frac{3}{y} y'$
    
    $\ln |u| = \ln y^3 + c$
    
    $u = cy^3$
    
    $y' = cy^3$
    
    $\frac{1}{y^3} y' = c$
    
    $-\frac{1}{y^2} = c_1 x + c_2$
    
    $y^2 = \frac{1}{c_1 + c_2 x}$
    
    $y = \sqrt{\frac{1}{c_1 + c_2 x}}$

6. $xy'' + 2y' + xy = 0$, given $y_1 = \frac{\cos x}{x}$
    
    Let $y_2 = uy_1$.
    
    ${y_2}' = u'y_1 + u{y_1}'$
    
    ${y_2}'' = u''y_1 + 2u'{y_1}' + u{y_1}''$
    
    Substituting into the original equation, we get:
    
    $xu''y_1 + 2xu'y_1' + xu y_1'' + 2u'y_1 + 2u y_1' + xu y_1 = 0$
    
    $u''(xy_1) + u'(2xy_1' + 2y_1) + u(y_1'' + 2y_1 + xy_1) = 0$
    
    Given $y_1'' + 2y_1 + xy_1 = 0$, we have:
    
    $u''(xy_1) = -u'(2xy_1' + 2y_1)$
    
    Let $u' = v$.
    
    $v'(xy_1) = -v(2xy_1' + 2y_1)$
    
    $\frac{1}{v} v' = -\frac{2}{y_1} y_1' - \frac{2}{x}$
    
    $\ln |v| = \ln |y^{-2}| + \ln |x^{-2}| + c$
    
    $v = \frac{1}{y_1^2} \frac{1}{x^2} \times c$
    
    $u' = \frac{c}{y_1^2 x^2}$
    
    Given $y_1 = \frac{\cos x}{x}$:
    
    $u' = c \sec^2 x$
    
    $u = c_1 \tan x + c_2$
    
    Therefore, $y_2 = \frac{\cos x}{x} (c_1 \tan x + c_2)$
    
    $y_2 = \frac{c_1}{x} \sin x + \frac{c_2}{x} \cos x$

7. $y'' + {y'}^3 \sin y = 0$
    
    $y'' = -\sin y {y'}^3$
    
    $-\frac{1}{y'^2} y'' = \sin y y'$
    
    $\frac{1}{y'} = -\cos y + c$
    
    $y' = \frac{1}{c - \cos y}$
    
    Integrating, we get:
    
    $c - \cos y y' = 1$
    
    $c + cy - \sin y = x$

8. $y'' = 1 + {y'}^2$
    
    Let $y' = u$.
    
    $u' = 1 + u^2$
    
    $\frac{1}{1 + u^2} u' = 1$
    
    $\arctan (u) = x + c$
    
    $u = \tan(x + c)$
    
    $y' = \tan(x + c)$
    
    $y = -\ln|\cos(x + c_1)| + c_2$

9. $x^2 y'' - 5xy' + 9y = 0$, given $y_1 = x^3$
    
    Let $y_2 = uy_1$.
    
    ${y_2}' = u'y_1 + u{y_1}'$
    
    ${y_2}'' = u''y_1 + 2u'{y_1}' + u{y_1}''$
    
    Substituting into the original equation, we get:
    
    $u''(x^2 y_1) + u'(x^2 {y_1}' + 5xy_1) = 0$
    
    $u'' (x^2 y_1) = -u' (x^2 y_1' + 5xy_1)$
    
    $\frac{1}{u'}u'' = -\frac{y_1'}{y_1} - \frac{5}{x}$
    
    $\ln |u'| = -\ln|y_1 \times x^5|$
    
    $u' = \frac{1}{x^8}$
    
    $y_2 = -\frac{1}{7}x^{-4}$

10. $y'' + (1 + \frac{1}{y})y'^2 = 0$
    
    $y'' = - (1 + \frac{1}{y})y'^2$
    
    $\frac{1}{y'} y'' = -(1 + \frac{1}{y})y'$
    
    Let $y' = u$.
    
    $\frac{1}{u} u' = -(1 + \frac{1}{y})y'$
    
    $\ln|u| = -y - \ln | y| + c$
    
    $u = \frac{c}{y} e^{-y}$
    
    $y' = \frac{c}{y} e^{-y}$
    
    $yy' = ce^{-y}$
    
    $ye^y y' = c$
    
    $\int ye^y dy = \int c dx$
    
    $ye^y - e^y = c_1 x + c_2$





