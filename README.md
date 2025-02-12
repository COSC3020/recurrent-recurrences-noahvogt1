# Recurrent Recurrences
I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice.

Give big $\Theta$ bounds for the following recurrence relations.

1.
$$ T(n) =
    \begin{cases}
        1 & n \leq 1\\
        T\left(\frac{n}{13}\right) + 5 & n > 1
    \end{cases}
$$

$T(n) = T(n/169) + 10$

$T(n) = T(n/13^i) + 5i$

Using $i = log_{13}(n)$  as a substitute.

$T(n) = T(1) + 5log_{13}(n)$

$T(n) \in \theta (log(n))$

2.
$$ T(n) =
    \begin{cases}
        1 & n \leq 1\\
        13 T\left(\frac{n}{13}\right) + 5 & n > 1
    \end{cases}
$$

$T(n) = 169T(n/169) + 10$

$T(n) = 13^iT(n/13^i) + 5i$

Using $i = log_{13}(n)$  as a substitute.

$T(n) = 1T(1) + 5log_{13}(n)$

$T(n) \in \theta (log(n))$

3.
$$ T(n) =
    \begin{cases}
        1 & n \leq 1\\
        13 T\left(\frac{n}{13}\right) + 2n & n > 1
    \end{cases}
$$

$T(n) = 169T(n/169) + 26n/13 + 2n$

$T(n) = 13^iT(n/13^i) i*2n$

Using $i = log_{13}(n)$  as a substitute.

$T(n) = 1T(1) 2nlog_{13}(n)$

$T(n) \in \theta (nlog(n))$
