---
layout: essay
type: essay
title: Building a Personal Sandbox
date: 2021-05-21
labels:
  - Learning
  - Website Design
---


## Task 1: Create a RadGradSegment containing "Hello, World"

<img class="ui centered image" src="../images/Task1Completed.png" alt="NONE">

### What I learned: 
- One of the useful tips I learned while working on this task was this one: **cmd shift f** in the folder you want to search through. 
  - This shortcut is extremely helpful when looking for examples of how to accomplish a certain task.

### Struggles: 
- I did alright and did not struggle with antyhing during this task. 

## Task 2: Create a RadGradSegment containing "Hello, World"

<img class="ui centered image" src="../images/Task2Completed.png" alt="NONE">

From previous projects I already knew how to grab the username of the user using Meteor.user(), so the first part of the task wasn't too hard. However, I was not too sure how to grab the username appearing in the URL. 


### What I learned: 
From previous projects I already knew how to grab the username of the user using Meteor.user(), so the first part of the task wasn't too hard. However, I was not too sure how to grab the username appearing in the URL. I had decided to refer to my other teamates' essays about how they solved this task. A lot of them mentioned using useParams() from ReactRouters. 

Basically, useParams() is returns an object of the params for the route rendered. More about useParams() can be found [here](https://reach.tech/router/api/useParams) and [here](https://reactrouter.com/web/api/Hooks).

Another great tip for doing this is again using the shortcut **cmd shift f** to find examples of how useParams() was used. 

The final code I ended up writting to get the user name looked like this:
`const { username } = useParams();`

### Struggles: 
- I initially struggled with finding out how to grab the username appearing in the URL. 

