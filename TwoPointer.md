I have seen two types of questions that occur in 2pointer

type 1 ->

FFFFFFFFTTTTTTFFFFFFFFFF

for a fixed i we are trying to find the j such that i and j shall contain all the Trues.
In case of counting think of this.


### Think about it more and add the questions.

type 2 ->

We are finding a pair simultaneously for a T.

Example# fixed value of the pair.










---------------------------------------
Imp thing so that I dont get stuck again;
https://codeforces.com/contest/1324/problem/D
In this problem this technique may look good but it will not work -
        for(ll i = 0; i< n-1; i++){
            j = max(i+1,j);
            while(j<n && v[i]+v[j]<=0)
                j++;
            ans += n-j;
        }
The core reason for that is, for one i the j will be i + x, however for i+1 it is not neccesary that the ans i + y will be having y>x  
    
