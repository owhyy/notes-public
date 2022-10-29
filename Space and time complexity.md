# Space and time complexity
#Programming #SICP

> How slow or fast a algorithm runs, and how many resources does it take up

**When talking about time complexity, the constant factor does not matter:**
- Suppose we have a program running in linear, $1000n$ time, and a program running in $n^2$ time, the $n^2$ one will be way faster for small inputs, but once n reaches big values, you need to double the time.

**Time complexity is not a good way to measure the quality of code**, because hardware is becoming faster and faster - so it's very platform dependent.