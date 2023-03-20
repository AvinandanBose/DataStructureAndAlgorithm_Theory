# AlgorithmDesignAndAnalysis

<h1> 1. The Analysis Framework</h1>
<ul>
<h3> <i><ins>A.Time Efficiency:</ins></i> It is also called <i><ins>Time Complexity </ins></i>,It indicates how fast an algorithm runs .</h3>
<h3> <i><ins>B.Space Efficiency:</ins></i> It is also called <i><ins>Space Complexity</ins></i>, refers to amount of memory units required by the algorithm in addition to the space needed for its input and output .</h3>
<ul>
<li><h3> <a href="https://github.com/AvinandanBose/AlgorithmDesignAndAnalysis/blob/main/1.The%20Analysis%20Framework.pdf">1.The Analysis Framework Doc</h3></li>
</ul>
</ul>
<h1> 2. Overview Of Algorithms</h1>
<ul>



```mermaid

flowchart LR
    id1((Agent))
    id1 --> Algorithm
    Input --> Algorithm
    Algorithm --> Output
    
```

<h3> <i><ins>A. Agent:</ins></i> It can be a human or a computer, is the performer. An agent is just something that acts. In terms of computer: Computer operate autonomously, perceive their environment, persist over a prolonged period, adapt to change, and create and pursue goals. A rational agent is one that acts so as to achieve the best outcome or, when there is uncertainty, the best outcome. .</h3>


<h3> <i><ins>B.Algorithm:</ins></i> An algorithm is a sequence of unambiguous for solving a problem, i.e., for obtaining a required output for any legitimate input in a finite amount of time. Algorithm refers to the steps to be carried out in order to accomplish a particular task .</h3>


<h3> Three things to be considered while writing algorithm:<i><ins>Input</ins></i>, <i><ins>process</ins></i>, and <i><ins>output</ins></i>.The input that we give to an algorithm is processed with the of the procedure and finally returns the output. </h3>

<li><h3> <a href="https://github.com/AvinandanBose/AlgorithmDesignAndAnalysis/blob/main/2.Overview%20Of%20Algorithms.pdf">2. Overview Of Algorithms Doc</h3></li> 

<h3><i>Examples : </i></h3>
<ul>
<li><h3>1. Euclid's Algorithm To Find Greatest Common Digit(GCD).</h3></li> 

```Syntax

//English Like Algorithm
Euclid's algorithm for computing GCD(m,n)

Step 1: If n = 0 , return the value of m as the answer and stop; otherwise proceed to Step 2.
Step 2: Divide m by n and assign the value of the remainder to r.
Step 3: Assign the value of n to m and the value to r to n . Go to Step 1.

//Pseudo Code

Euclid (m,n)
//Computes gcd(m,n) by Euclid's algorithm
//Input: Two nonnegative, not both zero integers m and n
//Output: Greatest Common Divisor of m and n

while n ≠ do
  r ← m mod n
  m ← n
  n ← r


```

<ul>

<li><h3> <a href="https://github.com/AvinandanBose/AlgorithmDesignAndAnalysis/blob/main/2.a.Euclid's%20Algorithm%20for%20computing%20gcd(m%2Cn).pdf"> Euclid's Algorithm To Find Greatest Common Digit(GCD) - Algorithm</h3></li>

<li><h3> <a href="https://github.com/AvinandanBose/JavaClassicalDataStructure/blob/main/Euclid.java">Euclid’s Algorithm To Find GCD(m,n) in Java Program[Algorithm Examples]</a></h3></li>

</ul>


<li><h3>2. Consecutive Integer Checking Algorithm  To Find Greatest Common Digit(GCD).</h3></li> 

```Syntax

//English Like Algorithm
Consecutive Integer Checking Algorithm for computing GCD(m,n)

Step 1: Assign the value of min{m,n} to t
Step 2: Divide m by t . If the remainder of this division is 0, 
	go to Step 3; otherwise , go to Step 4. 
	
Step 3: Divide n by t . If  the remainder of this division is 0, 
	return the value of t as the answer and stop; otherwise
	proceed to Step 4.
	
Step 4: Decrease the value of t by 1. Go to Step 2.
	


//Pseudo Code

GCD(m,n):
t←MIN⁡(m,n)
i←0
for i←t to 1 do
  if n mod i=0  And m mod i=0
     STOP
return i

MIN(i , j):
result ←0
if i <j∶
     result ←i
else if j<i:
	result←j
return result

```

<ul>

<li><h3> <a href="https://github.com/AvinandanBose/AlgorithmDesignAndAnalysis/blob/main/2.b.%20Consecutive%20Integer%20Checking%20Algorithm%20%20To%20Find%20Greatest%20Common%20Digit(GCD).pdf"> Consecutive Integer Checking Algorithm  To Find Greatest Common Digit(GCD) - Algorithm</h3></li>

