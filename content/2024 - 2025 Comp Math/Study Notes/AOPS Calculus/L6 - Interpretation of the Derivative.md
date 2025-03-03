##### Increasing/Decreasing
$f'(x)$ represents the slope of $f(x)$.

We say a function $f$ is monotone increasing on some set of points $S$ if for all $a,b$ points in $S$ with $a<b$, $f(a) \le f(b)$. Strictly decreasing is if $a<b$, $f(a)<f(b)$.
Similarly, $f$ is decreasing if $a<b$ then $f(a) \ge f(b)$.

When $f'(x) \ge 0$ for some interval $(a,b)$, $f(x)$ is monotone increasing in that range.
**Intuition:**
If $f'(a) = \lim_{h \rightarrow 0}{ \frac{f(a+h) - f(a)}{h}}>0$, then 
- If $h>0$, $f(a+h)>f(a)$.  
- If $h<0$, $f(a+h)<f(a)$. 
- Thus, we can deduce that $f(x)$ behaves like an increasing function near point $a$. 

When $f(x)$ is decreasing, slope is negative so $f'(x) < 0$.
- Similar idea can be used to deduce that $f(x)$ behaves like a decreasing function near point $a$ when $f'(a)<0$.

When $f(x)$ reaches local min/max, slope is $0$ so $f'(x)=0$, meaning the graph is just a constant (horizontal line).

**Example:** Given a cubic function $f(x) = x^3-3x^2+1$, sketch the ranges of increase and decrease.
Draw the graph. Splitting this graph up into ranges, we have it is increasing in range $(-\infty,0), (2,\infty)$ and decreasing in range $(0,2)$. Moreover, the graph crosses the x-axis at least once in each section. Since in each section the graph is strictly increasing or decreasing, it means that there is only one number in each range equal to a root. Since there are 3 ranges and thus 3 roots, that is all the roots of the cubic polynomial.

##### Concavity
$f''(x)$, the second derivative, represents the rate of change in the slope of $f(x)$, so determines whether $f'(x)$ is increasing or decreasing.

When $f''(x) >0$, the graph is concave up (parabola pointing upwards).
- Slope is increasing.
- Tangent line lies below the curve, secant line lies above curve.
When $f''(x) < 0$, the graph is concave down (parabola pointing downwards).
- Slope is decreasing, so slowly going from positive to 0, then going back down to negative.
- Tangent line lies above the curve, secant line lies below the curve.

When $f''(x) = 0$, the slope of the graph doesn't change.
- At this point, the concavity MAY switch. If the concavity changes, $x$ is called an **inflection point**.
- Though, it's not an inflection point if the concavity doesn't change. Take $f(x)=ax+b, f''(x)=0$ for example, where $x$ is not an inflection point. 
- Thus, concavity only switch at some $x$ where $f''(x) = 0$, but not necessarily the inverse.


##### Applications in Physics
Let $f(t)$ be a function based on time $t$, then
- $f'(t)$ represents the instantaneous rate of change at $t$.
	- Average rate of change from time $a$ to time $b$ is $\frac{f(b)-f(a)}{b-a}$. Let $b = a+h$, then it's $\frac{f(a+h)-a}{h}$ which is $f'(t)$.
	- If $f(t)$ is position, $f'(t)$ is instantaneous velocity.
- If $f(x)$ is position, $f''(x)$ represents the acceleration



##### About Functions
A continuous segment function will have a local min/max.
- It's derivative, if differentiable, will be 0.
Let $f$ be a continuous function on $[a,b]$.
If $f$ has max at $c$ inside $(a,b)$ and $f$ is differentiable at $c$, then $f'(c)=0$.
- Proof: $f'(c) = \frac{f(c+h)-f(c)}{h}$, $f'(c) \le 0$ when $h$ is positive and $f'(c) \ge 0$ when $h$ is negative. Thus, $f'(c)=0$.
If $f$ has min at $d$ inside $(a,b)$ and $f$ is differentiable at $d$, then $f'(d)=0$.
- Proof: Similar to proving max.

Let $f$ be a continuous function on $[a,b]$ and differentiable, but with $f(a)=f(b)$.

**Rolle's Theorem:** There must exist some $c$ in $(a,b)$ such that $f'(c)=0$. Proof: Either $c$ is the max or min point in which it works. An edge case is if max and min point are both $a$ and $b$, but since $f(a) = f(b)$ this means it's just a horizontal line anyways, so we can pick any point in $(a,b)$ as $c$.

Imagine a function in $[a,b]$ and differentiable on $(a,b)$ where $f(a) \neq f(b)$. If we rotate the graph, we may force it to have $f(a)=f(b)$. This means there exists some $c$ in $(a,b)$ that is max/min point by Rolle's Theorem. This means $f'(c)$ in the original function (slope of $c$) is equal to the slope of the secant line from $a$ to $b$. 

**Mean Value Theorem:** If $f$ is continuous function on interval $[a,b]$ and differentiable on $(a,b)$, then there exists some real $c$ with $a<c<b$ such that 
$$
f'(c) = \frac{f(b)-f(a)}{b-a}.
$$
Here, $\frac{f(b)-f(a)}{b-a}$ represents the rate of change.
- If $f(t)$ is position, this is just average velocity
- Mean Value Theorem states that there must be some point on the trip where the object's velocity will be exactly the average velocity of the entire trip (assuming $f$ is differentiable).


Let $f$ be function continuous on $[a,b]$ and differentiable on $(a,b)$. Prove if $f'(x)=0$ for all $x$ in $(a,b)$, then $f$ is constant on $[a,b]$.
We want to prove $f(x)=c$, and thus $f(a)=c$ since $f(x)=f(a)$.
Note for all $x$, by MVT, there must exist some $y$ in $(a,x)$ such that $f'(y) = \frac{f(x)-f(a)}{x-a}$. Since it must be that $f'(y)=0$, so $f(x)-f(a)=0,f(x)=f(a)$.








