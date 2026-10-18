# debug_log.md
# Author: Joshua Reddish

## Bug 1
Error type: KeyError
File + line: week8_buggy.py, line 12, inside get_total()
What the error means: Python tried to access the dictionary key 'amount', but the key was missing from the first record.
What I told the duck: The function starts total at 0, loops through each record, and adds rec['amount'] to total. Taylor's record uses the key 'amout', so Python cannot find 'amount'.
What I tried: I read the traceback from the bottom up and identified the missing dictionary key.
How I fixed it: change the type to amount instead of amout

## Bug 2
Error type: TypeError
File + line: week8_buggy.py, line 16
What the error means: Python cannot compare an integer with a string using the greater-than operator.
How I fixed it: I removed the quotation marks around 1000 so both values are numeric.

## After Fixing Both Bugs
Final output:Total: $5150.00 across 3 records and True.
Pytest result: Yes — 5 passed.

## AI Literacy Reflection
Did I use AI? Yes
exact prompt I used: I shared my debugging lab instructions and asked ChatGPT to help me work through the lab step by step.
What AI explained: ChatGPT explained how to read the KeyError traceback and identify the missing dictionary key.
What I changed myself: the debugging code
Can I explain every fixed line? yes

## What I learned
I learned how to use the debugging system is vs code and also the importance of running code before hand to make sure everything is running as it should.I also learned the importance of checking spelling because that was one of the key issues with bug #1. finally make sure to check intergers to make sure vs code and your personal code picks up on the actual amount being used.