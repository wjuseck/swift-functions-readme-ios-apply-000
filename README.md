# Functions

![CatDog gif](http://i.imgur.com/85Pd59R.gif)


## Learning Objectives - The student should be able to..

* Explain that a function is a **self-contained** chunk of code that performs a **specific** task.
* Explain that a function has a name that identifies what it does, and that name is used to "call" the function to perform its task when needed.
* Break down the various parts of a function.
* Properly be able to describe what is going on here:

```swift
func sayHelloToCat(kittenName: String) {
    print("Hello, \(kittenName), why do you sleep so much?")
}
```
* Create their own function that can take in two arguments of type String and Int and print out a sentence within that functions implementation utilizing both.





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
* Everyday, our owner takes us for a walk.. in this walk, we have to walk by dozens of cats (we know all of their names) and we want to say Hello to each one and ask them the question.. why do you sleep so much. It would be silly to have to write out doezens of print functions where they only difference is the kitten name. If we can have the student  (or dog) SEE that the only difference between each greeting is the cats name, that is very important. We then introduce **functions**.
* At this stage, we go into how to write our own function.

```swift
func sayHelloToCat(kittenName: String) {
    print("Hello, \(kittenName), why do you sleep so much?")
}

func sayHelloTDog(puppyName: String) {
    print("Hello, \(puppyName), want to go sniff that rock together?")
}

```

* This is the first time they are seeing a function, so we should be explicit in our explanation, talking about the func keyword, the name of the function and its arguments.
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

* Formulate a question or scenario (possibly still going with this dog/cat thing) where passing in two arguments to the function would help or solve the problem:

```swift
func sayHelloToCat(kittenName: String, kittenAge: Int) {
    print("Hello, \(kittenName)! \(kittenAge) is a wonderful age to be")
}
```

<a href='https://learn.co/lessons/FunctionStuff' data-visibility='hidden'>View this lesson on Learn.co</a>
