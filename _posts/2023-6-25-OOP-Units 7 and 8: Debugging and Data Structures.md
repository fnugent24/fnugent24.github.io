---
layout: post
title: Object Oriented Programming Units 7 and 8 reflection
subtitle: Debugging/error handling and Data Structures
tags: [OOP, Debugging, error handling, Data Structures, 7, 8]
---

#### Reflection of Units

Return values are a useful tool in terms of debugging/seeing where the error comes from.

A Python return statement can only return an object, not a value. It can only return one object (which can contain multiple values).

#### Data structures
I feel that there are still certain data structures which I need to go back to and make sure I’m comfortable with – we focused on data structures quite a bit in the previous module and I remember going through some of them and not being entirely comfortable with.
But I do feel comfortable with certain data structures such as dictionaries and lists. 

I am less sure about others such as tuples, sets and sequences.

It’s important to focus on these (and data structures in general) in the coming few weeks as that will be a part to include in the upcoming assignment of the driverless car.

The chapter “Python Data Structures” by Phillips (2018) has been useful in providing a recap of some of the core data structures in Python – including:

**Tuples** - the fact that they are immutable, can use them as keys in dictionaries, and can store data in them in order

**Dictionaries**

**Lists** – the fact that they usually only have the same type of object - i.e. strings or ints, that they store the data in some kind of order, and that they are useful for modifying data - i.e. delete, add

**Sets** - that they have a very similar syntactic structure to dictionaries (instead of using colons to separate the pairs of values, they use commas to separate them), and that they are most useful when using at least two of them in combination with each other

**Queues** – including FIFO (first-in first-out) queues which are most akin to real life queues, LIFO (last-in, first-out) queues which are known as stacks – i.e. having a stack/pile of paper and getting the top-most paper at the top, and Priority queues where the most “important” items are returned first 


#### Data Structures in Cybersecurity
The article by Kuk et al. (2019) is an interesting read showing the importance of Python language in the field of cybersecurity – suggests that knowledge of Python can be a particularly useful advantage compared to other programming languages in cybersecurity as it emphasises usage of algorithm designs/data structures.

Article has also led to me being (more) interested in the field of cybersecurity – potentially an area to research regarding what opportunities there are in this sector?


#### Codio Polymorphism notes
Learning about polymorphism – a very important concept in programming. It refers to the use of a single type entity (method, operator or object) to represent different types in different scenarios.

Example of polymorphism: using the **+** operator

The "+" operator can be used for different types in Python.
It can be used to add numbers together for int data types:
        
        1 + 2 = 3

Or it can also be used to form two words together (concatenation) for string data types: 
        
        “hello” + “dad” = hello dad

Another example of polymorphism: the **len( )** function

The len ( ) function can also be used for different data types in Python: it can be used to output the length of strings, lists, tuples, and dictionaries. 
> For strings, it outputs the number of letters in that string

> For lists, it outputs the number of items in that list 

> For dictionaries, it outputs the number of keys within that dictionary. 

So it outputs a number depending on the data type being used.

Like in other programming languages, the child classes in Python also **inherit** methods and attributes from the parent class. We can redefine certain methods and attributes specifically to fit the child class, which is known as *Method Overriding*. This process is particularly useful in cases where the method inherited from the parent child doesn’t quite fit the child class.

**Polymorphism** allows us to access these overridden methods and attributes that have the same name as the parent class.

For example, here is the code for an example of method overriding (i.e. redefining methods and attributes from the parent class (i.e. Bird) to fit into the child classes (i.e. sparrow and ostrich).

    class Bird:
      def intro(self):
        print("There are many types of birds.")
     
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

#### E-Portfolio Activities:
1.	Discuss the ways in which data structures support object-oriented development. Use examples of three different data structures to contextualise your response.
2.	Create a nested dictionary of data on cars within a Car class. Extend the program to work with the dictionary by calling the following methods:
•	items()
•	keys()
•	values()
3.	Read the article by Kampffmeyer & Zschaler (2007). Develop a program which allows a user to enter the properties which they require of a design pattern, and have the program make a recommendation. Your program should use a constructor to initialise attributes and assign values to variables based on input entered by the user.


#### References
Kuk, K., Milic, P., Spalević, P. & Gocic, M. (2019) *Algorithm design in Python for cybersecurity. Electrotechnical and Computer Science Conference*. ERK.

Philips, D. (2018) 'Python Data Structures' in: *Python 3 Object-Oriented Programming*. 3rd ed. Packt Publishing.

Reddy, P. P. (2019) Driverless Car: Software Modelling and Design using Python and Tensorflow.

Zhou, Z. Q. & Sun, L. (2019) Metamorphic testing of driverless cars. *Communications of the ACM* 62(3): pp. 61–67. DOI: 10.1145/3241979.
