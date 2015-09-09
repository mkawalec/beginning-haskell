## The Two Styles of Fibonacci

    fib :: Integer -> Integer
    fib 0 = 1
    fib 1 = 1
    fib n = fib (n-1) + fib (n-2)

But wait

    fib' :: [Integer]
    fib' = 1:1:zipWith (+) fib' (tail fib')

WAT?

