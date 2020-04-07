# Homework 1
#### Grant Gilson
#### 915804456

* 1
  * a
    $$
    \begin{aligned}
        \int_0^2\int_{-1}^1(x-y)dydx =&
        \int_0^2 (xy - \frac{y^2}{2}) \bigg]_{-1}^1 dx\\
        =& \int_0^2 (2x)dx\\
        =& x^2 \bigg]_0^2\\
        =& 4
    \end{aligned}
    $$

  * b
    $$
    \begin{aligned}
        \int_0^3 \int_{-2}^0 (x^2y-2xy) dydx=&
        \int_{-2}^0 \int_0^3 (x^2y-2xy) dxdy, \quad\text{by Fubini's Thm}\\
        =& \int_{-2}^0 (\frac{x^3}{3}-x^2y) \bigg]_0^3 dy\\
        =& \int_{-2}^0 (9 - 9y)dy\\
        =& 9y - \frac{9y^2}{2} \bigg]_{-2}^0\\
        =& 0
    \end{aligned}
    $$
  * c
    $$
    \begin{aligned}
        \int_{0}^1 \int_{0}^1 (\frac{y}{1+xy})dxdy =&
        \int_{0}^1 \int_{u_b}^{u_b} \frac{du}{u} dy, \quad \text{for}
        \begin{cases}
            u &= 1 + xy\\
            du &= ydx
        \end{cases}\\

        =& \int_{0}^1 \ln(u) \bigg]_{u_b}^{u_b} dy\\
        =& \int_{0}^1 \ln(1 + xy) \bigg]_{0}^1 dy\\
        =& \int_{0}^1 \ln(1+y)dy\\
        =& \int_1^2\ln(u)du, 
        \quad \text{for}  
        \begin{cases}
            u &= 1 + y\\
            du &= dy
        \end{cases}\\
        =& u \ln(u) - u \bigg]_1^2\\
        =& 2\ln(2) - 1
    \end{aligned}
    $$
  * d 
    $$
    \begin{aligned}
        \int_0^{\ln2}\int_1^{\ln5}(e^{2x+y}dydx) =&
        \int_0^{\ln2}\int_{u_a}^{u_b}e^ududx, 
        \quad \text{for}
        \begin{cases}
          u &= 2x+y\\
          du &= dy
        \end{cases}\\
        =& \int_0^{\ln2}e^{2x+y} \bigg]_1^{\ln5}dx\\
        =& (5-e)\int_0^{\ln2}e^{2x}dx\\
        =& \frac{(5-e)}{2}\int_{u_a}^{u_b}e^udu,
        \quad \text{for}
        \begin{cases}
          u &= 2x\\
          du &= 2dx
        \end{cases}\\
        =& \frac{(5-e)}{2} \bigg[ e^{2x}\bigg]_{0}^{\ln2}\\
        =& \frac{3}{2}(5-e)
    \end{aligned}
    $$
  * e
    $$
    \begin{aligned}
      \int_{-1}^2\int_0^{\pi/2} (y\sin x) dxdy
      =& \int_{-1}^2 -y\cos x \bigg ]_0^{\pi/2} dy\\
      =& \int_{-1}^2ydy\\
      =& \frac{y^2}{2} \bigg ]_{-1}^2\\
      =& \frac{3}{2}

    \end{aligned}
    $$
  * f
    $$
    \begin{aligned}
      \int_1^4\int_1^e \frac{\ln x}{xy} =& 
      \int_1^4\int_0^1 \frac{u}{y}dudy, \quad
      \begin{cases}
        u &= \ln x\\
        du &= \frac{1}{x}dx
      \end{cases}\\
      =& \int_1^4\frac{u^2}{2y} \bigg]_0^1 dy\\
      =& \frac{1}{2}\int_1^4 \frac{1}{y}dy\\
      =& \frac{1}{2} \ln y \bigg ] _1^4\\
      =& \ln2
    \end{aligned}
    $$

