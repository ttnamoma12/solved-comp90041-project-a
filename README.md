Download Link: https://assignmentchef.com/product/solved-comp90041-project-a
<br>
<h1>1        Nim: A Game of Strategy</h1>

This project is the first in a series of three, with the ultimate objective of designing and implementing a simple variant of the game of Nim in Java. Nim is a two-player game, and the rules of the version used here are as follows:

<ul>

 <li>The game begins with a number of objects (<em>g.</em>, stones placed on a table).</li>

 <li>Each player takes turns removing stones from the table.</li>

 <li>On each turn, a player must remove at least one stone. In addition, there is an upper bound on the number of stones that can be removed in a single turn. For example, if this upper bound is 3, a player has the choice of removing 1, 2 or 3 stones on each turn.</li>

 <li>The game ends when there are no more stones remaining. The player who removes the last stone, loses. The remaining player wins.</li>

 <li>Both the initial number of stones, and the upper bound on the number that can be removed, can be varied from game to game, and must be chosen before a game commences.</li>

</ul>

<h2>1.1       Example Gameplay</h2>

Here is an example play-through of the game, using <strong>12 initial stones</strong>, and an <strong>upper bound of 3 stones </strong>removed per turn:

<ul>

 <li><em>12 stones on the table.</em></li>

 <li><em>Player 1 removes 3 stones. 9 stones remain.</em></li>

 <li><em>Player 2 removes 1 stone. 8 stones remain.</em></li>

 <li><em>Player 1 removes 1 stone. 7 stones remain.</em></li>

 <li><em>Player 2 removes 2 stones. 5 stones remain.</em></li>

 <li><em>Player 1 removes 3 stones. 2 stones remain.</em></li>

 <li><em>Player 2 removes 1 stone. 1 stone remains.</em></li>

 <li><em>Player 1 removes 1 stone. 0 stones remain.</em></li>

 <li><em>Player 2 wins.</em></li>

</ul>

<h1>2        Assignment: Implement Nim’s Basic Game Mechanics</h1>

For this first project, the focus will be on creating two players and playing for multiple games:

<ol>

 <li>Your program will begin by displaying a welcome message.</li>

 <li>The program will then prompt for a string (no space in the string) to be entered via standard input(the keyboard) – this will be the name of Player 1. You may assume that all inputs to the program will be valid.</li>

 <li>The program will then prompt for another string (no space in the string) to be entered – this will bethe name of Player 2.</li>

 <li>The program will then prompt for an integer to be entered – this will be the upper bound on thenumber of stones that can be removed in a single turn.</li>

 <li>The program will then prompt for another integer to be entered – this will be the initial number ofstones.</li>

 <li>The program will then print the number of stones, and will also display the stones, which will berepresented by asterisks ‘*’.</li>

 <li>The program will then prompt for another integer to be entered – this time, a number of stones to beremoved. Again, you may assume this input will be valid and will not exceed the number of stones remaining or the upper bound on the number of stones that can be removed.</li>

 <li>The program should then show an updated display of stones.</li>

 <li>The previous two steps should then be repeated until there are no stones remaining. When thisoccurs, the program should display ‘Game Over’, and the name of the winner.</li>

 <li>The program should then ask user whether the players wanted a play again. The user is promptedto enter ‘Y’ for yes or ‘N’ for no. If the user enters ‘Y’, that is, the user wants to play another game, repeat steps 4-10. Otherwise, the program should terminate. Note, any input apart from ’Y’ should terminate the game.</li>

</ol>

<h2>2.1       Example Execution</h2>

After executing your program, the flow should be something like this:

Welcome to Nim

Please enter Player 1’s name:

Luke

Please enter Player 2’s name: Han

Please enter upper bound of stone removal:

3

Please enter initial number of stones:

12

12 stones left: * * * * * * * * * * * *

Luke’s turn – remove how many? 3

9 stones left: * * * * * * * * *

Han’s turn – remove how many? 1

8 stones left: * * * * * * * *

Luke’s turn – remove how many? 1

7 stones left: * * * * * * *

Han’s turn – remove how many? 2

5 stones left: * * * * *

Luke’s turn – remove how many? 3

2 stones left: * *

Han’s turn – remove how many? 1

1 stones left: *

Luke’s turn – remove how many? 1

Game Over Han wins!

Do you want to play again (Y/N):

Y

Please enter upper bound of stone removal: 5

