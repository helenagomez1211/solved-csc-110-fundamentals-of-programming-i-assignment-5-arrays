Download Link: https://assignmentchef.com/product/solved-csc-110-fundamentals-of-programming-i-assignment-5-arrays
<br>
<h1>Learning outcomes</h1>

When you have completed this assignment, you should understand:

<ul>

 <li>How to pass <em>parameters</em> and <em>return</em> values using static</li>

 <li>How to use</li>

 <li>How to <em>indent </em>and<em> document</em> a Java program.</li>

</ul>

An important task in bioinformatics is the identification of DNA and RNA sequences. In this assignment we will be looking at <em>nucleic acid sequences.</em> These <em>sequences</em> contain up to four different <em>bases</em> denoted by letters: <em>A</em> for <em>adenine</em>, <em>C</em> for <em>cytosine</em>, <em>G</em> for <em>guanine</em>, and <em>T</em> for <em>thymine</em>. <em> Sequence </em>strings are compared in order to determine whether <em>nucleic acid sequences</em> match each other, or are related through <em>mutations</em>. Real sequence data as used by biochemists and in bioinformatics research consist of very long strings of <em>A</em>, <em>C</em>, <em>G</em> and <em>T</em>. Determining relatedness can require the use of very complex algorithms, beyond the scope of this assignment.

