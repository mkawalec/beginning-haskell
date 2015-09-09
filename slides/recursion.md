##  Recursion

Let's declare a function that counts the length of a list

    len :: [a] -> Int
    len []     = 0
    len (x:xs) = 1 + len xs

We can even delete the type declaration!
