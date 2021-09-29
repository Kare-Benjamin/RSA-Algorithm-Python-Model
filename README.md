# RSA-Algorithm-Python-Model

This is a RSA implementation which generates keys and tests decryption
and encryption using the RSA principles. It takes a prompt from the user
with the highest prime number in key calculations. Then creates keys 
with random "legal" values based on the RSA model. Meaning the same prime 
numbers will in most cases also result in different keys (e and d value), while
the n will remain permanent. With both random keys, and unpredictable
e/d values the key generator becomes a bit safer. The library secrets, 
(adviced for crypto security) is used in place of "random" for a bit
safer random-like performance. The keys are then used in both encryption and
decryption to test if the message (M) has been converted to (C) and then
unlocked (back to M). All the values of d,e,q,p,n and r are zeroed (deleted). 
So that we cannot cheat during encryption and decryption.

The gen_prime function is not fully our,
as we have adapted it to our usage and modified it. It is based on the 
sieve of eratosthenes which is an ancient algorithm for finding prime numbers
up to any given limit. 

The script has been thuroughly tested and no bugs are observed, however they
might exist, albeit well hidden as this is a random machine 
with way too many scnearios for the developers (us) to test.
