# Generalizing Integrals to multivariate functions

## Recall from the FTC II
##### Finding the area under the curve
$$\int_{a}^{b}f(x)dx, \text{ for some function } f(x) \rightarrow \mathbb{R}, where x \in \mathbb{R}$$


##### We want to generalize this for 
$$f(x,y) \rightarrow \mathbb{R}, \text{where } x,y\in \mathbb{R}$$

Intuituvely this means that we would like the find the 3d-area under the 3d-curve, ie: the *volume* under the *surface*

##### Recall
$$\lim_{n\rightarrow \infty }\sum_{k=1}^{n} f(x_k)\Delta x_k = \int_a^bf(x)dx$$

##### So 
Lets take consider taking the volume over the rectangular space. By developing a Reiman Sum
$$a \leq x \leq b$$
$$c \leq y \leq d$$
Recall that the volume of a rectangular prism is 
$$V = lwh = A(x)h$$
Lets say that 
- $l$ be the distance in the x axis 
- $w$ be the distance in the y axis
- $h$ be the distance in the z axis



##### So
Lets develop a Reiman Sum with our knowledge of the volume formula

- Let $\Delta x_k$ be the change of $l$
- Let $\Delta y_k$ be the change of $w$
- We know that $f(x_k, y_k)$ will be the height of the surface at a point $x_k, y_k$

##### Then 
$$V = \lim_{n \rightarrow \infty}\sum_{k=1}^{n} f(x_k, y_k)\Delta x_k \Delta y_k$$


##### Def
If the limit of the Rieman sums of $f(x,y)$ as it approaches $\infty$\
Then we say f(x,y) is integrable\
And we write the Reiman Sum as:

$$
\begin{aligned}
    V &= \lim_{n \rightarrow \infty}\sum_{k=1}^{n} f(x_k, y_k)\Delta x_k \Delta y_k\\
    &= \int\int_Rf(x,y)dA \qquad\text{The double integral over a region R}
\end{aligned}
$$
