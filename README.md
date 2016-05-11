# Functions

![CatDog gif](http://i.imgur.com/85Pd59R.gif)


## Learning Objectives - The student should be able to..

* Explain that a function is a **self-contained** chunk of code that performs a **specific** task. A function should do one thing and one thing well.
* Explain that a function has a name that identifies what it does, and that name is used to "call" the function to perform its task when needed.
* Break down the various parts of a function. Create a function that takes no arguments:

```swift
func sayHello() {
    print("Hello everyone!")
}
```
* Create a function that contains one argument, like so:

```swift
func sayHelloToCat(kittenName: String) {
    print("Hello, \(kittenName), why do you sleep so much?")
}
```






## What the student can do at this point 

* Create variables and constants
* Knows how to use the print function (although they might not know that it's referred to as a function at this point).
* Can create variables of type String and Int (no other types).
* Will NOT have seen a function yet, this readme will be the first time they see it.
* They would have come off just doing a mini lab in a Playground file which had them  become familiar with everything they had just learned (String, Int, variables, constants, print, string interpolation, type inference, type annotations).



## Outline / Notes

*  At this stage, where the student has NOT seen a function yet. It's important to be explicit in our descriptions of the various elements that make up a function. Almost like operating in a slo-mo like manner, making NO assumptions.
* Readme narrative is around puppies and kittens (include this gif? - http://i.imgur.com/85Pd59R.gif)
* Put the student in the shoes of a dog. If they were a dog, there is certain functionality that a dog walks around with. They can bark, they can eat, etc. BUT, we're special.. we can speak English.
* We can encapsulate within a function, a print statement that will greet others (our personalized greeting) and we don't want to have to type this over and over and over again where we can make a mistake or make typo's, instead we can create a function that within the scope of that function.. it will print out the greeting we want. Then we can call on that function over and over.


```swift
func sayHello() {
    print("Hello everyone!")
}
```

* This will be the very first time they see a function, be very explicit in your explanation in **detail** to the various parts of the above code. Even go into how *sayHello* is written as camel case. Why are we writing our code within the curly braces `{ }`? If we declare something within those curly braces, can I access that variable outside of the function?

* How do I call on a function? When does the code within those curly braces get called? Have them follow along and get used to writing this out in a playground file. 
 
* Everyday, our owner takes us for a walk.. in this walk, we have to walk by dozens of cats (we know all of their names) and we want to say Hello to each one and ask them the question.. why do you sleep so much. It would be silly to have to write out doezens of print functions where they only difference is the kitten name. If we can have the student  (or dog) SEE that the only difference between each greeting is the cats name, that is very important. We then introduce **arguments**.
* At this stage, we go into how to write our own function that includes arguments. Instead of saying "Hello everyone!", we would like to say Hello to each individual cat. Show that in code:

```swift
func sayHelloToGarfield() {
    print("Hello, Garfield, why do you sleep so much?")
}

func sayHelloToBuster() {
    print("Hello, Buster, why do you sleep so much?")
}

func sayHelloToScratchy() {
    print("Hello, Scratchy, why do you sleep so much?")
}
```

* Instead of doing that, ask the student if they can recognize the common pattern here. What is the only difference between these three functions. Use this as a way to jump into functions with arguments:

```swift
func sayHelloToCat(kittenName: String) {
    print("Hello, \(kittenName), why do you sleep so much?")
}

func sayHelloTDog(puppyName: String) {
    print("Hello, \(puppyName), want to go sniff that rock together?")
}

```


* So we created a function, but now how do we call on it?
* These functions take in String types as their arguments, which is something we know how to do create.
* Show them these two ways of passing in Strings to this function:

```swift
let nameOfCatEatingLasagna = "Garfield"
sayHelloToCat(nameOfCatEatingLasagna)
// prints "Hello, Garfield, why do you sleep so much?"

sayHelloToCat("Max")
// prints "Hello, Max, why do you sleep so much?"
```


<a href='https://learn.co/lessons/FunctionStuff' data-visibility='hidden'>View this lesson on Learn.co</a>
