# Elisp memoization functions

See the header in the source file for details. It's very easy to use:

```cl
(require 'memoize)

(memoize 'my-function)
```

The macro `defmemoize` is also provided to directly create memoized
functions:

```cl
(defmemoize my-expensive-function (x)
  (if (zerop n)
      1
    (* n (my-expensive-function (1- n)))))
```