<li><h3> <a href="https://github.com/AvinandanBose/JavaClassicalDataStructure/blob/main/ConsIntCheckAlgo.java">Consecutive Integer Checking Algorithm  To Find Greatest Common Digit(GCD) in JAVA[Algorithm Examples]</a></h3></li>

</ul>


<li><h3>3. Middle School Procedure  To Find Greatest Common Digit(GCD).</h3></li> 

```Syntax

-----------------------------------------------
// English Like Algorithm
----------------------------------------------
Step 1: Find the prime factors of m.
Step 2: Find the prime factors of n.
Step 3: Identify all the common factors in the two prime expansions found in Step 1 and Step 2. 
(If p is a common factor occurring p_m   and p_n  times in m and n ,respectively ,
it should be repeated min⁡{p_m,p_n } times.)

E.g.: 
	60 =  2 ×2 ×3 ×5
	24 = 2×2×2×3
gcd⁡(60,24)=2×2×3=12


-----------------------------------------------
// Pseudo Code
----------------------------------------------

GCD(M,N):
	int IndexA ←0
	int IndexB←0
	int res←1
        Arr1[p]=primeFact(M)
        Arr2[q]=primeFact(N)
       Arr3[n]←NULL
      While(IndexA<p AND IndexB<q):
      
           if(Arr1[IndexA]== Arr2[IndexB]):
                   Arr3[n]←Arr1[IndexA]
                   IndexA←IndexA+1
                   IndexB←IndexB+1
            Else If(Arr1[IndexA]< Arr2[IndexB]) :
                   IndexA←IndexA+1
             Else:
                IndexB←IndexB+1	
  PrimeFact(n):
     Arr1[p]←NULL
        for i ←2 to n-1 do
           while ( n mod i ←0):
            n ← n / i
            Arr1[i]←i
   return Arr1




```



  

<ul>

<li><h3> <a href="https://github.com/AvinandanBose/AlgorithmDesignAndAnalysis/blob/main/2.c.%20Middle%20School%20Procedure%20to%20find%20GCD(m%2Cn).pdf">  Middle School Procedure  To Find Greatest Common Digit(GCD) - Algorithm</h3></li>
<li><h3> <a href="https://github.com/AvinandanBose/JavaClassicalDataStructure/blob/main/MiddleSchoolProc.java">Middle School Procedure To  Find Greatest Common Digit(GCD) in JAVA [Algorithm Examples] </a></h3></li>


</ul>

<li><h3>4.Sieve Of Eratosthenes To Find Prime Numbers.</h3></li>


```Syntax

:Description:

Given a Number N, print all Prime Numbers smaller than or equal to N. 

Process to find out Sieve of Eratosthenes
1.As prime number starts from 2
Therefore mark all multiples of 2 and exclude them.

2.Next prime number will be 3 , 
there fore mark all multiples of 3 and exclude them.

3.And this process will continue till we reach N .


-----------------------------------------------
// English Like Algorithm
----------------------------------------------

Step 1:	First fill an array to True up to N times.
Step 2:	Next Make those multiples of Numbers TO FALSE
Step 3:	Print those Numbers which remains True

----------------
//PSEUDO CODE//
-----------------

Prime(N):
Boolean a[N+1]
for i←2 to N do:
	a[i]←true
for i←2 to N do:
   if (a[i]=True)Then:
      Print(i)
        for j←i*i to n do:
           a[j]←False


```

<ul>

<li><h3> <a href="https://github.com/AvinandanBose/AlgorithmDesignAndAnalysis/blob/main/2.d.%20SieveOFEratosthenes.pdf">  Sieve of Eratosthenes To Find Prime Numbers - Algorithm</h3></li>

<h3><i> Java Programs Solving Sieve of Eratosthenes To Find Prime Numbers </i></h3>
<ul>

<h3> <a href="https://github.com/AvinandanBose/JavaClassicalDataStructure/blob/main/SeiveOfErastosthenes.java">1. Sieve of Eratosthenes To Find Prime Numbers in JAVA(1)[Algorithm Examples]</a></h3>
<h3> <a href="https://github.com/AvinandanBose/JavaClassicalDataStructure/blob/main/SieveOfErastothenes1.java">2. Sieve of Eratosthenes To Find Prime Numbers in JAVA(2)[Algorithm Examples] </a></h3>
<h3> <a href="https://github.com/AvinandanBose/JavaClassicalDataStructure/blob/main/sieveOfEratosthenes.java">3. Sieve of Eratosthenes To Find Prime Numbers in JAVA(3)[Algorithm Examples] </a></h3>

</ul>


</ul>

</ul>




</ul>

