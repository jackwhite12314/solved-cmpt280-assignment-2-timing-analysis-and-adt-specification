Download Link: https://assignmentchef.com/product/solved-cmpt280-assignment-2-timing-analysis-and-adt-specification
<br>
The questions on this assignment are about timing analysis and ADT specification. There is no programming on this assignment.

<strong>Question 1 ():</strong>

For each of the following functions, give the tightest upper bound chosen from among the usual simple functions listed in Section 3.5 of the course readings. Answers should be expressed in big-<em>O </em>notation.

<sup>4 </sup>log<sub>280 </sub><em>n </em>+ <u><sup>2</sup></u><sub>42</sub><em><sup>n </sup></em>(a) (1 point) <em>f</em><sub>1</sub>(<em>n</em>) = <em>n </em>log<sub>2 </sub><em>n </em>+ <em>n</em>

<ul>

 <li>(1 point) <em>f</em><sub>3</sub>(<em>n</em>) = 4<em>n</em><sup>4 </sup>+ <em>n</em><sup>2 </sup>log <em>n</em><sup>2 </sup>+ log<sub>2</sub>(2<em><sup>n</sup></em>)</li>

 <li>(1 point) <em>f</em><sub>2</sub>(<em>n</em>) = 4<em>n</em><sup>7 </sup>+ 29<em>n </em>log<sub>2 </sub><em>n </em>+ 280</li>

</ul>

<strong>Question 2 ():</strong>

Suppose the <strong>exact </strong>time required for an algorithm <em>A </em>in both the best and worst cases is given by the function

<em>T<sub>A</sub></em><em>          n</em>

<ul>

 <li>(2 points) For each of the following statements, indicate whether the statement istrue or false.

  <ol>

   <li>Algorithm A is <em>O</em>(log <em>n</em>)</li>

   <li>Algoirthm A is <em>O</em>(<em>n</em><sup>2</sup>)</li>

   <li>Algoirthm A is <em>O</em>(<em>n</em><sup>3</sup>)</li>

   <li>Algoirthm A is <em>O</em>(2<em><sup>n</sup></em>)</li>

  </ol></li>

 <li>(1 point) What is the time complexity of algorithm <em>A </em>in big-Θ notation.</li>

</ul>

<strong>Question 3 ():</strong>

If possible, simplify the following expressions. <em>Hint: See slide 11 of topic 4 of the lecture slides!</em>

<ul>

 <li>(1 point) <em>O</em>(<em>n</em><sup>2</sup>)+ <em>O</em>(log <em>n</em>)+ <em>O</em>(<em>n </em>log <em>n</em>)</li>

 <li>(1 point) <em>O</em>(2<em><sup>n</sup></em>) · <em>O</em>(<em>n</em><sup>2</sup>)</li>

 <li>(1 point) 42<em>O</em>(<em>n </em>log <em>n</em>)+ 18<em>O</em>(<em>n</em><sup>3</sup>)</li>

 <li>(1 point) <em>O</em>(<em>n</em><sup>2 </sup>log<sub>2 </sub><em>n</em><sup>2</sup>)+ <em>O</em>(<em>m</em>) <em>(yes, that’s an ‘m’, not a typo; note that m is independent of n)</em></li>

</ul>

<strong>Question 4 ():</strong>

Consider the following Java code fragment:

<table width="0">

 <tbody>

  <tr>

   <td width="353">// Print out all ordered pairs of numbers for(i = 1; i &lt;= n; i++) { for(j = 1; j &lt;= n; j++) {System.out.println( i + “,␣” + j) ;}}</td>

   <td width="66">between</td>

   <td width="17">1</td>

   <td width="33">and</td>

   <td width="132">n</td>

  </tr>

 </tbody>

</table>

<ul>

 <li>(3 points) Use the <em>statement counting approach </em>to determine the exact number of statements that are executed when we run this code fragment as a function of n. Show all of your calculations.</li>

 <li>(1 point) Express the answer you obtained in part (a) in big-Θ notation.</li>

</ul>

<strong>Question 5 ():</strong>

Consider the following pseudocode:

<table width="0">

 <tbody>

  <tr>

   <td width="601">Algorithm roundRobinTournament(a)This algorithm generates the list of matches that must be played in a round-robin pirate-dueling tournament (a tournament where each pirate duels each other pirate exactly once).a is an array of strings containing names of pirates in the tournamentn = a.length for i = 0 to n-1 for j = i+1 to n-1 print a[i] + “␣duels␣” + a[j] + “,␣Yarrr!”</td>

  </tr>

 </tbody>

</table>

<ul>

 <li>(6 points) Use the <em>statement counting approach </em>to determine the exact number of statements that are executed by this pseudocode as a function of n. Show all of your calculations..</li>

 <li>(1 point) Express the answer you obtained in part a) in big-Θ notation.</li>

</ul>

<strong>Question 6 (3 points):</strong>

Using the active operation approach, determine the time complexity of the pseudocode in question 5. Show all your work and express your final answer in Big-Θ notation.

<strong>Question 7 (6 points):</strong>

Consider the following pseudocode.

<table width="0">

 <tbody>

  <tr>

   <td width="601">Algorithm multiSearch( data, target ):data: an list of arrays of integers; in each array the integers are sorted in ascending order; the list ’data’ has a cursor.target: an integer// Iterate over the arrays in the list ’data’ using // its cursor: data.goFirst() found = false while( !data.after() and !found ) { // search for integer ’target’ in Afound = binarySearch(data.currentItem(), target) data.goForth()</td>

  </tr>

 </tbody>

</table>

Using the active operation approach to timing analysis determine the time complexity of this pseudocode in the worst case. Assume that the list of arrays contains <em>n </em>arrays and that each array has exactly <em>m </em>items in it. Show all your work and express your final answer in Big-<em>O </em>notation.

<strong>Question 8 (17 points):</strong>

A priority queue is a queue where a numeric priority is associated with each element. Access to elements that have been inserted into the queue is limited to inspection and removal of the elements with smallest and largest priority only. A priority queue may have multiple items that are of equal priority.

Give the ADT specification for a bounded priority queue using the specification method described in Topic 7 of the lecture notes. By “bounded”, it is meant that the priority queue has a maximum capacity specified when it is created, and it can never contain more than that number of items.

Your specification must specify the following operations:

<strong>newPriorityQueue: </strong>make a new queue <strong>insert: </strong>inserts an element with a certain priority <strong>isEmpty: </strong>test if the queue is empty <strong>isFull: </strong>test if the queue is full <strong>maxItem: </strong>obtain the item in the queue with the highest priority <strong>minItem: </strong>obtain the item in the queue with the lowest priority <strong>deleteMax: </strong>remove from the queue the item with the highest priority <strong>deleteAllMax: </strong>remove from the queue all items that are tied for the highest priority <strong>deleteMin: </strong>remove from the queue the item with the lowest priority

<strong>frequency: </strong>obtain the number of times a certain item occurs in the queue (with <strong>any </strong>priority)