##Basic Javascript! Data types, variables, arrays, oh my!

###SWBAT
* List the five primitive javascript data types
* Create an array and access any item in that array
* Add and remove items from an array


##Types

A **type** in a programming language specifies a **kind of data**. While this might not be the most technical way to describe it, it's how we're most likely to think about it. 

Javascript has five **primitive** types:

* String - characters or textual data... stuff like:  "abc" and "hello there 123"
* Number - just like it sounds... this is a number: 123 or 12.3
* Boolean - these are `true` or `false` values
* Null - has exactly one value which is: `null`. This is used to signify an empty value. 
* Undefined - usually this is a variable that hasn't been initialized: `var x;` will result in x being undefined at this point.  


Those are primitive data types. What does that mean...that they live in caves? No, in the context of Javascript we can think of them as being baseline values.


**Anything that dosen't belong to any of these five primitive types is considered an object.**

* Object

Objects are complex types with many properties and methods attached or 'built in' to them. An object can be thought of as a logical containment unit for values and functionality that will manipulate or provide access to those values. Believe it or not, a function is a type of object. An array is also a type of object.


### What's the point of knowing these data types?

Because each data type has a whole bunch of built-in methods you can call on it. 

Try this in your console:
```
"hello".length

3.length
```

Now try this:
```
"carrot" - "car"

6 - 3
```

lastly, try this:
```
3 + 5

"tea" + "pot"
```

Interesting... we can use the `+` operator on both the number type AND the string type. But it does something different for each of them.


##Variables
What's the point of having data types if there is nowhere we can temporarily store them?

This is where variables come in.

The special word (keyword) `var` indicates that this sentence is going to define a variable. It is followed by the name of the variable and, if we want to immediately give it a value, by an `=` operator and an expression.

This is not arithmetic, this is *assignment*.

So we can say 
```
var x = 1
x = x + 9

console.log(x) => gives us what?
```

How do we name variables? Use common sense and camelCase.

We will come back to how variables are stored later...

###Array of hope!

**A JavaScript array are high-level, list-like objects**

**What is an Array**

*    A container for data, similar to a list. You could think about it like a pill box.
*    An array is a data structure.
*    Each item in an array is called an element.
*    Arrays can hold all kinds of different data types: strings, integers, objects, functions, even other arrays!

What types of arrays did we see in the prework?

There are two ways to properly create an array; one that you all have seen before and one that is relatively rare, but I still want you to be able to understand it.

```
// rare syntax
var superheroes = new Array("Batman", "Superman", "Buffy", "Captain America");

// what we're going to be using
var superheroes = ["Batman", "Superman", "Buffy", "Captain America"];

```

The most important thing we're going to be using arrays for is to access the elements inside of them.

What would I need to type to access the element "Batman" in my `superheroes` array?   
`superheroes[0]` right?

How could I access "Buffy"?

Think of it like years in your life. You start at zero and go from there. 

###Loops
**What is a loop** 

So far we've seen two different loops in Javscript in the prework:

* `While`
* `For`

###While Loops

Let's start with a `while` loop and then move onto `for` loops later.

The two parts of a while loop:  

*  A condition that it checks
*  Something that it does

####For Loops
While loops are similar to For loops, but for loops are often the better choice because they take care of the assignment, the run condition and the incrementation/decrementation all in one step.

Why is it called a for loop? 

	"The loop body is executed 'for' the given values of the loop variable"

```
for(assignment; run condition; increment/decrement){
    //LOOP ACTION HERE
}
```

* THE ASSIGNMENT sets a variable before the loop begins
* THE RUN CONDITION defines the condition for the loop to run
* INCREMENTS/DECREMENTS executes after each completed loop  

**Avoiding Infinite Loops**

Loops operate based on conditional statements, running as long as the condition it is checking against is true. Take care not to write a condition that will always evaluate to true, otherwise you will create an infinite loop that will crash your browser (and maybe your whole computer!!!).

