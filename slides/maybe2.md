We missed something, let's add a typeclass derivation:


    module Maybe where

    import Prelude hiding (Nothing, Just)

    data Maybe a = Nothing | Just a deriving (Show)

And run it:

    ghci Maybe.hs
    > Just 4
    Just 4

    > :t Just 4
    Just 4 :: Num a => Maybe.Maybe a

Yey!
