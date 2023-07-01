---
layout: post
title: Object Oriented Programming Unit 6 reflection
subtitle: Abstract Methods and Interfaces
tags: [OOP, Abstract, Methods, Interfaces 6]
---
## Reflection of Unit

#### Codio Encapsulation notes:
Learning about **encapsulation** makes it useful for me to gain a better understanding of why it is used and why it is important. Essentially, there seems to be an element of restriction to certain parts of data which provides several benefits (such as increasing the probability of errors/bugs).

It also seems to be important to be aware that there are differences in terms of how encapsulation works between different program languages – whereas in languages such as Java which explicitly state which types of data are public and private in their code, the Python language does this in a different way. Because classes in Python do not explicitly hide or restrict access to data, all attributes and methods in a class are in fact *public by default!*.

Python uses the convention of an **underscore** to indicate the data being private. However, it’s important to be aware that Python itself still thinks that the data is public; if it were really private, Python would instead print an error message.

#### Encapsulation – Getters and Setters (Codio):
All to do with the **private attribute** (using a single underscore (_). 
**Getters** are used to return the private attribute.
**Setters** are used to update the value of the private attribute.
        
Example of Getter method:
        
        def get_model (self):
	        return self._model
        
Example of Setter method:
        
        def set_model (self, new_model):
	      self._model = new_model


#### References
Philips, D. (2018) 'The Iterator Pattern' in: *Python 3 Object-oriented Programming*. 3rd ed. Packt Publishing.
