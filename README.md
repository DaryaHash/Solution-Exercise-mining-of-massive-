# Solution-Exercise(mining-of-massive)

## chapter 2
* exercise 2.3.1
  * a) *map:* for each input integer n, define (k,n)-pair that k is constatnt
  then each chanck sort (k,ni ) and calculate (k, max (n1,.., nk))
  perpose max(1,...,nk) is nj and calculate hash (k, nj) and send to reduce
   *reduce:* in reduce sort again all (k, nj) then calculate (k, max(n1,...,nm))
   and output is (k,nmax)
  
  * b)*map:* for each input integer n, define (k,n)-pair that k is constatnt
  then each chanck sort (k,ni) and hash (k,(n1,.., nk)) end to reduce
   *reduce:* in reduce sort again all (k,(n1,...,nk)) then calculate (k,avrege(n1,...,nm))
   and output is (k,naverge)
   
  * c)
  * d)

* exercise 2.3.2
* exercise 2.3.3
* exercise 2.3.4
* exercise 2.3.5
