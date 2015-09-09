##  What's going on?

    fib' :: [Integer]
    fib' = 1:1:zipWith (+) fib' (tail fib')

Assume we already know the fibbonacci sequence, then we have

    fib' = [1,1,2,3,5,8,12,..]
    tail fib' = [1,2,3,5,8,12,20,..]

`zipWith` applies the operation (addition) to corresponding elements of
the list, so:

    fib'                         = [1,1,2,3,5,8,12,..]
    tail fib'                    = [1,2,3,5,8,12,20,..]
    zipWith (+) fib' (tail fib') = [2,3,5,8,12,20,32,..]

We can 'lie' about knowing the rest of the list, because Haskell is
lazy!
