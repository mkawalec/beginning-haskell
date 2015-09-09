##  Quicksort

Counting the length of a list is all nice, but what if we wanted to sort
stuff ourselves?

    qs :: Ord a => [a] -> [a]
    qs [] = []
    qs (x:xs) = qs [y | y <- xs, y <= x] ++ [x] ++ [y | y <- xs, y > x]
