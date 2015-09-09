##  Our own maybe

Let's write our own maybe type:

    module Maybe where

    import Prelude hiding (Nothing, Just)

    data Maybe a = Nothing | Just a

And run it:

    ghci Maybe.hs
    > Just 4

    No instance for (Show (Maybe.Maybe a0))
    arising from a use of ‘print’
    In the first argument of ‘print’, namely ‘it’
    In a stmt of an interactive GHCi command: print it