The <em>sequence</em>s in this assignment will all contain between 2 and 4 of the possible <em>bases</em> (<em>A,</em> <em>C</em>, <em>G</em>, and <em>T</em>). Your task is to search through a collection of sequence data and count how many times a specific <em>sequence</em> occurs. (For example, if the collection contains the following sequences: {<em>ACTG</em>, <em><u>GATC</u>, ACT, GTC, AC, <u>GATC</u>, GA</em>} and we search for the specific sequence <em>GATC</em> we would report that it was found 2 times.

One of the difficulties in this assignment will be dealing with <em>mutated sequences</em>. A <em>mutation</em> can occur due to insertions of additional <em>bases</em> within a <em>sequence</em>. For the purpose of this assignment, a <em>mutated sequence </em>contains at least two of the same <em>bases</em> occurring in a row (so in the sequence <em>GAAATC</em> the <em>A</em> has <em>mutated</em>, and in the sequence <em>CCGGAT</em> both the <em>C</em> and <em>G</em> have <em>mutated</em>). Another task in this assignment is to detect how many of the <em>sequences</em> in the collection are <em>mutated</em>. The final task will be to search through the collection of sequence data for a specific <em>sequence</em>, but you must treat original and <em>mutated sequences</em> the same (For example, if the collection contains {<em><u>TGC</u>, AC, <u>TTGC</u>, TACG, <u>TGGCC</u>, AGTC</em>} and we search for the specific sequence <em>TGC</em> we would report that it was found 3 times (because <em>TTGC</em> and <em>TGGCC</em> are mutated forms of <em>TGC</em>).

<h1>Recommended steps to follow in order</h1>

<ol>

 <li>Similar Assignment 4, the <a href="https://connex.csc.uvic.ca/access/content/group/c695ec2f-7536-40a4-8ddc-eec4c5c20d41/Assignment%20Resources/Assignment5/SearchDNA.html">specification document</a> outlines all of the required methods for this assignment. Appendix A illustrates some examples of how to call and test the methods in your SearchDNA.java program.</li>

 <li>The printArray method is a nice place to start. Focus on passing in an array of Strings as a parameter and using a loop to visit each element in the array. Remember that array indexes start at 0 (similar to Strings)!</li>

 <li>After finishing printArray, we recommend working on the findLongest or the findFrequency methods, as they are quite similar. Within both methods, a loop should be created to visit each element in the array. In the findLongest method, you must keep track of which String in the array contains the most characters, whereas in the findFrequency method, you must keep track of how many times a specific String is found in the array.  Make sure you finish and test them both before moving to the next step.</li>

 <li>The methods involving mutations are a little more difficult. In this assignment, a mutation occurs when two or more characters in a String are repeated in a row. Think about how you might be able to detect a mutation in a String. Once you come up with a strategy, test it with a number of Strings to see if it works!</li>

</ol>

<strong> </strong>

<h1>Marking</h1>

Your mark will be based on the following criteria:

<ul>

 <li>Your code <em>must compile and run</em>. Some examples of how to test your methods, along with expected output, are outlined in <strong>Appendix A.</strong></li>

 <li>Your code must conform to all the requirements mentioned in the <a href="https://connex.csc.uvic.ca/access/content/group/c695ec2f-7536-40a4-8ddc-eec4c5c20d41/Assignment%20Resources/Assignment5/SearchDNA.html">specification document</a><a href="https://connex.csc.uvic.ca/access/content/group/c695ec2f-7536-40a4-8ddc-eec4c5c20d41/Assignment%20Resources/Assignment5/SearchDNA.html">.</a></li>

 <li>The main method must show all of your testing code. Each of the required methods should be tested.</li>

 <li>Your code must follow the guidelines outlined in Style_Guidelines.pdf, found through the Lectures &amp; Stuff link in the Lab Resources folder on connex. You may notice that the specification document provides some very nice comments you are welcome to borrow.</li>

</ul>

<h1><u>Appendix A – Testing your code</u></h1>

As you work through a solution, it is recommended that you save, compile and test your code after every line or two of code that you write. This can be something as easy as printing out the value of a variable, or calling a method to print out the value returned. It is important to do this to confirm a component of your code works correctly, so you can be confident using that component throughout your code later.




<strong>Testing the </strong><em>printArray</em><strong> method: </strong>

One way to do this is to create an array of Strings in the main method and then call the <strong>printArray</strong>  method from main. An example is shown below:




<em>findLongest</em> <strong>method: </strong>

One way to do this is to create an array of Strings in the main method and then call the <strong>longestWord  </strong>method from main, assign the value returned by the method to a  String variable, and print out the word.

<em>findFrequency </em><strong> method: </strong>

<strong>findFrequency  </strong>method from main passing in the String and the

array as parameters, assign the value returned by the method to an int variable, and print out the value of the integer. (Matches are underlined in red)

<em>countTotalMutations </em><strong>method: </strong>

<strong>countTotalMutations </strong>method from main passing in the String

array as a parameter, and then assign the value returned by the method to an int variable, and print out the value of the integer.

Remember that in this assignment, a<em> mutation </em>occurs when any <em>base</em> is repeated twice in a row. So, the sequences <em>TAG</em> and <em>ACTA</em> are not mutations, but the sequences <em>TGGGGAA</em> and <em>AATTCCGG</em> are. In the example below, Strings including one or more mutations are underlined in red.

<em>findFreqWithMutations </em><strong>method: </strong>

<strong>findFreqWithMutations </strong>method from main passing in the String

and the array as parameters, assign the value returned by the method to an int variable, and print out the value of the integer.

Remember that in this assignment, a <em>mutation</em> occurs when any <em>base</em> is repeated twice in a row. So, removing the mutations from <em>TGGGGAA</em> would result in <em>TGA</em>. The sequences found to be matches when searching through the array including mutations are underlined in red.







<h2>Extra challenge – Testing with real data from a file</h2>

On the connex page, under Lectures &amp; Stuff &gt; Assignment Resources &gt; Assignment5, there are text files containing a collection of <em>sequences</em> that you can further test your program with. Also in the folder is a java program, FileToArrayExample.java. It contains code to read data from a file and place it into an Array of strings.  Feel free to copy the method arraySetup found in FileToArrayExample.java and use it in your own program to further test your methods.

The arraySetup method can be used to fill the array with sequence data using any of the text files, which have been created to be used in this assignment. All of the text files contain a different sets of <em>sequences</em> with varying amounts of mutations:

<ul>

 <li>txt – 5 sequences, without mutations</li>

 <li>txt – 25 sequences, without mutations</li>

 <li>txt – 20 sequences, few mutations</li>

 <li>txt – 50 sequences, few mutations</li>

 <li>txt – 20 sequences, many mutations</li>

 <li>txt – 100 sequences, many mutations</li>

 <li>txt – 1000 sequences, many mutations</li>

 <li>txt – 10000 sequences, many mutations</li>

</ul>

Below is an example of how we might use an input file to read in a collection of sequences, ask a user to search for a specific sequence, and output the results.


