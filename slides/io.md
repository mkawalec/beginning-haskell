##  IO

That's all fine and all, but let's actually do some input. How about a
program telling us if a number is odd?

    main = do
        putStrLn "Give a number, please"
        line <- getLine
        let num = read line :: Integer

        case num `mod` 2 of
            0 -> putStrLn $ "The number " ++ (show num) ++ " is even"
            1 -> putStrLn "It's odd"

We can clean it up, though.

