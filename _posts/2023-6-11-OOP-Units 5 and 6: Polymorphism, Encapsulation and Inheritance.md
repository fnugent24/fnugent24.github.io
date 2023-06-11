---
layout: post
title: Object Oriented Programming Units 5 and 6 reflection
subtitle: Polymorphism, Inheritance and Encapsulation
tags: [OOP, Polymorphism, Inheritance, Encapsulation, 5, 6]
---

## Reflection of Units

#### Polymorphism:
Learning about polymorphism – a very important concept in programming. It refers to the use of a single type entity (method, operator or object) to represent different types in different scenarios.

Example of polymorphism: using the + operator

The + operator can be used for different types in Python (it can be used to add numbers together 1 + 2 = 3 for int data types or it can also be used to form two words together (concatenation) for string data types – “hello” + “dad” = hello dad).

Another example of polymorphism: the len( ) function

The len ( ) function can also be used for different data types in Python. It can be used to output the length of strings, lists, tuples, and dictionaries. For strings, it outputs the number of letters in that string, for lists, it outputs the number of items in that list and for dictionaries, it outputs the number of keys within that dictionary. So it outputs a number depending on the data type being used.

Like in other programming languages, the child classes in Python also inherit methods and attributes from the parent class. We can redefine certain methods and attributes specifically to fit the child class, which is known as Method Overriding. This process is particularly useful in cases where the method inherited from the parent child doesn’t quite fit the child class.

Polymorphism allows us to access these overridden methods and attributes that have the same name as the parent class.
For example, here is the code for an example of method overriding (i.e. redefining methods and attributes from the parent class (i.e. Bird) to fit into the child classes (i.e. sparrow and ostrich).

> class Bird:
>> def intro(self):
>>> print("There are many types of birds.")
     
    def flight(self):
      print("Most of the birds can fly but some cannot.")
   
  class sparrow(Bird):
    def flight(self):
      print("Sparrows can fly.")
     
   class ostrich(Bird):
    def flight(self):
      print("Ostriches cannot fly.")
     
  object_bird = Bird()
  object_spr = sparrow()
  object_ost = ostrich()
 
  object_bird.intro()
  object_bird.flight()
 
  object_spr.intro()
  object_spr.flight()
 
  object_ost.intro()
  object_ost.flight()


### This will output the following:
There are many types of birds.

Most of the birds can fly but some cannot.

There are many types of birds.

Sparrows can fly.

There are many types of birds.

Ostriches cannot fly.


#### Inheritance (Codio):
Inheritence is the ability to define a new class that is a modified version of an existing class.

For example, in poker, there are different concepts involved in the game including the use of a “deck” and a “hand”. A hand is similar to a deck as both are made up of a collection of cards and both require the uses of adding and removing cards. But they both have differences between them as well. Lets say we create a class for each of “hand” and “deck”. The relationship between these classes (which are similar but also different to each other) is known as inheritance.

To define a new class that inherits from an existing class, you put the name of the existing class in parentheses. E.g. if we were to inherit the class “hand” from the class we have already created called “deck” we would use the following code:

**class Hand(Deck):**

Here, the existing class (Deck) is known as the parent and the new class is known as the child.

Inheritance is a useful feature (and core feature) of object-oriented programming. It can promote the reusability of code since the behaviour of the parent class(es) can be customised (i.e. creating child classes) without having to essentially modify them.

On the other hand, inheritance can make programming hard to read. When a method is called, it can be unclear where to find its definition. It can also make debugging difficult because when invoking a method on an object, it may be hard to figure out which method will be invoked.


#### Class diagram:
A class diagram is a diagram showing all the classes and the relationships between them.
There are several kinds of relationships between classes:
> Objects in one class may contain references to objects in another class. For example, in poker, each Deck contains references to many Cards. Or a tv remote contains references to many types of buttons. This kind of relationship is called HAS-A, as in, “a Deck has a Card”.
> A further relationship includes one class that inherits from another class. For example, a Hand inherits from a Deck. This kind of relationship is called IS-A, as in, “a Hand is a kind of a Deck”.


The following class diagram shows the relationships between Card, Deck and Hand:

<img width="491" alt="image" src="https://github.com/fnugent24/fnugent24.github.io/assets/119634822/c944845a-50a3-426a-8ff0-cca1b59f6f57">




#### Encapsulation (Codio):
Learning about encapsulation makes it useful for me to gain a better understanding of why it is used and why it is important. Essentially, there seems to be an element of restriction to certain parts of data which provides several benefits (such as increasing the probability of errors/bugs).

It also seems to be important to be aware that there are differences in terms of how encapsulation works between different program languages – whereas in languages such as Java which explicitly state which types of data are public and private in their code, the Python language does this in a different way. Because classes in Python do not explicitly hide or restrict access to data, all attributes and methods in a class are in fact public by default.

Python uses the convention of an underscore to indicate the data being private. However, it’s important to be aware that Python itself still thinks that the data is public; if it were really private, Python would instead print an error message.

