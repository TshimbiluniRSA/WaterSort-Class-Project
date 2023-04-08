# WaterSort-Class-Project

Water Sort Puzzle (WSP) Part 1![image](https://user-images.githubusercontent.com/65872561/230719067-c6edc805-7772-45fd-a820-5de767405743.png)
In Part 1 we do mostly preparation: we are extending the MyArrayList class developed in SU3 and the StackAsArray class of SU5. You need to master the Stacks as Array (SU5 Session 2) before you start.
You also need to master the Water Sort Puzzle game (Android, Apple or Microsoft app stores). Play at least the first 20 levels before you start.

WSP 1: Modifications (2)![image](https://user-images.githubusercontent.com/65872561/230719108-68125918-8c8d-4481-9bcd-27266785db42.png)
Make the following Additions to the StackAsMyArrayList class
As you know you may only use a few actions of a stack: Push and Pop but there is another common one called Peek. Peek returns the value of the top element without removing it. 
You need to create a Peek method:
public E peek() [Make sure you understand the difference between Peek and Pop]
We are going to add 2 non-typical stack methods [just to make this cool game work!]
public int getStackSize()  which calls the getSize() method of the MyArrayList class
public boolean checkStackUniform() which calls the checkUniform() method of the MyArrayList class
HINT: The toString() of the stack class calls the  toString() of the MyArrayList class

WSP 1: Test program (1)![image](https://user-images.githubusercontent.com/65872561/230719148-9189cb86-a7de-4bea-b267-000cbd711769.png)
Create a test class containing a main() method – Call it Watersort
The test program first should create single bottle (StackAsArrayList). 
Create objects of the character glass called red, green and blue.
Use the following type of static variables: 
static Character red= new Character('r'); 
Put ink in the bottles (Push character objects onto the stack) 
Test the getStackSize() and CheckStackUniform() methods thoroughly.

WSP 1: Test program (2)![image](https://user-images.githubusercontent.com/65872561/230719196-d701155f-171e-4112-9742-43d96447bcd3.png)
If you succeeded you are now ready to add more bottles 
Carefully think about the game. Can you see that each bottle is one stack. We need 5 bottles. What type of data structure would you require when you need 5 objects of the same class?

You can either use and array or a linked list. In this case the direct access of an array is much easier to use. So you need an array of 5 bottles. [Call the array bottles]. We are using the simple built-in array of Java NOT our own MyArrayList class. [We want direct access without using accessors and mutators.]

WSP 1: Test program (3)![image](https://user-images.githubusercontent.com/65872561/230719255-3c7b5994-4e9f-4a58-a3a5-f5dff55efc28.png)
If you succeeded you are now ready to display more bottles 
You can add ink to your bottles – take care not to spill ink!
Write a ShowAll() method which displays the content of all the bottles
Fill the bottles with ink to make sure your ShowAll works well! 
Make use of the toString() method in the stack class – remember that because your bottles are in an array you can use a for-loop
![image](https://user-images.githubusercontent.com/65872561/230719271-1bc30dff-ce2a-4e87-a5cb-3ebe21007717.png)

WSP 2: Mix-up ink![image](https://user-images.githubusercontent.com/65872561/230719291-fe876e9b-a9eb-404b-bc73-025435a58950.png)
The aim of Part 2 is to set up the puzzle for the player to solve in Part 3.
There are at least 2 strategies for this. Before you continue think creatively about this. Each of the strategies has advantages and disadvantages.
![image](https://user-images.githubusercontent.com/65872561/230719295-db968c6e-f10c-4c0d-8ef7-adb051df6a33.png)