2. Find values of $c$ 
$$
\begin{aligned}
  \int_{-1}^c \int_0^2 xy + 1 dydx &= 4 + 4c\\
   \int_{-1}^c \frac{xy^2}{2} + y \bigg]_0^2dx &= \vdots\\
   \int_{-1}^c 2x + 2 dx &= \vdots\\
   x^2 + 2x\bigg]_{-1}^c &= \vdots\\
   c^2 + 2c + 1 &= 4 + 4c\\
   (c-3)(c+1)&= 0\\
   c = -1, c = 3
\end{aligned}
$$

3. Eval integrals over the Rectangle R:
     * a
     $$
     \begin{aligned}
       \iint_R \frac{\sqrt{x}}{y^2}dA 
       =& \int_0^4\int_1^2 \frac{\sqrt{x}}{y^2}dydx\\
       =& \int_0^4\sqrt{x}\ln y \bigg ] _1^2dx\\
       =& \ln 2 \int_0^4\sqrt x dx\\
       =& \ln 2 \bigg[ \frac{2}{3}x^{3/2}\bigg]_0^4\\
       =& \frac{16}{3}\ln 2
     \end{aligned}
     $$  
     * b 
     $$
     \begin{aligned}
       \iint_R (xy\cos y) dA 
       =& \int_0^\pi \int_{-1}^1 (xy\cos y) dx dy\\
       =& \int_0^\pi \frac{x^2}{y}\cos y\bigg ] _{-1}^1 dy\\
       =& \int_0^\pi y \cos y dy \\
       =& y \sin y - \int_0^\pi (\sin y )dy \quad \text{apply integration by parts}
       \begin{cases}
         u = y, \quad dv = \cos y\\
         du = dy, \quad v = \sin y\\
       \end{cases}\\
       =& y \sin y + \cos y \bigg ] _0^{\pi}\\
       =& 2
     \end{aligned}
     $$

     * c
     $$
     \begin{aligned}
       \iint_R xye^{xy^2}dA 
       =& \int_0^2\int_0^1 xye^{xy^2}dydx\\
       =& \int_0^2\int_{u_a}^{u_b} \frac{1}{2}dudx, 
       \begin{cases}
         u = e^{xy^2}\\
         du = 2xye^{xy^2}dy
       \end{cases}\\
       =& \frac{1}{2} \int_0^2 u \bigg ]_{u_a}^{u_b}dx\\
       =& \frac{1}{2} \int_0^2 e^{xy^2} \bigg] _0 ^1\\
       =& \frac{1}{2} \int_0^2 e^x -1 dx\\
       =& \frac{1}{2} (e^2 - 3)

     \end{aligned}
     $$

     * d 
     $$
     \begin{aligned}
       \iint_R \frac{y}{x^2y^2 + 1}dA 
       =& \int_0^1 y \int_0^1 \frac{1}{x^2y^2 + 1}dxdy\\
       =& \int_0^1 y \int_0^y \frac{1}{y(1+u^2)}dudy,\begin{cases}
         u = xy\\
         du = ydx
       \end{cases}\quad \text{ and apply arctan antiderivative subsitution}\\
       =& \int_0^1 \arctan(u)\bigg]_0^ydy\\
       =& \int_0^1 \arctan(y)dy\\
       =& y\arctan(y) - \frac{1}{2} \ln(y^2+1) \bigg]_0^1\\
       =& \frac{\pi}{4} - \frac{1}{2} \ln(2)
     \end{aligned}
     $$

4. 
  $$
  \begin{aligned}
    \int_{-1}^1\int_{-1}^1x^2+y^2dxdy
    =& \int_{-1}^1\frac{x^3}{3} + y^2x\bigg]_{-1}^1dy\\
    =& \int_{-1}^1\frac{2}{3} + 2y^2dy\\
    =& \frac{2}{3}y + \frac{2}{3}y^3 \bigg] _{-1}^1\\
    =& \frac{8}{3}

  \end{aligned}
  $$