<h1> 3. Ways of Writing an Algorithm</h1>
<ul>
<h3> There are various ways of writing an algorithm. </h3>
    <ul>
        <li><h3> 1.<ins>English-Like Algorithm</ins></h3></li> 
        <ul>
            <h3><i><ins>Eg:</ins></i></h3>
            
```Syntax

Algorithm : English – like algorithm of linear search.
	
Step 1: Compare `item` with the first element of the array, A.
Step 2: If the two are same, then print the position of the element and exit.
Step 3: Else repeat the above process with the rest of the elements.
Step 4: If the item is not found at any position, then print ‘not found’ and exit.

```

<h3> Disadvantage:</h3>
<ul>
<li><h3> 1.Natural Languages can be ambiguous and therefore its lack the characteristics of being definite.</h3></li> 
<li><h3> 2.English language-like algorithms are not considered good for most of the task.</h3></li> 
</ul>
            
</ul>

<li><h3> 2.<ins>Flow Chart</ins></h3></li> 
<ul>
<h3> Flowcharts pictorially depict a process. They are easy to understand and are commonly used in the case of simple problems.</h3> 
</ul>
<li><h3> 3.<ins>Pseudo-code.</ins></h3></li> 
<ul>
<h3>An artificial and informal language constituting of notations helps in resembling a simplified programming language, used in program design. This way of writing algorithm is most acceptable and most widely used.</h3> 
</ul>
</ul>
<ul>
<li><h3> <a href="https://github.com/AvinandanBose/AlgorithmDesignAndAnalysis/blob/main/3.Ways%20of%20Writing%20An%20Algorithm.pdf">3. Ways Of Writing Algorithms Doc[with Full Description]</h3></li> 

</ul>
</ul>
<h1> 3. Some Mathematical Concepts</h1>
<ul>
<h3> Prior going with the analysing part of the Programming concept , one must have clear understanding  on :</h3>
<ul>
.....
</ul>



</ul>

<h1> 4. Rate of Growth</h1>
<ul>

<h3>The <i>Rate Of Growth</i> helps to find the behavior of an Algorithm. The rate at which the running time increases as a function of input is called <i>Rate Of Growth</i>.The <i>Rate Of Growth Of An Algorithm</i> is the rate at which its running time increases as a function of input <i>‘n’</i>. </h3>
<ul>
 <h3><li><a href="https://github.com/AvinandanBose/AlgorithmDesignAndAnalysis/blob/main/Rate%20of%20Growth.pdf"> Rate of Growth -In Details</li></h3>
</ul>


</ul>

<h1> 5.Algorithm Classes / Commonly Used Rates of Growth</h1>
<ul>

<Table>
<tr>
<th>Function Name</th>
<th>Name used for algorithm analysis</th>
<th>Remarks</th>	
</tr>
	
<tr>
<td> c</td>
<td>Constant Algorithm</td>
<td>These algorithms are independent of the input.</td>	
</tr>
	
<tr>
<td> Log log N</td>
<td>Log log⁡ function</td>
<td>Logarithmic algorithms are preferred, as their growth is always low.</td>	
</tr>
	
	
<tr>
<td> Log N</td>
<td>logarithmic</td>
<td>These are very optimal algorithms.</td>	
</tr>
	
<tr>
<td> Log^2 N</td>
<td>Log-squared</td>
<td>These are optimal algorithms.</td>	
</tr>
	
<tr>
<td> N</td>
<td>Linear algorithm</td>
<td>Linear algorithms are preferred, e.g., summing of an array.</td>	
</tr>
	
<tr>
<td> N^2</td>
<td>Quadratic</td>
<td>Sorting algorithms are preferred, e.g., bubble sort, selection sort.</td>	
</tr>
	
<tr>
<td> N^3</td>
<td>Cubic</td>
<td>Matrix multiplication is preferred.</td>	
</tr>
	
<tr>
<td> N^k</td>
<td>Polynomial</td>
<td>Polynomial algorithms of lesser order k are preferred.</td>	
</tr>
	
<tr>
<td> a^n</td>
<td>Exponential</td>
<td>Here a is constant, and intractable algorithms are exponential.</td>	
</tr>
	
<tr>
<td> N!</td>
<td>Factorial</td>
<td>These algorithms are intractable.</td>	
</tr>
	
	
	
</Table>
	
 <h3><li><a href="https://github.com/AvinandanBose/AlgorithmDesignAndAnalysis/blob/main/5.Comparison%20Framework.pdf"> Algorithm Classes / Commonly Used Rates of Growth</li></h3>
</ul>

<h1> 6.RELATIONSHIP BETWEEN DIFFERENT RATES OF GROWTH</h1>

<ul>


