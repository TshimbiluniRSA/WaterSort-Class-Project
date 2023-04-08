# WaterSort-Class-Project

Water Sort Puzzle (WSP) Part 1

In Part 1 we do mostly preparation: we are extending the MyArrayList class developed in SU3 and the StackAsArray class of SU5. You need to master the Stacks as Array (SU5 Session 2) before you start.
You also need to master the Water Sort Puzzle game (Android, Apple or Microsoft app stores). Play at least the first 20 levels before you start.

WSP 1: Modifications (2)

Make the following Additions to the StackAsMyArrayList class
As you know you may only use a few actions of a stack: Push and Pop but there is another common one called Peek. Peek returns the value of the top element without removing it. 
You need to create a Peek method:
public E peek() [Make sure you understand the difference between Peek and Pop]
We are going to add 2 non-typical stack methods [just to make this cool game work!]
public int getStackSize()  which calls the getSize() method of the MyArrayList class
public boolean checkStackUniform() which calls the checkUniform() method of the MyArrayList class
HINT: The toString() of the stack class calls the  toString() of the MyArrayList class

WSP 1: Test program (1)

Create a test class containing a main() method – Call it Watersort
The test program first should create single bottle (StackAsArrayList). 
Create objects of the character glass called red, green and blue.
Use the following type of static variables: 
static Character red= new Character('r'); 
Put ink in the bottles (Push character objects onto the stack) 
Test the getStackSize() and CheckStackUniform() methods thoroughly.

WSP 1: Test program (2)

If you succeeded you are now ready to add more bottles 
Carefully think about the game. Can you see that each bottle is one stack. We need 5 bottles. What type of data structure would you require when you need 5 objects of the same class?

You can either use and array or a linked list. In this case the direct access of an array is much easier to use. So you need an array of 5 bottles. [Call the array bottles]. We are using the simple built-in array of Java NOT our own MyArrayList class. [We want direct access without using accessors and mutators.]

WSP 1: Test program (3)

If you succeeded you are now ready to display more bottles 
You can add ink to your bottles – take care not to spill ink!
Write a ShowAll() method which displays the content of all the bottles
Fill the bottles with ink to make sure your ShowAll works well! 
Make use of the toString() method in the stack class – remember that because your bottles are in an array you can use a for-loop


WSP 2: Mix-up ink

The aim of Part 2 is to set up the puzzle for the player to solve in Part 3.
There are at least 2 strategies for this. Before you continue think creatively about this. Each of the strategies has advantages and disadvantages.

