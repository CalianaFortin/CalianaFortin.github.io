---
layout: essay
type: essay
title: Solving the Puzzle    
date: 2020-12-03
labels:
  - Learning
  - Design Patterns 
---

<img class="ui centered medium image" src="../images/puzzle.jpg" alt="NONE">


## Hitting A Brick Wall 

"How do I go about creating this?" is one of the main questions I had when working on my *Campus Occupancy* project. I did not know what libraries or components we were going to need to begin on our project. I did not really understand where I needed to direct my team, so we could get started. It was hard to map out a plan of getting from point a to b. 

## Breaking Through the Brick Wall

I was really lost, but then it hit me. Throughout the semester we learned about how to create websites/applications by manipulating the different templates provided. By utilizing these templates and manipulating the code to fit our application we could get started on our project. This scenario is a great example of the utilization of design patterns. Design patterns basically gives software engineers the ablility to rehash code. It provides the developer with an outline for how to go about things, and this outline can be used in number of different ways and in variety of different conditions. 

## Why use Design Patterns?

Design patterns provide developers with a way of tackling problems efficiently and effectively. This process, in my opinion helps to promote effective team work. It allows team members to commincate to other members about how to solve similar problems. Now we know the benefits of design patterns but, how can we utilize this? 

## Types of Design Patterns:

One of the main ways to begin utilizing desgin patterns is to understand the types. The most common types of design pattern are Factory, Singleton, Observer, and MVC. 

### Factory 

The factory design pattern consists of creating objects without exposing underlying logic, potentially returning objects associated with
different classes, and/or creating dependent objects. This type of design pattern is often more complicated than the typical object oriented constructor.

### Singleton

Provide a "global variable" in an object oriented language that does not support global variables, and/or provide complex global state.

### Observer 

The Observer deisgn pattern is useful when a set of objects (called the "Observers") need to be informed whenever a change in state occurs to another object (called the "Subject") This is a common scenario in event-driven systems when you need to provide one or more "event handlers".

### MVC 

MVC stands for model view controller. MVS is useful when implementing a user interface, it is desirable to decouple the internal representation of information from the way it is presented to and accepted from the user.

## Solving the Puzzle: Design Patterns used in Campus Occupancy 

By utilizing the Design Patterns used in the Bowfolios template we were able to "solve the puzzle" and begin starting our project. 

In the Campus Occupancy project my team, and I utilized the observer, MVC, singleton, and the factory design pattern. 

Here are some examples of where and how we ustilized these design patterns. 

An example of how observer is used in our project the publisher and subscriber implementation in our code. Basically, we publish the data, and the subscribers make sure to update the other things if something was changed. Bellow is an image showing the publishing of our data collection and the subscribers. 

<img class="ui centered large image" src="../images/publish.png" alt="NONE">


<img class="ui centered large image" src="../images/subscribe.png" alt="NONE">


MVC can be seen. The model is seen in our Data Collection then the view is the Datas.jsx where we loop through to create each row displaying the data. The file app.jsx is the controller and, it connects the Model, and the view so the user can input data. 

<img class="ui centered large image" src="../images/datascollection.png" alt="NONE">


<img class="ui centered large image" src="../images/Data.png" alt="NONE">


<img class="ui centered large image" src="../images/controller.png" alt="NONE">





