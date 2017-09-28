## Homework 06 - Tristan Porter ##

#### 1. Consider the programming languages you may have studied and their differences. Think of two problem domains you would use for each language. For each problem domain, explain why your choice of the other language would be a poorer choice for an implementation language. ####

**Python**

- Coding simple programs - Java has a lot of extra syntax that can be avoided with Python
- Doing calculations - Setting up functions in Java is more complicated

**Java**

- Making a game - Python is not object-oriented which would make it almost impossible to code a substantial game
- Making data structures - Python simply cannot handle all of the data types and cannot do objects
			

#### 2. Give some concrete counter-examples of good programming practices as discussed in the book. These include meaningful variable names, self documenting code, symbolic constants, and code layout. In other words, give examples of what not to do.? ####

**Non-meaningful variable names:**
 
	this = 1;
	that = 2;
    other = 3;

What do the variables represent?

**Non-documented code:**
	
	finalResult = firstAnswer - secondAnswer;

What does this final result mean?

**Bad code layout:**

	public static void function1() {
		return;
	}
	public static void function2() {
		return:
	}
	
	public int numberOne;
	public int numberTwo;

Variables can get lost or forgotten if they are not declared at the beginning of the code.

#### 3. Give two versions of coding standards for sub procedure blocks. This may require an internet search. Which do you prefer, and why? ####

An example of a sub procedure in Python:

    def exampleFunction():
        print("This is an example function")

An example of a sub procedure in Java:

    public static void printExampleText(){
    	System.out.println("This is an example");
    }

I prefer the Java approach. To me it looks cleaner and the brackets help to clearly define where the definition of the function ends. Also you can tell from just the first line of the definition whether the function returns anything or not.

#### 4. An informal description of the DRY principle is this: "The second time you write exactly the same code, stop what you are doing and place that functionality in a sub procedure. Then, invoke the sub procedure whenever you need that functionality." Give one example of this from your previous programming experience. If you have never experienced this in practice, make up an example. ####

The most recent time was for an assignment in my Defensive Programming class. We had to write a program and part of it had to print out information after calculating some values. I had to write the same print statement a few times, so instead I put that print statement and calculation in a function. Then when I needed to do the calculation and print the information, I just called that function.

#### 5. What is a stub ? What is a driver ? Have you ever used stubs or drivers in your previous programming experience? If so, give an example. If not, consider a function that takes a unit price, a sales tax rate, and the quantity ordered, and write a stub (using pseudo code or a language of your choice) that takes these three arguments and returns a value. ####

A stub is a piece of code that is used to stand in for some other programming functionality. It simulates the behavior of a lower-level module that is not integrated yet. A driver simulates the behavior of an upper-level module that is not integrated yet. No, I don't think that I have ever used them.	

    public static int example(int unitPrice, int salesTaxRate, int quantityOrdered) {
		unitCost = 18;
		salesTaxRate = 19;
		quanityOrdered = 20;
		cost = unitPrice * quantityOrdered;
    	finalCost = cost + (cost * salesTaxRate);
    	return finalCost;
    }

#### 6. List two strengths and one weakness of top down integration. ####

**Strengths:**

- Advantageous if major flaws occur toward the top of the program.
- Early skeletal Program allows demonstrations and boosts morale.

**Weakness**

- Test conditions ma be impossible, or very difficult, to create.

#### 7. List two strengths and one weakness of bottom up integration. ####

**Strengths:**

- Test conditions are easier to create.
- Observation of test results is easier.

**Weakness**

- The program as an entity does not exist until the last module is added.

#### 8. This is not in the book and will require some independent research. A domain specific language (DSL) is a small, incomplete language typically use as a "glue" language between a lower level language (like C) and a higher level language (like Python). An example of a DSL might be a helper language for HTML, e.g. div(...) might resolve to <div> ...</div>. How might a DSL promote what the book calls sandwich integration ? This is not a trick question but it will require some thought. If you work as a developer, you will eventually write your own DSLs for various purposes. ####

A DSL would promote sandwich integration because

#### 9. What is the difference in testing carried out by the implementation group and the testing carried out by the SQA group? ####

The implementation group is familiar with the program and code and know how it works. While, the SQA group will be fresh eyes seeing it for the first tiume.

#### 10. Read the letter by Edgar Dijkstra to the Communications of the ACM (in the PDF directory as dijkstra68.pdf) and write a one paragraph appreciation of this letter. ####

Dijkstra is explaining why he finds the use of the go-to statement bad. He wants programmers to stop using it. And explains his reasoning by giving an example of want to measure the progress of a process. He uses a lot of technical talk that was a little hard for me to understand. But what I got out of it was that while go-to statements are not inherently bad, it makes tracking progress easier if one uses other things instead.