# xyzzy-calc
common lisp port from xyzzy's [calc-mode](https://github.com/xyzzy-022/xyzzy/blob/develop/lisp/calc.l)
without mode facility.

# how to use
put files accessible from asdf

```
(ql:quickload :xyzzy-calc)
```

```
(xyzzy-calc:calc "100+20") ;; => 120
(xyzzy-calc:calc "fib(50)") ;; => 12586269025
```

# what is supported in calc
support non-lispy expression it understand operator precedence.
Paren are used for associativity.

## infix operators

 * ``+``
 * ``-``
 * ``*``
 * ``/``
 * % (remainder)
 * = (assign variable)
 * \ (rounded toward 0)
 * ^ (expotential)
 * << (lshift)
 * ``>>`` (rshift)
 * &  (logand)
 * |  (logor)
 * `  (logxor)

## prefix
 * ``+``
 * ``-``
 * ``~`` (lognot)

## suffix
 * ! (factrial)

## constants
 * pi
 * e

## functions
 * round
 * rem
 * ffloor
 * fceiling (or fceil)
 * ftruncate (or ftrunc)
 * fround
 * float
 * int
 * rational
 * complex
 * phase
 * cis
 * min
 * max
 * conjugate
 * signum
 * realpart (or real)
 * imagpart (or imag)
 * numerator (or num)
 * denominator (or den)
 * shift (or ash)
 * random (or rand)
 * fibonacci
 * fact
 * sigma

# todo
 * define function is disabled.
