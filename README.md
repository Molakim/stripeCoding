# Stripe Coding Challenge 16/11/2018

I was asked to code a simple "Radar" that will check if a transaction was allowed or not.

Given a string :

```java
String charge = "["CHARGE:card_country=US&currency=USD&amount=250&ip_country=CA","ALLOW:amount>500", ]"
```
the algorithm has to return 1 of the transaction is allowed and 0 if not.\
We have 2 different family rules : ALLOW and BLOCK, and both of them can accept up to 2 rules separated by an OR or an AND.\
We have 6 different operations ( >, <, >=, <=, ==, !=)

## Improvements 

1. Using regex to process the initial string
2. Reduce the boilerplate code
3. Taking in consideration the edge case where we have rules like : "ALLOW:amount>500ANDamount<2000"

## FeedBack

I couldn't finish in 1h15 because I am not familiar with regex, which forced me to use different tricks that are very time consuming. But I had a lot of fun trying to solve this problem even if my solution is not the best.

## Thanks

* Special thanks to [Stripe](https://stripe.com) that gave me the chance to take this challenge.
* And [HackerRank](https://hackerrank.com) that provided a nice user experience with their online IDE.
