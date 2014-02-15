This page intentionally left blank
<br><br><br><br><br><br>
<span style="float:right;color:#888;font-style:italic;">(no it isn't)</span>

----

# Alternative testing
## by The Fat Man

<img style="height: 400px; display: inline-block;" src="../troy-mcclure1.jpg">
<img style="height: 400px; display: inline-block; margin-left:1em;" src="../Girls-stinky-cheesy-feetP-32027579468.jpeg">

----

# Introduction

Hi.  I know you're all pretty busy; I'll try to keep this short.

----

# Alternative testing

----

# Alternative testing

Or, "how can we test more, and better, with less work"

----

# Alternative testing

Or, "how can we test more, and better, with less work"

There're a million ways.  I'm going to cover two I like.

----

# Alternative testing

Or, "how can we test more, and better, with less work"

There're a million ways.  I'm going to cover two I like.

## 1) Stochastic
## 2) Property based

----

# Alternative testing

Or, "how can we test more, and better, with less work"

## 1) Stochastic
## 2) Property based

There is established tooling support for this in JS, Perl, Ruby, and PostgreSQL.  As a combined tool, originally comes from Haskell land, I think, in ***QuickCheck***.  I learned about it from the Erlang port `eqc`.

----

# I am programmar and wat is this

`stochastic randomized property based eigenvector cascade with a chroniton neutrino flux in the b-code parse tree until the warp tokenizer has a core breach in the increasing monotonic zermelo-franklin functor monad matrix because vector fetch macros are phase-transductive when mapped to a sequential left-zipper on closure clauses`

----

# Two related things

<img style="height: 300px;" src="../custom_dice_big.jpg">
<img style="height: 300px;" src="../function_addparameter_objectreleation2_3.gif">

----

# Two related things

1. Stochastic

<img style="height: 400px;" src="../custom_dice_big.jpg">

----

# Two related things

1. Stochastic
    1. ***Testing with Math.rand()***

----

# Two related things

1. Stochastic
    1. Testing with Math.rand()
    1. ***AKA***
        1. "fuzz testing," 
        1. "randomized testing," 
        1. "dart testing," 
        1. "lazy systematics"

----

# Two related things

1. Stochastic
    1. Testing with Math.rand()
    1. AKA ...
1. ***Property based***

<img style="height: 300px;" src="../function_addparameter_objectreleation2_3.gif">

----

# Two related things

1. Stochastic
    1. Testing with Math.rand()
    1. AKA ...
1. Property based
    1. ***"Given these circumstances, the answer should feel like X"***
    1. Gets less vague with examples

----

# Two related things

1. Stochastic
    1. Testing with Math.rand()
    1. **my\_function( rand\_int(), rand\_string() )**
1. Property based
    1. "Given these circumstances, the answer should feel like X"

----

# Two related things

1. Stochastic
    1. Testing with Math.rand()
    1. `my_function( rand_int(), rand_string() )`
1. Property based
    1. "Given these circumstances, the answer should feel like X"
    1. ***A function that returns the square of a float should always return a float"***

----

# Two related things

1. Stochastic
    1. Testing with Math.rand()
    1. `my_function( rand_int(), rand_string() )`
1. Property based
    1. "Given these circumstances, the answer should feel like X"
    1. A function that returns the square of a float should
        1. always return a float
        1. ***always `return >= 0`***

----

# Two related things

1. Stochastic
    1. Testing with Math.rand()
    1. `my_function( rand_int(), rand_string() )`
1. Property based
    1. "Given these circumstances, the answer should feel like X"
    1. A function that returns the square of a float should
        1. always return a float
        1. always return >= 0
        1. ***never underflow***

----

# Two related things

1. Stochastic
    1. Testing with Math.rand()
1. Property based
    1. "Given these circumstances, the answer should feel like X"
    1. ***A function that ... should ...***

----

# Two related things

1. Stochastic
    1. Testing with Math.rand()
1. Property based
    1. A function that ... should ...
1. ***Not joined at the hip***
    1. Can be used seperately
    1. Two great tastes that go great together

----

# Not identical

These are powerful tools that complement one another very well, and are easy to make alongside one another; so ***they often occur together*** and lots of people think of them as the same thing. You sometimes see this around classes and inheritance, too - you can have classes without inheritance and vice versa.

----

# Not identical

1. ***Randomized can also be "constructive"*** eg

----

# Not identical

1. Randomized can also be "constructive" eg
    1. ***Manufacturing test cases randomly with known specific answers***

----

# Not identical

1. Randomized can also be "constructive" eg
    1. Manufacturing test cases with known answers
    1. ***Usually you manufacture the answer alongside the test***
    1. "Okay, we'll put `&lt;b&gt;&lt;i&gt;&lt;/i&gt;&lt;/b&gt;` around it, and then require the answer to be `{ b: { i: 'whatever' } }`"

----

# Not identical

1. Randomized can also be "constructive" eg
    1. Manufacturing test cases with known answers
1. ***Property based can be "exhaustive"*** eg

----

# Not identical

1. Randomized can also be "constructive" eg
    1. Manufacturing test cases with known answers
1. Property based can be "exhaustive" eg
    1. ***Search the entire space, every property combination***
    1. Can get very expensive
    1. Is often impossible
    1. Randomization sparse search is the natural cure
    1. Sometimes you actually need to test every answer though

----

# Let's talk about stochastics

<img style="height: 500px; margin-top: 2em;" src="../hE67D906B.jpeg">

----

# Stochastic testing

----

# Stochastic testing

"Please do horrible things to / for me"

----

# Stochastic testing
## The small idea

"Please do horrible things to / for me"

----

# Stochastic testing
## The small idea

"Please do horrible things to / for me"

1. ***Testing on dice***

----

# Stochastic testing
## The small idea

"Please do horrible things to / for me"

1. Testing on dice
1. ***"I hate writing all these coverage cases"***

----

# Stochastic testing
## The small idea

"Please do horrible things to / for me"

1. Testing on dice
1. "I hate writing all these coverage cases"
1. ***"I never thought to try negative numbers"***

----

# Stochastic testing
## The small idea

"Please do horrible things to / for me"

1. Testing on dice
1. "I hate writing all these coverage cases"
1. "I never thought to try..."
    1. Negative numbers
    1. ***Non-numbers in my math function***

----

# Stochastic testing
## The small idea

"Please do horrible things to / for me"

1. Testing on dice
1. "I hate writing all these coverage cases"
1. "I never thought to try..."
    1. Negative numbers
    1. Non-numbers
    1. ***Missing values, who would forget the argument***

----

# Stochastic testing
## The small idea

"Please do horrible things to / for me"

1. Testing on dice
1. "I hate writing all these coverage cases"
1. "I never thought to try..."
    1. Negative numbers
    1. Non-numbers
    1. Missing values
    1. ***that weird and impossible grouping of settings***

----

# Stochastic testing
## The small idea

"Please do horrible things to / for me"

1. Testing on dice
1. "I hate writing all these coverage cases"
1. "I never thought to try..."
    1. Negative numbers
    1. Non-numbers
    1. Missing values
    1. "that grouping" of settings
    1. ***Dude who would call this with two extra arguments?  That doesn't even make sense***

----

# Stochastic testing
## The small idea

"Please do horrible things to / for me"

1. Testing on dice
1. "I hate writing all these coverage cases"
1. "I never thought to try..."
    1. Negative numbers
    1. Non-numbers
    1. Missing values
    1. "that grouping" of settings
    1. Wrong argument counts
    1. ***Chinese***

----

# Stochastic testing
## The small idea

"Please do horrible things to / for me"

1. Testing on dice
1. "I hate writing all these coverage cases"
1. "I never thought to try..."
    1. Negative numbers
    1. Non-numbers
    1. Missing values
    1. "that grouping" of settings
    1. Wrong argument counts
    1. Chinese
    1. ***Writing the month as a word, abbreviation, or in euro format***

----

# Stochastic testing
## The small idea

"Please do horrible things to / for me"

1. Testing on dice
1. "I hate writing all these coverage cases"
1. "I never thought to try..."
    1. Negative numbers
    1. Non-numbers
    1. Missing values
    1. "that grouping" of settings
    1. Wrong argument counts
    1. Chinese
    1. Unexpected notations
    1. ***Most of the things which make you want to stab users***

----

# Stochastic testing
## The small idea

"Please do horrible things to / for me"

1. Testing on dice
1. "I hate writing all these coverage cases"
1. "I never thought to try..."
1. ***"I didn't realize the behavior was `o(n^3)`"***

----

# Stochastic testing
## The small idea

"Please do horrible things to / for me"

1. ***Creates verifiable documentation***
1. Testing on dice
1. "I hate writing all these coverage cases"
1. "I never thought to try..."
1. Unexpected consequences

----

# Stochastic testing
## The small idea

"Please do horrible things to / for me"

1. Creates verifiable documentation
    1. ***Quite a bit better at this than unit testing***
1. Testing on dice
1. "I hate writing all these coverage cases"
1. "I never thought to try..."
1. Unexpected consequences

----

# Stochastic testing
## The small idea

"Please do horrible things to / for me"

1. Creates verifiable documentation
    1. Quite a bit better at this than unit testing
    1. ***It's documentation which fights back***
1. Testing on dice
1. "I hate writing all these coverage cases"
1. "I never thought to try..."
1. Unexpected consequences

----

# Stochastic testing
## The small idea

"Please do horrible things to / for me"

1. ***Much cheaper than unit testing***
1. Creates verifiable documentation
1. Testing on dice
1. "I hate writing all these coverage cases"
1. "I never thought to try..."
1. Unexpected consequences

----

# Stochastic testing
## The small idea

"Please do horrible things to / for me"

1. Much cheaper than unit testing
    1. ***One good stoch test is worth dozens of (related) unit tests***
1. Creates verifiable documentation
1. Testing on dice
1. "I hate writing all these coverage cases"
1. "I never thought to try..."
1. "I didn't realize the behavior was <tt>o(n^3)</tt>"

----

# Stochastic testing
## The small idea

"Please do horrible things to / for me"

1. Much cheaper than unit testing
    1. One good stoch test is worth dozens of (related) unit tests
    1. *For matrix coverage, dozens* ***per axis***

----

# Stochastic testing
## The small idea

"Please do horrible things to / for me"

1. Much cheaper than unit testing
    1. One good stoch test is worth dozens of (related) unit tests
    1. For matrix coverage, dozens per axis
    1. ***These arguably accumulate by multiplying, not adding, so for five axes, this is effectively tens of thousands of tests***

----

# Stochastic testing
## The small idea

"Please do horrible things to / for me"

1. ***Much cheaper than unit testing***
    1. One good stoch test is worth dozens of (related) unit tests
    1. For matrix coverage, dozens *per axis*
    1. Potentially thousands of free tests
    1. Fast and easy because not exhaustive (especially over many properties)
        1. Still alarmingly good at finding counter-examples


----

# Stochastic testing
## The small idea

"Please do horrible things to / for me"

1. ***Lets you test properties*** (hurr durr hence the name)
1. Much cheaper than unit testing
1. Creates verifiable documentation
1. Testing on dice
1. "I hate writing all these coverage cases"
1. "I never thought to try..."
1. Unexpected consequences


----

# Stochastic testing
## The small idea

"Please do horrible things to / for me"

1. Lets you test properties
    1. "This function is well defined under these circumstances:"
    1. Oh yeah?  ***Show me***.
1. Much cheaper than unit testing
1. Creates verifiable documentation
1. Testing on dice
1. "I hate writing all these coverage cases"
1. "I never thought to try..."
1. Unexpected consequences


----

# Stochastic testing
## The small idea

"Please do horrible things to / for me"

1. ***Does not limit itself to the stuff you thought of***
1. Lets you test properties
1. Much cheaper than unit testing
1. Creates verifiable documentation
1. Testing on dice
1. "I hate writing all these coverage cases"
1. "I never thought to try..."
1. Unexpected consequences


----

# Stochastic testing
## The small idea

"Please do horrible things to / for me"

1. Does not limit itself to the stuff you thought of
    1. ***This turns out to be very important in testing***
1. Lets you test properties
1. Much cheaper than unit testing
1. Creates verifiable documentation
1. Testing on dice
1. "I hate writing all these coverage cases"
1. "I never thought to try..."
1. Unexpected consequences


----

# Stochastic testing
## The small idea

"Please do horrible things to / for me"

1. ***Very good at finding subtle bugs in old, trusted code***
1. Does not limit itself to the stuff you thought of
1. Lets you test properties
1. Much cheaper than unit testing
1. Creates verifiable documentation
1. Testing on dice
1. "I hate writing all these coverage cases"
1. "I never thought to try..."
1. Unexpected consequences

----

# Property based
## The big idea

----

# Property based
## The big idea

1. Testing the way you think

----

# Property based
## The big idea

1. Testing the way you think
    1. Pause: **Someone please explain what cent splitting *should* do**

----

# Property based
## The big idea

1. Testing the way you think
    1. Pause: Someone please explain what cent splitting *should* do
    1. Please look into how that was phrased.

----

# Property based
## The big idea

1. Testing the way you think
    1. Assertions made about expectations

----

# Property based
## The big idea

1. Testing the way you think
    1. Assertions made about expectations
    1. Driven by clauses - "X should Y, except Z, when Q"

----

# Property based
## The big idea

1. Testing the way you think
    1. Assertions made about expectations
    1. Driven by clauses - "X should Y, except Z, when Q"
    1. In many ways very similar to Eiffel contracts (*sup Al*)

----

# Property based
## The big idea

1. Testing the way you think
    1. Assertions made about expectations
    1. Driven by clauses - "X should Y, except Z, when Q"
    1. In many ways very similar to Eiffel contracts
    1. Much simpler and easier to work with IMO

----

# Property based
## The big idea

1. Testing the way you think
    1. Assertions made about expectations
    1. Driven by clauses - "X should Y, except Z, when Q"
    1. In many ways very similar to Eiffel contracts
    1. Much simpler and easier to work with IMO
    1. Non-invasive - easier to read; not quite as strong

----

# Property based
## The big idea

1. Testing the way you think
    1. Assertions, clauses; like contracts
1. ***Results the way you want***

----

# Property based
## The big idea

1. Testing the way you think
    1. Assertions, clauses; like contracts
1. Results the way you want
    1. "Here is a case where your function defies the rule that you set: `[5, "tuesday", 11, 1988]`"

----

# Property based
## The big idea

1. Testing the way you think
1. Results the way you want
    1. "Here is a case: [5, "tuesday", 11, 1988]"
    1. Even without context, you get some idea what's gone wrong there

----

# Property based
## The big idea

1. Testing the way you think
1. Results the way you want
    1. "Here is a case: [5, "tuesday", 11, 1988]"
    1. Even without context, you get some idea what's wrong
    1. Need more counter-examples?  Cool.  Run it again.

----

# Property based
## The big idea

1. Testing the way you think
1. Results the way you want
    1. "Here is a case: [5, "tuesday", 11, 1988]"
    1. Even without context, you get some idea what's wrong
    1. Need more counter-examples?  Cool.  Run it again.
    1. In better tools there's "reduction"
        1. The tool will work with the case to try to make it simpler
        1. "Oh it looks like [1,"saturday",0,1988] fails too."
        1. Now we know it's probably the day label or the year
        1. We don't even know what the property is `:D`

----

# Why bother?

----

# Why bother?

1. More coverage

----

# Why bother?

1. More coverage
1. Easier, once you get it

----

# Why bother?

1. More coverage
1. Easier, once you get it
1. Great at finding edge cases

----

# Why bother?

1. ***Models the definition***
1. More coverage
1. Easier, once you get it
1. Great at finding edge cases

----

# But this doesn't work for

----

# But

1. UI/UX

----

# But

1. UI/UX
1. Round trip testing

----

# But

1. UI/UX
1. Round trip testing
1. Checking if the images load

----

# But

1. UI/UX
1. Round trip testing
1. Checking if the images load
1. etc etc etc

----

# But

Yep.  Property/Stoch is a pretty special case testing tool.  PagerDuty doesn't cover everything either.

----

# So where does it work for us?

----

# So where does it work for us?

1. Algorithms

----

# So where does it work for us?

1. Algorithms
1. Support coverage

----

# So where does it work for us?

1. Algorithms
1. Support coverage
1. Partial exhaustion


----

# So where does it work for us?

1. Algorithms
1. Support coverage
1. Partial exhaustion
1. Anything functionally round-trip

----

# So where does it work for us?

1. Algorithms
1. Support coverage
1. Partial exhaustion
1. Anything functionally round-trip
1. Verifying tool behavior

----

# So where does it work for us?

1. Algorithms
1. Support coverage
1. Partial exhaustion
1. Anything functionally round-trip
1. Verifying tool behavior
1. Bizarre cases

----

# So where does it work for us?

1. Algorithms
1. Support coverage
1. Partial exhaustion
1. Anything functionally round-trip
1. Verifying tool behavior
1. Bizarre cases
1. Any time you say "a user wouldn't be stupid enough to X, would they?"

----

# So where does it work for us?

1. Actually lots of other places too

The list was getting long and boring, and I had lots of other boring stuff to say.  Be glad I trap-doored.  But seriously, the more comfortable you get with property and stoch testing, the more places you see that it can be applied, often to great effect.

----

# So where does it work for us?

1. Algorithms
    1. ***Cent splitting***
1. Support coverage
1. Partial exhaustion
1. Anything functionally round-trip
1. Verifying tool behavior
1. Bizarre cases
1. Where user stupidity matters

----

# So where does it work for us?

1. Algorithms
    1. Cent splitting
        1. A function splitting cents in a group purchase should

----

# So where does it work for us?

1. Algorithms
    1. Cent splitting
        1. A function splitting cents in a group purchase should
            1. Be ready for purchase of multiple "tickets"

----

# So where does it work for us?

1. Algorithms
    1. Cent splitting
        1. A function splitting cents in a group purchase should
            1. Be ready for purchase of multiple "tickets"
            1. Always return the value for one purchase

----

# So where does it work for us?

1. Algorithms
    1. Cent splitting
        1. A function splitting cents in a group purchase should
            1. Be ready for purchase of multiple "tickets"
            1. Always return 
                1. the value for one purchase
                1. a non-negative price

----

# So where does it work for us?

1. Algorithms
    1. Cent splitting
        1. A function splitting cents in a group purchase should
            1. Be ready for purchase of multiple "tickets"
            1. Always return 
                1. the value for one purchase
                1. a non-negative price
                1. a price in whole cents

----

# So where does it work for us?

1. Algorithms
    1. Cent splitting
        1. A function splitting cents in a group purchase should
            1. Be ready for purchase of multiple "tickets"
            1. Always return 
                1. the value for one purchase
                1. a non-negative price
                1. a price in whole cents
                1. within one-cent-per-ticket of `total / count`

----

# So where does it work for us?

1. Algorithms
    1. Cent splitting
        1. A function splitting cents in a group purchase should
            1. Be ready for purchase of multiple "tickets"
            1. Always return 
                1. the value for one purchase
                1. a non-negative price
                1. a price in whole cents
                1. within one-cent-per-ticket of `total / count`
            1. ***Always add up to exactly the right price, iteratively***

----

# So where does it work for us?

1. Algorithms
    1. Cent splitting
        1. A function splitting cents in a group purchase should
            1. Be ready for purchase of multiple "tickets"
            1. Always return 
                1. the value for one purchase
                1. a non-negative price
                1. a price in whole cents
                1. within one-cent-per-ticket of `total / count`
            1. Always add up to exactly the right price
                1. ***No matter what order, grouping, etc***

----

# So where does it work for us?

1. Algorithms
    1. Cent splitting
        1. A function splitting cents in a group purchase should
            1. Be ready for purchase of multiple "tickets"
            1. Always return 
                1. the value for one purchase
                1. a non-negative price
                1. a price in whole cents
                1. within one-cent-per-ticket of `total / count`
            1. Always add up to exactly the right price
        1. ***If any of those fail, something is seriously wrong***

----

# So where does it work for us?

1. Algorithms
    1. Cent splitting
        1. A function splitting cents in a group purchase should
    1. ***Our old cent splitting stuff violated several of those***
        1. This was in production
        1. I hit it in real use, not testing
        1. Remember cents rounding lady

----

# So where does it work for us?

1. Algorithms
    1. Cent splitting
    1. ***Tag-aware text trimming*** (*Sup Andy*)
1. Support coverage
1. Partial exhaustion
1. Anything functionally round-trip
1. Verifying tool behavior
1. Bizarre cases
1. Where user stupidity matters

----

# So where does it work for us?

1. Algorithms
1. Support coverage
    1. ***Unicode*** (holy jesus srsly)
1. Partial exhaustion
1. Anything functionally round-trip
1. Verifying tool behavior
1. Bizarre cases
1. Where user stupidity matters

----

# So where does it work for us?

1. ***Unicode*** (holy jesus srsly)
    1. Every time you think you have it right, mix some Thai, some Chinese, some Arabic, and some Hebrew, then put that in
    1. Result: you did not actually have it right, did you
    1. Without randomized testing this is a fucking nightmare

----

# So where does it work for us?

1. Unicode (holy jesus srsly)
    1. Every time you think you have it right, mix some Thai, some Chinese, some Arabic, and some Hebrew, then put that in
    1. Result: you did not actually have it right, did you
    1. Without randomized testing this is a fucking nightmare
    1. Oh we're doing punycode urls with internationalization?  ***PLEASE PLEASE PLEASE STOCH PLEASE STOCH OH GOD I WILL DIE***

----

# So where does it work for us?

1. Algorithms
1. Support coverage
    1. Unicode
    1. Checking if our libraries work against all tags
1. Partial exhaustion
1. Anything functionally round-trip
1. Verifying tool behavior
1. Bizarre cases
1. Where user stupidity matters

----

# So where does it work for us?

1. Algorithms
1. Support coverage
1. Partial exhaustion
    1. Oh, it takes nine arguments and half are real valued?
1. Anything functionally round-trip
1. Verifying tool behavior
1. Bizarre cases
1. Where user stupidity matters

----

# So where does it work for us?

1. Algorithms
1. Support coverage
1. Partial exhaustion
    1. Oh, it takes nine arguments and half are real valued?
    1. Time to make a dart board
    1. It turns out it takes 2 million monkies to make Hamlet
1. Anything functionally round-trip
1. Verifying tool behavior
1. Bizarre cases
1. Where user stupidity matters

----

# So where does it work for us?

1. Algorithms
1. Support coverage
1. Partial exhaustion
1. Anything functionally round-trip
    1. `encode` / `decode`
1. Verifying tool behavior
1. Bizarre cases
1. Where user stupidity matters

----

# So where does it work for us?

1. Algorithms
1. Support coverage
1. Partial exhaustion
1. Anything functionally round-trip
1. Verifying tool behavior
    1. DOM-compare pre-minify to post-minify
    1. Great for sussing out limitations ahead of time
1. Bizarre cases
1. Where user stupidity matters

----

# So where does it work for us?

1. Algorithms
1. Support coverage
1. Partial exhaustion
1. Anything functionally round-trip
1. Verifying tool behavior
1. Bizarre cases
1. Where user stupidity matters
    1. Of course their name mixes Japanese, Hindi, and Tagalog; it's a unicode smiley
    1. Your test set didn't cover musical notation, the poo symbol, or i-ching hexagrams, did it

----

# Next steps

----

# Next steps

1. ***Andy, Forest, John, and Dave can neckbeard about which JS one to use***

----

# Next steps

1. JS Neckbearding
1. ***Naveed, Al, and Vat can civilly and responsibly choose a perl one***

----

# Next steps

1. JS Neckbearding
1. Perl Neckbearding
1. ***Let's look into writing up some requirements*** `:)`

----

# Thank you for coming

get the fuck out

( *or, questions?* )