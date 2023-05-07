Download Link: https://assignmentchef.com/product/solved-mailing-system-in-c
<br>
For this program, you will modify your program in Part 1 to output a mailing label with a true barcode using <strong>:</strong> for half bars and <strong>|</strong> for full bars. You will also calculate the amount of postage due and replace the word, “Postage” in your mailing label with the exact amount of postage due formatted in dollars and cents. Use the table below to encode each of the digits in your “pseudo” barcode from Part 1. <strong>Note:</strong> do not put spaces between the encoded digits.

<table border="1" cellspacing="0" cellpadding="0" align="left">

 <tbody>

  <tr>

   <td><strong>Value</strong></td>

   <td><strong>Encoding</strong></td>

  </tr>

  <tr>

   <td>1</td>

   <td><strong>:::||</strong></td>

  </tr>

  <tr>

   <td>2</td>

   <td><strong>::|:|</strong></td>

  </tr>

  <tr>

   <td>3</td>

   <td><strong>::||:</strong></td>

  </tr>

  <tr>

   <td>4</td>

   <td><strong>:|::|</strong></td>

  </tr>

  <tr>

   <td>5</td>

   <td><strong>:|:|:</strong></td>

  </tr>

  <tr>

   <td>6</td>

   <td><strong>:||::</strong></td>

  </tr>

  <tr>

   <td>7</td>

   <td><strong>|:::|</strong></td>

  </tr>

  <tr>

   <td>8</td>

   <td><strong>|::|:</strong></td>

  </tr>

  <tr>

   <td>9</td>

   <td><strong>|:|::</strong></td>

  </tr>

  <tr>

   <td>0</td>

   <td><strong>||:::</strong></td>

  </tr>

 </tbody>

</table>

The postage due is based on whether the mailing is a letter, a large envelope or a parcel. Prompt the user for the type of item they are mailing and the weight of the item. Use the following criteria to calculate the postage and display it on the mailing label as shown in the <strong>Sample Output</strong>.

Postage for letters is $0.49 for letters weighing one ounce or less. An additional $0.22 per ounce is added for every ounce (or part of an ounce) over one ounce. For example, a letter that weighs 2.1 ounces will cost $0.49 + (2 * $0.22) = $0.93 to mail.

Postage for large envelopes is $0.98 for envelopes weighing one ounce or less. An additional $0.22 per ounce is added for every ounce (or part of an ounce) over one ounce. For example, a large envelope that weighs 0.5 ounces will cost $0.98 to mail.

Postage for parcels is $2.54 for parcels weighing three ounces or less. An additional $0.20 per ounce is added for every ounce (or part of an ounce) over three ounces. For example, a parcel that weighs 5.5 ounces will cost $2.54 + (3 * $0.20) = $3.14 to mail.

<strong>HINT:</strong> Use the <em>ceil</em> function (http://www.cplusplus.com/reference/cmath/) .

Write your program in such a way that a change in the postage rates would only require you to change the values stored in <strong>named constants</strong> and your program would still work.

<strong>Instructions:</strong>

Write a program that prints a mailing label with all information specified in the <strong>Sample Output</strong>.

Prompt the user for their name, street address, city, state, zip code, type of mailing and weight of item to be mailed.

Encode your “pseudo” barcode into a true bar code .

Using named constants calculate and display the amount of postage on the mailing label formatted in dollars and cents.

Your program’s output should be formatted in the same manner as the <strong>Sample Output</strong>. Make sure that frame bars surround the encoded digits.

After completing all instructions above, add code to randomly generate a 1-digit number that represents the check digit and a 4-digit number that represents the first four digits of a zip code. Using the two random numbers, calculate the value of the fifth zip code digit and then combine the first four digits and your calculated fifth digit to create one number that represents a 5-digit zip code. Overwrite the user’s input stored in your zip code variable with the 5-digit zip code you created. Each time the program is run, a different 1-digit check digit should be generated and a different 4-digit zip code should be generated.<strong>HINT</strong>: You will know that you’ve calculated the missing zip code digit correctly if the value of the check digit in your existing code matches the one you randomly generated.

———————————————————–

Sample Output Part 1:

Enter name : Larry Smith

Enter street address: 122 Main Street

Enter city: Charlotte

Enter state: NC

Enter zip code: 23499

Enter 1 for letter, 2 for envelope, 3 for parcel: 1

Enter weight in ounces: 1.8

——————————————————-

Sample Output Part 2:

**************************$0.71

Larry Smith

122 Main Street

Charlotte     NC 23499

<strong>|</strong><strong>::|:|::||::|::||:|::|:|::::||:</strong><strong>|</strong>