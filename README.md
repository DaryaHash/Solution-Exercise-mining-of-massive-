# Solution-Exercise(mining-of-massive)

## chapter 2
* exercise 2.3.1
  * a)
  **map:** for each input integer n, define (k,n)-pair that k is constatnt
  then each chanck sort (k,ni ) and calculate (k, max (n1,.., nk))
  perpose max(1,...,nk) is nj and calculate hash (k, nj) and send to reduce
  
   **reduce:** in reduce sort again all (k, nj) then calculate (k, max(n1,...,nm))
   and output is (k,nmax)
  
  * b)
  **map:** for each input integer n, define (k,n)-pair that k is constatnt
  then each chanck sort (k,ni) and hash (k,(n1,.., nk)) send to reduce
  
   **reduce:** in reduce sort again all (k,(n1,...,nk))-pairs then calculate (k,avrege(n1,...,nm))
   and output is (k,na verge) 
   
  * c)
  **map:** for each input integer n, define (n ,1)-pair that k is constatnt
  then each chanck sort (n ,1)-pairs and if m pairs similar include just one (n,1)-pair and
  c alculate hash (n,1) that n is diffrent
  send m hash (n,1) to reduce that m is the number of diffrent pairs
  
   **reduce :** in reduce sort again all (n,1)-pairs then if m pairs similar include just one
   pair and output is ((n1,.., nm),1)

  * d)

* exercise 2.3.2
* exercise 2.3.3
* exercise 2.3.4
* exercise 2.3.5
