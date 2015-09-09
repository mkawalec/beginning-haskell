##  Types

There are types, from the simple ones:

    > :t 1
    1 :: Num a => a

    > :t "something"
    "something" :: [Char]

To some more complex ones:

    > import Data.Maybe
    > :t Just 5
    Just 5 :: Num a => Maybe a


