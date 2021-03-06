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
- I did alright and did not struggle with anything during this task. 

## Task 2: Create a RadGradSegment containing the current user

<img class="ui centered image" src="../images/Task2Completed.png" alt="NONE">

### What I learned: 
From previous projects I already knew how to grab the username of the user using Meteor.user(), so the first part of the task wasn't too hard. However, I was not too sure how to grab the username appearing in the URL. I had decided to refer to my other teamates' essays about how they solved this task. A lot of them mentioned using useParams() from ReactRouters. 

- Basically, useParams() returns an object of the params for the route rendered. More about useParams() can be found [here](https://reach.tech/router/api/useParams){:target="_blank"} and [here](https://reactrouter.com/web/api/Hooks){:target="_blank"}.

- Another great tip for doing this is using the shortcut **cmd shift f** to find examples of how useParams() was used. 

- The final code I ended up writting to get the user name looked like this:
`const { username } = useParams();`

### Struggles: 
- I initially struggled with finding out how to grab the username appearing in the URL. 

## Task 3: Create a RadGradSegment presenting MiniMongo data

<img class="ui centered image" src="../images/Task3Completed.png" alt="NONE">

### What I learned/ Struggles: 
Task 3 wasn't too hard. I knew that in order to randomize the careerGoals I needed an array of career goals to randomize. From previous projects, I had used underscore's .sample to randomize the chosen value from an array, however I don't think Radgrad is using underscore so I had to look for another way to randomize input from an array. The solution I found came from this link: https://stackoverflow.com/questions/9286473/whats-the-equivalent-of-sample-in-javascript

Another thing I needed to know was how to actually get the data needed to randomize. I decided to consult my teamates' essays. I noticed that they used CareerGoalBrowserViewPage.tsx as an example to follow, so I decided to take a look. CareerGoalBrowserViewPage.tsx uses something called interface to get the career goals.

According to [typescript documentation](https://www.typescriptlang.org/docs/handbook/2/objects.html){:target="_blank"} an interface is simply a way to represent object types. An interface allows us to name the object. 

In this case I decided to name the object Task3CareerGoalsProps. The object looked something like this: 
- `interface Task3CareerGoalsProps {
  careerGoals: CareerGoal[];
}`
- `careerGoals` is the singleton instance of this class from the CareerGoalsCollection api 
- `CareerGoal[]` is an array which holds all of the career goals in the database. 

One of the things I was a little confused by was the `React.FC` thing? I've never used this in any of my previous projects so I decided to look it up. According to this website https://fettblog.eu/typescript-react-why-i-dont-use-react-fc/ , since react was not written in Typescript a package from the community was provided called @types/react. FC is simply a generic type that is used to create function components. 

From a lot of examples I am seeing inside these `<...>` brackets we put the object name. 
- [good resource for typescript](https://react-typescript-cheatsheet.netlify.app/){:target="_blank"}

## Task 4: Create a RadGradSegment containing Labels

<img class="ui centered image" src="../images/Task4Completed.png" alt="NONE">

### What I learned/ Struggles: 
This task wasn't too hard since I had a code with me session to complete it. After knowing how to display the labels for the career goals, the rest was not hard. This was the following code used to display the career goal labels. 

` <h3>Career Goals</h3> `
`{careerGoals.map((goal) => (`
   `<CareerGoalLabel slug={Slugs.getNameFromID(goal.slugID)}/> ))}`
   
Another important thing to keep in mind while doing this task is that for the student profiles you have to make sure to only retrieve the students are not alumni, so the following code does that. 

`const students = StudentProfiles.findNonRetired({ isAlumni: false });`

## Task 5: Use a form to control what's displayed in a page
<img class="ui centered image" src="../images/Task5Completed.png" alt="NONE">

### What I learned/ Struggles: 

For this task I first looked for examples of how autoforms is used with in the RadGrad2 project. I used the [Add academic year Instance file](https://github.com/radgrad/radgrad2/blob/master/app/imports/ui/components/admin/datamodel/academic-year/AddAcademicYearInstanceForm.tsx) to help me write the swal alerts and the form. Since I have already used autoforms in previous project this task was not too hard. I also referred to my other teamates essays for more direction. 

## Task 6: Meteor Methods: Create a form that updates the database
<img class="ui centered image" src="../images/Task6Completed(1).png" alt="NONE">
<img class="ui centered image" src="../images/Task6Completed(2).png" alt="NONE">

### What I learned/ Struggles: 

For this task I first looked for examples of how to edit autoforms in the RadGrad2 project. I used the editCareerGoals file to help me figure out what I would need to complete this task. I noticed that the two most important things for editing is the update method with call promise and update schema, so I knew that I had to include these in the component to edit the description. I also referred to my other teamates essays for more direction.

## Task 7: Tabbed and Modal components (Bonus round)
<img class="ui centered image" src="../images/Task7Completed.png" alt="NONE">

### What I learned/ Struggles: 

For this task I first referred to my teamates essays to complete this task. This task was not too hard. I have used modal before, but I have never used tabs before so it was a little hard at first but after getting the first tab to work it was straightforward. I used the advisorFilteredStudentTabs.tsx as an example of how to use tabs.

&nbsp;
&nbsp;
&nbsp;
&nbsp;
&nbsp;
&nbsp;
&nbsp;
&nbsp;
