# Two's complement encoding

#Programming

- same as [[Unsigned encoding]], except the first [[9t6c-bits]] (most significant bit) is negative: ${2^i \cdot \ 0 \ or \ 1}$ : ${1101 = -1 \cdot 2^3 + 1 \cdot 2^2 + 0 \cdot 2^1 + 1 \cdot 2^0 = 4+1=-5}$
- smallest value is $10\dots0$ -> $-2^{w-1}$
- biggest value is $01\dots1$ -> $2^{w-1}-1$
- is called Two's complement, because for $x, -x = \mathbf{2}^w - x$ (for $w=16$ and $x=12345$, you have $-12345 = 2^16 - 12345 = 32768 - 12345$) ???
- for $T2U$ (two's complement to [[Unsigned encoding]]), we use $T2U_w(x)=\begin{cases} x+2^w,\quad x < 0 \\ x, \qquad \quad \ x \geq0\end{cases}$
