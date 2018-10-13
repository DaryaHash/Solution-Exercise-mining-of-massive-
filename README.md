# Solution-Exercise(mining-of-massive)

## chapter 2
* exercise 2.3.1
  * a)
  
  **map:** for each input integer n, define (k,n)-pair that k is constatnt
  then sort (k,ni ) and calculate (k, max (n1,.., nk))
  perpose max(1,...,nk) is nj and calculate hash (k, nj) and send to reduce
  
   **reduce:** in reduce sort again all (k, nj) then calculate (k, max(n1,...,nm))
   and output is (k,nmax)
  
  * b)
  
  **map:** for each input integer n, define (k,n)-pair that k is constatnt
  then sort (k,ni) and hash (k,(n1,.., nk)) send to reduce
  
   **reduce:** in reduce sort again all (k,(n1,...,nk))-pairs then calculate (k,avrege(n1,...,nm))
   and output is (k,na verge) 
   
  * c)
   
  **map:** for each input integer n, define (n,1)-pair
  then sort (ni,1)-pairs and instate all (ni,1)-pairs that ni is same include just one (ni,1)-pair
  and calculate hash (ni,1)
  send m hash (ni,1) to reduce that m is the number of  pairs with diffrent ni
  
   **reduce :** in reduce sort again all (ni,1)-pair if (ni,1)-pair is same  incude just one
   and output is (ni,1)

  * d)
  
  **map:** for each input integer n, define (1,1)-pair
  then calculate (1,(1+1+...+1)) and send hash (1,(1+...+1))
  
   **reduce :** in reduce calculate all (1,(1+...+1+1+...+1+...)) and output is (1,count number)

* exercise 2.3.2


* exercise 2.3.4
* exercise 2.3.5
