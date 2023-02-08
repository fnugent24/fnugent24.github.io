---
layout: post
title: Unit 2
subtitle: Introduction to Computer Architecture and the Functionality
categories: 
tags: [Architecture, Functionality, 2]
---

## Reflection of unit

Already have some prior knowledge about the key components in the CPU and their functions but nonetheless good to clarify up on.
The circuitry in a computer that controls the manipulation of data is called the central processing unit, or CPU (often referred to as merely the processor).
A CPU consists of **three parts**: 

1.	The Arithmetic/Logic unit, which contains the circuitry that performs operations on data (such as addition and subtraction). This unit is  also capable of performing operations other than the basic arithmetic operations, such as the Boolean operations AND, OR, and XOR.

2. The Control Unit, which contains the circuitry for coordinating the machine’s activities

3. The Register Unit, which contains data storage cells (similar to main memory cells), called registers, that are used for temporary storage of information within the CPU.


Important to be aware that although we perceive the computer as a very intelligent device, it is actually a set of instructions that has made the computer an intelligent device. A computer has the ability to execute a set of instructions and these executions can be iterative or maybe by selection. This specific feature enables the programmers to write a set of instructions for computers to execute and they are called software.

Fairly comfortable already with how inputs, outputs, storage and instructions all coordinate with each other to perform a specific task or can be utilised to solve a problem by providing a set of instructions.

Some useful points I found in the article/core e-book:

The key to managing complexity in computer systems is their division into **levels of abstraction** separated by well-defined interfaces. The levels of abstraction are arranged in a hierarchy, with lower levels implemented in hardware and higher levels in software. In the hardware levels, all the components are physical, have real properties, and their interfaces are defined so that the various parts can be physically connected. In the software levels, components are logical, with fewer restrictions based on physical characteristics.

The diversity in instruction sets and operation systems in computers has both positives and negatives – while it encourages innovation and discourages stagnation, it also leads to reduced **interoperability** (the ability of computer systems or software to exchange and make use of information), which becomes restrictive, especially in a world of networked computers, where it is advantageous to move software as freely as data.

The hardware resources of a system are generally managed by a single operating system which limits the flexibility of the system. The concept of **virtualisation** provides a way of relaxing these constraints and increasing flexibility – it is the process of turning hardware into a software equivalent without sacrificing functionality. 

**A virtual machine (VM)** is implemented by adding a layer of software to a real machine to support the desired virtual machine's architecture. E.g., virtualizing software installed on an Apple Mac can enable Windows to run on it. Another example is that a computer user might have a Java application running on a laptop PC. This is done via a Java virtual machine developed for Linux.

The term **architecture**, when applied to computers, refers to the functionality and appearance of a computer system or subsystem but not the details of its implementation. The term **implementation** will be used to describe the actual embodiment of an architecture. Any architecture can have several implementations, each one having distinct characteristics, e.g., a high-performance implementation or a low-power implementation. An example of an implementation in software 
Is an interface between an application program and standard libraries.

**Emulation** adds considerable flexibility by permitting "mix and match" cross-platform software portability.

System virtual machines provide a complete system environment in which many processes, possibly belonging to multiple users, can coexist. At the time they were first developed, mainframe computer systems were very large and expensive, and computers were almost always shared among a large number of users. Different groups of users sometimes wanted different operating systems to be run on the shared hardware, and VMs allowed them to do so. Over time, as hardware became much less expensive and much of it migrated to the desktop, interest in these classic system VMs faded.

Benefits for using system virtual machines - if security on one guest system is compromised or if the guest OS suffers a failure, the software running on other guest systems is not affected. The ability to support different operating systems simultaneously, e.g., Windows and Linux, is another reason for their appeal.



>**e-portfolio – managed to progress quite a bit with this this week. Already started in unit 1 but this week I polished it quite a bit and have gained the knowledge >of how to implement posts which I am labelling for each separate unit. Seem to be quite confident of how to perform the fundamentals with e-portfolios on github >now.**




>**Codio – progressed quite a bit with this. Started with the Python tasks and managed to work through many of them throughout the week. Though still feel that I >might have rushed some of the tasks and may have to look back at them to fully clarify things.**




### Learning Outcomes:
To appreciate the evolution of computer and computing technologies due to innovations

To describe the critical functional issues of computer structure components

To identify and demonstrate the basic characteristics, functions and features of each element of a computer system

To demonstrate the theories and nature of data representation for computers