```mermaid

flowchart TD

    id1((2^2n))
    id2((n!))
    id3((4^n))
    id4((n^2))
    id5((nlogn))
    id6((logn!))
    id7((n))
    id8((2^logn))
    id9((log log n))
    id10((1))
    
  
    id1 --> id2
    id2 --> id3
    id3 --> id4
    id4 --> id5
    id5 --> id6
    id6 --> id7
    id7 --> id8
    id8 --> id9
    id9 --> id10
      
    
```

<h3 align="Center"> <i> The above Diagram shows decreasing rates of growth. </i></h3>

<h3> <li><a href="https://github.com/AvinandanBose/AlgorithmDesignAndAnalysis/blob/main/6.Relationship%20between%20different%20rates%20of%20growth.pdf"> Relationship between different rates of growth - In Details </a> </li></h3>

</ul>

<h1>7.Need for Analysing Algorithm </h1>
<ul>

<h3><i>It is reasonable to measure an algorithm’s efficiency as a function of a parameter indicating the size of the algorithm’s input. But there are many algorithms for which running time depends not only on an input size but also on the specifics of a particular input.</i></h3>

<ul>
<ul>
<h3><li> It is logical to assume that the efficiency of algorithms depends solely on the input size n.</li></h3> 

<h3><li> Efficiency of an algorithm also depends upon the distribution of input data as well.</li></h3> 
</ul>
</ul>

<h3><i> Hence we represents the algorithm with multiple expressions:</i></h3>

<ul>
<ul>
<h3><li> One for the case where it takes less time: <ins><i>Best Case.</i></ins></li></h3> 

<h3><li> Another for the case where it takes more time: <ins><i>Worst Case.</i></ins></li></h3> 
<h3><li> And there is another case where input is random and number of trials taken gives an average runtime , hence we get the third case : <ins><i>Average Case.</i></ins></li></h3> 
</ul>

</ul>
<h3><i>And to analyse an algorithm, we need some kind of syntax and that forms the base for <ins>Asymptotic Analysis/Notation.</ins></i></h3>

<ul>
<ul>

<h3><li> <a href="https://github.com/AvinandanBose/AlgorithmDesignAndAnalysis/blob/main/7.Need%20for%20Analysing%20Algorithm.pdf"> Need For Analysing Algorithm - In Details </li></h3>

<ul>
<h3> <a href="https://github.com/AvinandanBose/JavaClassicalDataStructure/blob/main/java_sequential_Search.java">1. Sequential Search using while loop </a><h3>

```Syntax

ALGORITHM: SEQUENTIAL SEARCH ( 𝑨[𝟎. . 𝒏 − 𝟏], 𝑲 ) 
//Searches for a given value in each array by sequential Search 
//Input: An array A[0..n-1] and a search key K 
//Output: The index of the first element in A that matches K 
// or -1 if there are no matching elements. 
𝟏 ← 𝟎 
while 𝒊 < 𝒏 and A[i] ≠ 𝑲 𝒅𝒐 
       𝒊 ← 𝒊 + 𝟏 
if  𝒊 < 𝒏 𝒓𝒆𝒕𝒖𝒓𝒏 𝒊 
𝒆𝒍𝒔𝒆 𝒓𝒆𝒕𝒖𝒓𝒏 − 𝟏 

```

<h3> <a href="https://github.com/AvinandanBose/JavaClassicalDataStructure/blob/main/java_sequential_Search1.java">2. Sequential Search using for loop</a></h3>
<h3> <a href="https://github.com/AvinandanBose/JavaClassicalDataStructure/blob/main/java_sequential_Search2.java">3. Sequential Search using Recursion</a></h3>

</ul>
</ul>

</ul>
</ul>

<h1>8.Types of Analysis </h1>
<ul>

<ul>
<h3><ins>1. Worst Case Complexity And UpperBound :</ins>The worst-case efficiency of an algorithm is its efficiency for the worst-case input of size n , which is an input (or inputs) of size n, for which the algorithm runs the longest among all possible inputs of that size.</h3>
<ul>
<h3><ins>1.a.Upper Bound :</ins>The upper bound of an algorithm  is the measure of the maximum computational effort required to solve a given problem.</h3>
</ul>



</ul>

<ul>
<h3><ins>2. Best Case Complexity and Lower Bound :</ins>The best-case efficiency of an algorithm is its efficiency for the best-case of size n, which is an input( or inputs) of size n for which  the algorithm runs fastest among all possible inputs of that size.</h3>
<ul>
<h3><ins>2.a.Lower Bound :</ins>The Lower Bound of an algorithm  is the measure of the minimum computational effort required to solve a given problem.</h3>
</ul>

</ul>

<ul>
<h3><ins>3. Average-case Complexity :</ins>The average-case analysis assumes that the input is random and provides prediction about the running time of an algorithm for a random input.</h3>

</ul>

</ul>
