@def title = "My Franklin Sandbox"
@def hasmath = true
@def hascode = true

# Set up

## Update title

## Update config.md file

* change author

* add site name for GitHub

## Cretate a table of contents

\toc

## Upload using GitHub Desktop

# Examples

## How to enter text

 Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec sodales, ante tristique iaculis blandit, risus nibh rhoncus urna, aliquet accumsan nisi est eget lorem. Sed sit amet justo neque. Cras tellus leo, scelerisque nec urna in, varius mollis risus. Mauris feugiat aliquet quam quis vulputate. Aenean arcu mi, rutrum quis mauris ut, suscipit iaculis sapien. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Ut neque justo, efficitur id urna sed, lacinia ultrices nunc. Nunc magna turpis, consequat sed ligula et, viverra facilisis ligula. Aenean at vulputate velit, eu consequat tellus. Proin mollis congue massa, non consequat nulla ullamcorper non. Vestibulum id purus ut odio tempus cursus a eget tortor. Etiam vel sem eu elit facilisis pulvinar. Morbi in ligula tincidunt, eleifend nibh vel, viverra mi.

Quisque a nibh elementum, convallis urna quis, rhoncus dui. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia curae; Quisque dignissim velit nec sem tincidunt lacinia. Phasellus pharetra accumsan mauris, cursus aliquam erat hendrerit in. Etiam augue ante, lacinia at ultricies eu, varius non ante. Sed accumsan nunc non fermentum tempor. Phasellus imperdiet in nulla vitae pellentesque. Phasellus condimentum tortor a nibh imperdiet rutrum. Donec id hendrerit nunc, in finibus nulla. 

## How to render math equations

Examples from the last tutorial

$$ a^2 + b^2 = c^2 $$

$$ \frac{d}{dx} \int_a^x f(t) dt = f(x)$$

$$ \bar{x} = \frac{1}{n} \Bigg(\sum_{i=1}^n x_i \Bigg) = \frac{x_1 + x_2 + \cdots + x_n}{n}$$

$$
    \begin{alignedat}{3}
        2&x + y \space - &z &= &8 \\
        -3&x - y + 2&z &= \space&-11 \\
        -2&x + y + 2&z &= &-3
    \end{alignedat}
$$

$$
 M = 
    \begin{bmatrix}
        \begin{aligned}
            &2 & &1 & -&1\space \\
            \space-&3 & -&1 & &2 \\
            -&2 & &1 & &2 
        \end{aligned}
    \end{bmatrix}
$$

(optional: disable numbering)

## How to insert Julia code (with outputs!)

Hello, World!

```julia:./ex11
println("Hello, World!")
```

\show{./ex11}

Basic Math

```julia:./ex12
1 + 1
```

\show{./ex12}

Create Function

```julia:./ex13
function add(x,y)
    x + y
end
```

\show{./ex13}

Call Function

```julia:./ex14
add(2, 3)
```

\show{./ex14}

Random Numbers

```julia:./ex15
rand(5,5)
``` 

\show{./ex15}

## How to insert a table from a CSV file

World Population by Region by Year:

\tableinput{}{./tableinput/population_by_year.csv}

@@source
Source: Wikipedia
@@

## How to insert an image file

![beeswarm plot of population by region](/assets/p_beeswarm_region.svg)

@@source
Source: Wikipedia
@@

## How to insert a clickable thumbnail to a YouTube video
[![TY thumbnail](https://img.youtube.com/vi/fVBiLEtZB7A/0.jpg)](https://youtu.be/fVBiLEtZB7A)

## How to inject raw HTML
~~~
<iframe width="640" height="360" src="https://www.youtube.com/embed/fVBiLEtZB7A" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
~~~


<!-- # Franklin syntax sandbox

This page is meant as a sandbox for Franklin Syntax so that you can quickly practice or experience things.

## Sandbox

Write whatever you want here to practice Franklin Syntax:

```julia:./ex1
using LinearAlgebra, Random
Random.seed!(135)
a, b = randn(50), randn(50)
println(dot(a, b))
println(sum(ai * bi for (ai, bi) ∈ zip(a, b)))
```

\output{./ex1}

(yet another example that floating point arithmetics can be complicated).

$$ \forall x \in \R:\quad \scal{x, x} \ge 0 $$

\newcommand{\E}{\mathbb E}

Surely some people remember the ordering, but I always forget:

$$ \varphi(\E[X]) \le \E[\varphi(X)] $$

for $\varphi$ convex.
 -->