Please enter initial number of stones: 15

15 stones left: * * * * * * * * * * * * * * *

Luke’s turn – remove how many? 1

14 stones left: * * * * * * * * * * * * * *

Han’s turn – remove how many?

2

12 stones left: * * * * * * * * * * * *

Luke’s turn – remove how many? 3

9 stones left: * * * * * * * * *

Han’s turn – remove how many? 4

5 stones left: * * * * *

Luke’s turn – remove how many? 5

Game Over Han wins!

Do you want to play again (Y/N):

N

<h2>2.2       Some Hints</h2>

Please note that:

<ul>

 <li>You need to create a class called Nimsys with a main() method to manage the above game playing process.</li>

 <li>When a player’s name is entered, a new object of the NimPlayer class should be created. You need to create the class NimPlayer. Player 1 and Player 2 are two instances of this class. This class should have a String typed instance variable representing the player name. This class should also have a removeStone() method that returns the number of stones the player wants to remove in his/her turn. You will lose marks if you fail to create two instances of NimPlayer.</li>

 <li>Add other variables and methods where appropriate such that the concept of information hiding and encapsulation is reflected by the code written.</li>

 <li>There is <strong>NO </strong>blank line before the first line, i.e., no println() before ‘Welcome to Nim’.</li>

 <li>There is a withespace between stones left : sentence and * * *, and also between all * * *, but <strong>NO </strong>withespace at the end of * * *.</li>

 <li>The line that prints the winners name should be <strong>a full line</strong>, i.e., ‘Han wins!’ is printed out using println().</li>

 <li>And there are <strong>NO </strong>blanks after the last stone in lines displaying asterisks.</li>

 <li>Keep a good coding style.</li>

</ul>

You do not need to worry about changing your output for singular/plural entities, i.e., you should output ‘1 stones’, etc.

<h1>3        Important Notes</h1>

Computer automatic test will be conducted on your program by automatically compiling, running, and comparing your outputs for several test cases with generated expected outputs. The automatic test will deem your output wrong if your output does not match the expected output, even if the difference is just having an <strong>extra space or missing a colon</strong>. Therefore it is crucial that <strong>your output follows exactly the same format shown in the examples above.</strong>

The syntax import is available for you to use standard java packages. However, please <strong>DO NOT </strong>use the package syntax to customize your source files. The automatic test system cannot deal with customized packages. If you are using Netbeans as the IDE, please be aware that the project name may automatically be used as the package name. Please remove the line like package ProjA; at the beginning of the source files before you submit them to the system.

Please use <strong>ONLY ONE </strong>Scanner object throughout your program. Otherwise the automatic test will cause your program to generate exceptions and terminate. The reason is that in the automatic test, multiple lines of test inputs are sent all together to the program. As the program receives the inputs, it will pass them all to the currently active Scanner object, leaving the rest Scanner objects nothing to read and hence cause run-time exception. Therefore it is crucial that <strong>your program has only one Scanner object. </strong>Arguments such as “It runs correctly when I do manual test, but fails under automatic test” will not be accepted.

<h1>4        Assessment</h1>

This project is worth 10% of the total marks for the subject.

Your Java program will be assessed based on correctness of the output as well as quality of code implementation. See Canvas for a detailed marking scheme.

<h1>5        Test Before Submission</h1>

You will find the sample input file and the expected ouput file in the Projects page on LMS for you to use on your own. You should use them to test your code on your own first, and then submit your code. Note that you must submit your code through the submit system in order to make a valid submission of the project, details of submit system can be found in Section 6. To test your code by yourself:

<ol>

 <li>Upload to the server your Java code files named “java” and “NimPlayer.java”, and the test input data files “test0.txt”.</li>

 <li>Run command: javac *.java (this command will compile all your java file in the current folder)</li>

 <li>Run command: java Nimsys &lt; test0.txt &gt; output.txt (this command will run the Nimsys using contents in ‘txt” as input and write the output in output.txt)</li>

 <li>Run command: more output.txt (this command will show the your program’s output)</li>

 <li>Compare your result with the provided output file test0-output.txt. Fix your code if they are different.</li>

 <li>When you are satisfied with your project, submit and verify your project using the instructions givenin the Section 6.</li>

</ol>

<strong>NOTE: </strong>The test cases used to mark your submissions will be different from the sample tests given. You should test your program extensively to <strong>ensure it is correct for other input values </strong>with the same format as the sample tests.