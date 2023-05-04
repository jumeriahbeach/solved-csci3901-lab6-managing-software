Download Link: https://assignmentchef.com/product/solved-csci3901-lab6-managing-software
<br>
In this lab, you will explore managing a system of software with test suites via JUnit and build management with Make. you will apply your knowledge of JUnit and Makefiles to write a test script for the newest release of the HfxDonairExpress online ordering system, to improve their build automation, and to include your test cases in their existing testing setup.

<strong>Preparation</strong>

<ul>

 <li>Download and install GNU Make. You can alternatively use it on timberlea.</li>

</ul>

<h1>Procedure</h1>

<strong>Set-up</strong>

<ol>

 <li>Download and unzip the source directory posted on Brightspace.</li>

</ol>

<strong>Lab steps</strong>

<strong>Part 1 – Unit Testing </strong>Write a JUnit test suite for HfxDonairExpress, with <strong>one test method for each </strong>of the following cases. You should put these test cases in a file called UnitTests.java. Your test cases should check that the method in question (either order or makeOrder) returns the correct value.

<ol>

 <li>order method: Ordering a small donair</li>

 <li>order method: Ordering a large donair with the coupon code “YOLO5”</li>

 <li>order method: Ordering a medium pizza with pepperoni and mushrooms</li>

 <li>makeOrder method: Making 1 order</li>

 <li>makeOrder method: Making 2 orders in a row</li>

</ol>

1

<strong>Part 2 – Understanding Makefiles             </strong>Answer the following questions about the provided Makefile:

<ol>

 <li>Which file(s) are included in the SRC variable?</li>

 <li>What file(s) does the all target depend on?</li>

 <li>What is the command used to make the jar file?</li>

 <li>What does the test target do? You may want to try running the command make test to see.</li>

</ol>

<strong>Part 3 – Writing Makefiles              </strong>Add the following features to the existing Makefile:

<ol>

 <li>Modify the Makefile so that your unit test class is compiled and included in jar</li>

 <li>Modify the Makefile to put the compiled .html documentation files into a new sub-directory, docs</li>

 <li>Modify the Makefile to include a target clean which deletes the compiled .class and .html Note: the rm command can be used to delete a file</li>

</ol>

<h1>Questions</h1>

<ol>

 <li>Why is it important to have a portable, reproducible build system that isn’t tied to a particular IDE?</li>

 <li>How often should you run a class’ test suite when developing a software system? Explain.</li>

 <li>Can you see any reason to split test cases up into separate files, or should you just include all of your test cases for every class in the same file?</li>

</ol>