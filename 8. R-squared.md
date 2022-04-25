# R squared Intuition:

### Simple Linear Regression:
Sum (y <sub> i </sub> - y'<sub> i </sub>)<sup> 2 </sup> -> min

this is called the "sum of squared all residuals" SS<sub>res</sub> <br>
Hence,       
> SS<sub>res</sub> = Σ (y <sub> i </sub> - y'<sub> i </sub>)<sup> 2 </sup> <br>

"Total Sum of squares"        
> SS<sub>tot</sub> = Σ (y <sub> i </sub> - y<sub> avg </sub>)<sup> 2 </sup> <br>

### Now R squared is :

> R<sup>2</sup> = 1 -  SS<sub>res</sub> / SS<sub>tot</sub>  
<img src= https://user-images.githubusercontent.com/54764108/165123945-3ed1652d-b343-431b-af41-6c5659cbb744.png width = "230">

 R squared can be negative. but never greater than 1. the closer it is to 1 (lesser the value of SS<sub>res</sub>), the better
 
 ### Adjusted R<sup>2</sup> :
 adding a new independent variable doesnt increase R<sup>2</sup>. (SS<sub>res</sub> decreases)
 
 Adj R<sup>2</sup> = 1 - (1 - R<sup>2</sup>)((n-1) / (n-p-1))
 
 <img src= https://user-images.githubusercontent.com/54764108/165125837-2207f694-70bd-4a4a-a32a-add2f5fbcb37.png width = "380">
 R<sup>2</sup> increases with the number of variabls.
 
