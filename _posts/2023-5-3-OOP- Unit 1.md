---
layout: post
title: Object Oriented Programming Unit 1 reflection
subtitle: Introduction to Python Programming and the OO Programming Paradigm
categories: 
tags: [Object, Oriented, Programming, OOP, 1]
---

#### Reflection
I look forward to completing this module, particularly as there is a strong focus on the Python language. I am also hoping to get some experience with working on Java as that will be helpful to my development in software engineering.

While I am getting more to grips with the basics of Python, there are already a few things that I am not entirely comfortable with, and would like to improve my understanding upon. These include using For loops, classes, Lambda, and recursion. I think with loops (particularly with for loops), the issue is trying to get my head around being able to acknowledge what the computer is able to “understand” and the step-by-step approach that the computer undergoes.

#### Further reading
One thing I have learnt from the reading (Joque, 2016) is the argument surrounding the nature of a programming “language” – whether it is merely a way of providing instructions to a computer which it compiles literally and unambiguously through a strict set of rules, or whether it is more complex than that and is more akin to human languages which contain ambiguities, and can be creative, metaphoric etc. It seems to me that the creation and development of object-oriented languages (such as Python) have been able to demonstrate that programming languages can be creative and more akin to “real” languages.

The article by Di Silvestro & Nadir (2021) provides an interesting insight on the 'emerging and increasingly successful use of ePortfolios'. Perhaps, for me, one aspect of the article that I found particularly insightful was the fact that there was an element of a "journey" involved in the making of the portfolio; but not simply a way to see one's improvements in, for example, their levels of knowledge increasing in a particular field or their improvements in their writing skills, but also on a deeper, more profound level where they could see the development of their "pathway through life" opening up - as one student puts it: 'As I read through old postings, essays, and projects, a clear picture of a person in search of something, and trying to find her way emerged.


#### Unit 1 Activities:
Develop a Python program and apply protected and unprotected variables within it:

    class Shape:
      def __init__(self, length, width):
        self._length = length
        self.width = width

    obj = Shape(50, 10)
    print(obj._length)
    print(obj.width)

Note: protected/"private" variables are denoted by putting an underscore before the object name (e.g. self._length = length) while the conventional way of unprotected/"public" variables are to omit using an underscore (e.g. self.width = width).


#### References
Di Silvestro, F. & Nadir, H. (2021) The Power of ePortfolio Development to Foster Reflective and Deeper Learning in an Online Graduate Adult Education Program. *Adult Learning*, 32(4), pp.154-164.

Joque, J. (2016) The Invention Of The Object: Object Orientation and the Philosophical Development of Programming Languages. *Philosophy & Technology*, 29, pp.335-356.

Seth, A., Aggarwal, H. & Singla, A.R. (2011) Evolution of Technology through Procedural, Object Oriented, and Component Based to Service Oriented. *Journal for Computing Teachers.*
