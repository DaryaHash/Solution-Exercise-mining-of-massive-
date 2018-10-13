# Solution-Exercise(mining-of-massive)

# chapter 2

- [x] ##exercise 2.3.1

  * **a)**
  
  **map:** for each input integer n, define (k,n)-pair that k is constatnt
  then sort (k,ni ) and calculate (k, max (n1,.., nk))
  perpose max(1,...,nk) is nj and calculate hash (k, nj) and send to reduce
  
   **reduce:** in reduce sort again all (k, nj) then calculate (k, max(n1,...,nm))
   and output is (k,nmax)
  
  * **b)**
  
  **map:** for each input integer n, define (k,n)-pair that k is constatnt
  then sort (k,ni) and hash (k,(n1,.., nk)) send to reduce
  
   **reduce:** in reduce sort again all (k,(n1,...,nk))-pairs then calculate (k,avrege(n1,...,nm))
   and output is (k,na verge) 
   
  * **c)**
   
  **map:** for each input integer n, define (n,1)-pair
  then sort (ni,1)-pairs and instate all (ni,1)-pairs that ni is same include just one (ni,1)-pair
  and calculate hash (ni,1)
  send m hash (ni,1) to reduce that m is the number of  pairs with diffrent ni
  
   **reduce :** in reduce sort again all (ni,1)-pair if (ni,1)-pair is same  incude just one
   and output is (ni,1)

  * **d)**
  
  **map:** for each input integer n, define (1,1)-pair
  then calculate (1,(1+1+...+1)) and send hash (1,(1+...+1))
  
   **reduce :** in reduce calculate all (1,(1+...+1+1+...+1+...)) and output is (1,count number)

- [x] **exercise 2.3.2**

**if the data  is to stored memory**

  **map:** matrix M is r×c, M divide to r×t (that c is dividable to t) and Matrix N is c×n, N divide to t×n
  for each part in map task have ((i,k),(M,j,mij)) and ((i,k),(N,j,njk)) for j same calculate ((i,k),mijnjk)
  and hash ((i,k),mijnjk) send to reduce task

  **reduce:** in reduce sort to (i,k) and calculate ((i,k), sum(mijnjk)=pik)
  output is ((i,k),pik)
  
**if the data is not to stored memory**

 **map:** matrix M is r×c divide to v×t (that r&c is dividable to v&t) and Matrix N is c×n divide to t×u
 for each part map task ((i,k),(M,j,mij)) and ((i,k), (N,j,njk) sort to component j then calculate ((i,k),mijnjk)
 and hash ((i,k),mijnjk) send to reduce task

  **reduce:** sort to (i,k) and then calculate ((i,k),sum(mijnjk)=pik)
  output is ((i,k),pik)
  
- [x] **exercise 2.3.3**

  * a)
  
  * b)
  
  * c)

- [x] **exercise 2.3.4**

- [x] **exercise 2.3.5**
