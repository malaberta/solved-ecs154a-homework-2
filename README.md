Download Link: https://assignmentchef.com/product/solved-ecs154a-homework-2
<br>
<h1>Problem 1: adder4.circ</h1>

Implement a 4-bit <strong>prefix</strong> adder. The adder you implement must be a <strong>prefix</strong> adder. If you implement any other adder, such as a ripple carry adder, you will <strong>not receive any points.</strong> The automated checking cannot tell the difference between adders so the TAs will look at your submission after the due date to validate that you implemented the correct type of adder. Again, if you did not, you will <strong>not receive any credit for this problem.</strong>




It should go without saying that you cannot use the builtin adder for this problem not only because it would defeat the purpose of this problem but also because it isn’t one of the generally allowed components.

<h2>Inputs</h2>

<table width="624">

 <tbody>

  <tr>

   <td width="208">Pin</td>

   <td width="208">Size (in bits)</td>

   <td width="208">Explanation</td>

  </tr>

  <tr>

   <td width="208">Ain</td>

   <td width="208">4</td>

   <td width="208">The A in A + B</td>

  </tr>

  <tr>

   <td width="208">Bin</td>

   <td width="208">4</td>

   <td width="208">The B in A + B</td>

  </tr>

  <tr>

   <td width="208">Cinin</td>

   <td width="208">1</td>

   <td width="208">The incoming carry bit</td>

  </tr>

 </tbody>

</table>




<h2>Outputs</h2>

<table width="624">

 <tbody>

  <tr>

   <td width="208">Pin</td>

   <td width="208">Size (in bits)</td>

   <td width="208">Explanation</td>

  </tr>

  <tr>

   <td width="208">Sum_Out</td>

   <td width="208">4</td>

   <td width="208">The sum of A + B</td>

  </tr>

  <tr>

   <td width="208">Carry_Out</td>

   <td width="208">1</td>

   <td width="208">The carry coming out of the most significant bit from doing A + B</td>

  </tr>

 </tbody>

</table>




<h1>Problem 2: shifter.circ</h1>

Build a circuit that can logical/arithmetic left/right shift a value a variable amount.

<h2>Additional Components</h2>

For this problem and this problem only, you can also use

<ul>

 <li>Muxes</li>

</ul>

<h2>Inputs</h2>

<table width="624">

 <tbody>

  <tr>

   <td width="208">Pin</td>

   <td width="208">Size (in bits)</td>

   <td width="208">Explanation</td>

  </tr>

  <tr>

   <td width="208">IsRightShiftIn</td>

   <td width="208">1</td>

   <td width="208">If 0 do a left shift. If 1 do a right shift.</td>

  </tr>

  <tr>

   <td width="208">IsArithmeticIn</td>

   <td width="208">1</td>

   <td width="208">If 0 do a logical shift. If 1 do an arithmetic shift</td>

  </tr>

  <tr>

   <td width="208">ShiftAmountIn</td>

   <td width="208">2</td>

   <td width="208">How much to shift NumberIn by</td>

  </tr>

  <tr>

   <td width="208">NumberIn</td>

   <td width="208">3</td>

   <td width="208">The bit string to shift</td>

  </tr>

 </tbody>

</table>




<h2>Outputs</h2>

<table width="624">

 <tbody>

  <tr>

   <td width="208">Pin</td>

   <td width="208">Size (in bits)</td>

   <td width="208">Explanation</td>

  </tr>

  <tr>

   <td width="208">ShiftedNumberOut</td>

   <td width="208">3</td>

   <td width="208">The result of the shift performed on NumberIn</td>

  </tr>

 </tbody>

</table>




<h2>Hints</h2>

<ol>

 <li>Don’t focus heavily on Kmaps for this problem. An easier solution can be found by thinking of this problem at a higher level</li>

 <li>Focus on each bit of the output one by one when trying to find an answer to this problem</li>

 <li>Treat the multi-bit inputs as a bunch of bits instead of as numbers</li>

 <li>Use muxes to solve this problem</li>

</ol>










<h1>Problem 3: bitcounter.circ</h1>

Create a circuit that counts the number of 1’s or 0’s in an 8 bit bit string.




<h2>Additional Components</h2>

For this problem and this problem only, you can also use

<ul>

 <li>All of the components under Plexers</li>

 <li>All of the components under Arithmetic <strong>except</strong> <strong>for Bit Adder</strong></li>

</ul>




<h2>Inputs</h2>

<table width="624">

 <tbody>

  <tr>

   <td width="208">Pin</td>

   <td width="208">Size (in bits)</td>

   <td width="208">Explanation</td>

  </tr>

  <tr>

   <td width="208">BitsIn</td>

   <td width="208">8</td>

   <td width="208">The bit string whose 1’s or 0’s your circuit is to count</td>

  </tr>

  <tr>

   <td width="208">CountZerosIn</td>

   <td width="208">1</td>

   <td width="208">If 0 count the number of 1’s in BitsIn. If 1 count the number of 0’s in BitsIn</td>

  </tr>

 </tbody>

</table>




<h2>Outputs</h2>

<table width="624">

 <tbody>

  <tr>

   <td width="208">Pin</td>

   <td width="208">Size (in bits)</td>

   <td width="208">Explanation</td>

  </tr>

  <tr>

   <td width="208">BitCountOut</td>

   <td width="208">4</td>

   <td width="208">The number of 1’s/0’s in BitsIn</td>

  </tr>

 </tbody>

</table>







<h2>Credit</h2>