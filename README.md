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
  
  **map:** for each input integer n, define (n ,1)-pair
  then sort (n ,1)-pairs and if m same pairs include (n,(1,...,1)) that number of 1 is m
  and calculate hash (n,(1,...,1)) 
  send m hash (n,(1,...,1)) to reduce
  
   **reduce :** in reduce sort again all (n,(1,..,1))-pairs then if n is same include
   (n,(1,...,1,1,...,1,..)) and output is (ni,m)

  * d)
  

* exercise 2.3.2
* exercise 2.3.3
* exercise 2.3.4
* exercise 2.3.5
