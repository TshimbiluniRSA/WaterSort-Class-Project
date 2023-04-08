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

WSP 2: Mix-up ink: Strategy 1

IMPORTANT NOTE: We are not going to start with 2 empty bottles, but rather with 8 empty slots spread over the 5 bottles as explained in the intro video.
Start with 5 empty bottles. Use a random number generator to fill bottles one slot at a time with the colours while keeping 8 slots empty – there is a total of 5*4 = 20 slots – so if we will 12 slots, 8 are free.
Advantage: Easy to create a puzzle with a good mix
Disadvantage: With more colours and  bottles and only 2 open bottles for more advanced versions of the game, the result might not be solvable.

WSP 2: Mix-up ink: Strategy 2

Start with three sorted bottles. In the strategy the idea is to load three bottles with uniform colour and then move ink around for a number of moves until the bottles are mixed up.
Advantage: Result is always solvable since the bottles are created in a reversed-game	strategy.
Disadvantage: It is hard to develop an algorithm which will reach the bottoms of the bottles. We tried this by moving on item from every bottle in rounds. But it still took more than 100 moves to obtain a good mix in the bottles.

WSP 2: Implement any strategy

You need to extend your WaterSort program to implement one of these strategies. It is a good idea to play around with both – please use Random numbers in both cases.
Important: To add ink to a bottle (strategy 1) or to move ink from one bottle to another (strategy 2) or you need to use the stack operators.
You need to ensure that you are not spilling ink! (now you understand why you needed the getSize()) method in Part 1.

You only need to submit one of the two strategies. Your program should have output of 5 scrambled bottles.

WSP 3: Playing the game (1)

We are not going to spoil your fun by providing you with all the detail!
To start off: create a method called
	public static boolean solved( StackAsMyArrayList bottles[])
    Which checks if a the game is solved.
Watch the Introductory Video again – there are a large number of special cases to check – before you move ink from one bottle to another. (Remember the difference between Peek and Pop


WSP 3: Playing the game (2)

When you have the basic game working, you can try implement finer rules such as that one that if there is enough space  in the target bottle and the source bottle has 2 adjacent similar colour spots, both will be poured.

We will not give you the solution of WSP3. You can spend time in the holiday to refine your game!
Submit your best effort – we will use a marking scheme to credit you for working aspects.


WSP 4: Future Fun

During the November holiday you can add an “undo” function.
Undo’s are typically done using stacks – so you add each operation on a stack – the most recent ones will be on top!
You will have to create a class for a “move” with instance variables for “source” and “target” to push on the  undo stack.
A Note on Graphics:
The game was created in Unity – try it!!!
You can even attempt it in Java without the pouring animation.

I hope you feel empowered after this project!

