---
layout: post
title: Object Oriented Programming Units 2 and 3 reflection
subtitle: Introduction to UML
categories: 
tags: [OOP, UML, 2, 3]
---

I have learnt about the key concepts associated with object oriented programming (OOP). While this theory seems reasonably simple to me, the practical using codio exercises, such as classes and objects, is more of a difficulty for me. I think it will take some more time for me to get to grips with the new syntax involved, but more importantly, to get to grips with understanding the processes that are going on. 

I am finding the codio classes very hard at the moment – started doing the classes and objects classes this week and it just seems a bit confusing to me. The previous module seemed a lot easier to head my head around and learn the processes step-by-step. There was a more logical and straightforward structure to those classes compared to the ones in this module (i.e. learn the theory and then execute what you have learnt in the final exercises). I understand that we are being introduced to more complex topics now but it still feels hard to learn from. Although, I am using additional resources to learn about the topics involved in OOP (including Udemy and Codecademy) which has helped my understanding of this topic.

#### Unit 2 Codio notes for Class Functions and Class Methods:
A programmer-defined type is also called a **class**.

Defining a class named Point creates a **class object**.

Because Point is defined at the top level, its “full name” is **__main__**.Point.

The class object is like a factory for creating objects. To create a Point, you call Point as if it were a function.

Creating a new object is called **instantiation**, and the object is an **instance** of the class (object = instance)

When you print an instance, Python tells you what class it belongs to and where it is stored in memory.

For example, in contemporary operating systems, windows, icons, and other elements can be programmed once and then multiple instances can be created.
We are assign values to named elements of an object. These elements are called **attributes**.

      For example, to represent a rectangle, we might have to instantiate a rectangle object and assign values to the attributes:
      box = Rectangle()
      box.width = 100.0
      box.height = 200.0
      box.corner = Point()
      box.corner.x = 0.0
      box.corner.y = 0.0

      The expression box.corner.x means, “Go to the object box refers to and select the attribute named corner; then go to that object and select the attribute named x.”

An object that is an attribute of another object is known as an **embedded object**.
      e.g. user.height = 65

You can change the state of an object by making an assignment to one of its attributes. For example, to change the size of a rectangle without changing its position, you can modify the values of width and height:
      box.width = box.width + 50
      box.height = box.height + 100

When writing a new class, it is probably best to start by writing __init__, which makes it easier to instantiate objects, and __str__, which is useful for debugging.

A class variable is different to an instance variable. 
For example:
      class Girls:                                                            
	      gender = ‘female’ 
	      def __init__(self, name):        
		      self.name = name


#### Unit 3 Notes
Learning about **UML (Unified Modelling Languages)**: seems to be quite a straightforward and simple concept used in IT/businesses in order to efficiently and effectively communicate software designs/models so that essentially everyone is on ‘the same page’ and has a general understanding of what is needed and what to expect (i.e. software engineers, stakeholders, management team).

I found the lecturecast to be very helpful when giving a clear and organised way of how UML works and the different models that are involved within in. I feel confident in understanding what the different models do, which models are associated with which type (behavioural, structural or architectural), why there are different models to be aware of.

From what I have seen, it seems to be at least useful to know and be aware about UML but they do not seem to be necessarily common to experience when working in software companies. However, it appears that being able to know and understand some form of software diagramming is very important for a career in development.

It’s also useful to be aware of the various issues that can occur with experiences with UML including:

> The lack of consistency – especially when there are multiple teams involved in the development process and these teams have different understandings with each other regarding the model/system.

> Poor quality models/diagrams which may lead to various ways in which the model is represented by different groups/members, which can affect the overall understanding of the model.

> The informality that some developers may apply when creating the models, which can lead to key information being missing and shortcuts being taken - although it should be noted that modelling is not the same as coding. For example, it is similar to the way in which the building industry works, whereby blueprints are written in an informal style using many different methods that depend on the common sense of the builder, but the buildings are still built from them successfully.


#### e-Portfolio activities

Discuss which UML models are most applicable at different stages of the Software Development Life Cycle.

Making reference to ‘The Unified Modeling Language Reference Manual Second Edition’, use the State Machine Diagram in Figure 3-7 to design a similar model for a washing machine.





#### References
Lange, C.F., Chaudron, M.R. & Muskens, J. (2006) In Practice: UML Software Architecture and Design Description. *IEEE Software*, 23(2), pp.40-46.

Philips, D. (2018) 'Object Oriented Design' in: *Python 3 Object-Oriented programming*. 3rd ed. Packt Publishing

Rumbaugh, J., Jacobson, I. & Booch, G. (2004) 'UML Walkthrough' in: *The Unified Modeling Language Reference Manual*. 2nd ed. Addison-Wesley.

von der MaBen, T. & Lichter, H. (2002) Modeling variability by UML use case diagrams. *In Proceedings of the International Workshop on Requirements Engineering for product Lines*, pp. 19-25.
