// incomplete

Computers are better than humans at tracking time. Unlike human, they keep a constant track of time using hardware and structures, using any type of ocscillation or time protocols. But that's not at all intelligent of the machines. Just another algoritm doing its work. But by taking this away and making a computer create its own perception of time would be interesting.

Think of model where:
* we define a unit of time but do not provide computer with any mechanism to constantly track or know the time passing
* the computer is not always connected to Real Time Clock but has to make a request for time
* the request for time is penalised in the object function (treated as cost)
* computer needs to return() at time specified
* deviations in return time from time specified is also penalised
* computer treats the time requested by it as an epoch for "guessing" when the return is due but it does not keep any constant track of time from epoch (or maybe use all previous requests as references)
* whenever computer thinks the time to return arrives, it makes a request and validates if its the closest possible time to return. (If time to return is left, computer waits (guesses for when make next request) || If time to return is exceeded, computers returns immediately and incurrs penalty in proportion to how late did it return)

If we run such model, computer will try to guess right time to return with least requests. The penalty for time request and return deviations need to be decided upon.

If we allow the machine to learn from model overtime, it would be interesting (and scary) how computer gains "awareness" of time.
