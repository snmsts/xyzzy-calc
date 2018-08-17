# xyzzy-calc
common lisp port from xyzzy's [calc-mode](https://github.com/xyzzy-022/xyzzy/blob/develop/lisp/calc.l)
without mode facility.

# how to use
```
(calc-print (calc-eval (calc-read-from-string "100+20"))) ;; => 120
```

# todo
 * define function is disabled.
