# Fubini's **Thm**
Given an integrable function f(x,y)\
If  x,y are continuous on a region R and 
- $R$ is defined by
    $$
    \begin{aligned}
        a \leq &x \leq b\\
        g_1(x) \leq &y \leq g_2(x)
    \end{aligned}
    $$ 
    Then 
$$

\begin{aligned}
    \iint_Rf(x,y)dA = \int_a^b\int_{g_1(x)}^{g_2(x)}f(x,y)dydx    
\end{aligned}
$$

- $R$ is defined by 
    $$
    \begin{aligned}
        c \leq &x \leq d\\
        h_1(x) \leq &y \leq h_2(x)
    \end{aligned}
    $$

    Then 
$$
\begin{aligned}
    \iint_Rf(x,y)dA = \int_c^d\int_{h_1(x)}^{h_2(x)}f(x,y)dxdy
\end{aligned}
$$