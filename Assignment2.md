# Computer Science – Core Skills

Grup A
Assigment 2
78952 – Diego Alves de Oliveira

## Binary to decimal:

```
Convert your student number to a binary number and write it out:
```

My student number is: 78952.
In binary 78952 → 10011010010101000₂

```
Convert the following decimal numbers to 8-bit binary:
```

| Decimal |	Binary | Decimal | Binary     |
| :------ | :----- | :-------| :--------- |
| `0`     | 0₂     | `256`   | 100000000₂ |
| `0`     | 0₂     | `256`   | 100000000₂ |
| `1`     | 1₂     | `128`   | 10000000₂  |
| `2`     | 10₂    | `64`    | 1000000₂   |
| `3`     | 11₂    | `32`    | 100000₂    |
| `4`     | 100₂   | `16`    | 10000₂     |
| `5`     | 101₂   | `8`     | 1000₂      |
| `6`     | 110₂   | `4`     | 100₂       |
| `7`     | 111₂   | `2`     | 10₂        |
| `8`     | 1000₂  | `1`     | 1₂         |
|


## Version Control

We can compare version control to a "recipe book," where a chef tries to create a new dish but is unsure about the result of some spice combinations. To ensure they can recreate the best flavors in the future, they write down each combination they test.
Version control using Git works in a similar way: you write the code, and at the end of the change, you may realize that the solution wasn't as satisfying. In this case, Git allows you to revert to a previous version of the code, recovering a functional state without losing the history of changes.

## What is Git?

Git is a version control software. It allows developers to create different versions of a software from a main version without the risk of making a change that could cause a system failure.
It’s important to mention that Git is not a collaborative tool on its own, but when combined with other platforms like GitHub, GitLab, and Bitbucket, it allows for more effective management of collaborative work.

## To show its importance, let’s imagine a situation:

You received a request from a client to create an app. As one of the first steps, I imagine you will create a directory to store all the app's dependencies, such as images, features, and the files containing the code you will write.
After creating the app with the basic features, you present the project to the client, and they like what they see. However, they ask you to add more features to the app.

### At this point, we have two situations:
- Establish this as your main version. From this main version, you will make
  all the necessary evolutions.

- Create a copy of this main version to implement the changes the client
  requested.

```
To illustrate this process, let’s look at the flow below.
```

<flowWorkstation  align= "left">
<img width= "6000" src= "src/assets/img/flowWorkstation.gif">
</flowWorkstation>

---

With Git, you can test changes separately, and when everything is working, you can implement them into the main version of the code.
Another great benefit of version control is the ability to separate which version is in production and which one is in development, receiving improvements or bug fixes. Here, we are talking about the branches a software can have.

### What is a Branch?

A branch is a new offshoot created from the software where new features or adjustments will be made. Each new version saved is recorded through the commits the developer makes.

Let's look at the next example:

Imagine now that you work in a team with two other developers. In this scenario, each developer would create a copy of the main branch and make the necessary changes. After each developer finishes, they would commit and push their version to the main branch.

<flowBranch align= "left">
<img width= "6000" src="src/assets/img/flowBranch.png">
</flowBranch>

---

```
In the following example, we can see more clearly how two developers would work on the same project:
```

<flowTeamwork align="left">
<img width= "6000" src="src/assets/img/flowTeamwork.gif">
</flowTeamwork>

---

## What is GitHub?


GitHub is a platform for hosting repositories remotely. It allows developers to access their projects from anywhere, similar to cloud storage services like Google Drive, OneDrive, and others, but with features specific to developers.

It’s important to highlight that GitHub is more than just a platform for hosting source code. It helps teams better manage their projects without interference between team members, maintaining an organized history of all changes.

Even for developers working alone, keeping the code in a remote repository offers security. If something happens to the computer, like a hard drive failure, your code will be saved.
Another convenience is being able to switch workstations without losing any progress.

### But what’s the difference between Git and GitHub?
Many people confuse Git with GitHub, but they are not the same thing:
- Git is version control software that lets you track all changes made and revert or simply check previous versions.
- GitHub is a platform for hosting software managed with Git to facilitate collaborative work among a team.

### How does GitHub help with teamwork?
GitHub allows multiple developers to work on the same project, implementing or adjusting features without conflicts.
Branches allow team members to work in isolation, and pull requests keep the project organized and structured with a process defined by the team, such as only merging versions after a testing phase.

In the following flow, we can see this process clearly:

<flowTeamwork align= "left">
<img width="6000" src = "src/assets/img/flowGitHub.gif"> 
</flowTeamwork>


Although GitHub is more popular and has the highest number of users, [according to a StackOverflow 2022 Developer Survey](https://survey.stackoverflow.co/2022/#section-version-control-version-control-platforms).
Gitlab and Bitbucket are alternatives to GitHub and offer functionalities that attract the attention of companies, making the number of professional users greater than the number of users for personal use.

<surveyStackOverflow align= "left">
<img width="6000" src="src/assets/img/surveyStackOverflow.png">
</surveyStackOverflow>

```
Top 3 version control tools according to the StackOverflow 2022 Developer Survey
```

## FDE (Fetch Decode Execute)

It is the way in which a processor performs its tasks.
It represents the sequence of steps that the CPU follows to carry out a task.
No matter how complex the computer architecture, the CPU carries out the instructions for all the peripherals in the same way:

1. Fetch - Fetches the instruction from memory, always starting from position zero in its address.
2. Decode - the CPU decodes the value that is stored in the address that fetched the information.
3. Execute - The CPU executes the instruction that was decoded in the previous step.

```
Let's look at the following flow:
```
<flowFDE align="left">
<img width="6000" src="src/assets/img/flowFDE.png">
</flowFDE>

To better understand what FDE is, we can compare CPU to a chef preparing a recipe. In this case:

**Fetch:**
The chef fetches the recipe from his recipe book.
The CPU fetches the next instruction from memory (RAM).

**Decode:**
The Chef reads the instruction in his book, such as ‘Boil the water’ or ‘Chop the vegetables’ The CPU decodes the instructions to understand what needs to be done, such as ‘make the sum of 3+4’.

**Execute:**
The Chef performs the action of putting the water on to boil and cutting the vegetables.
The CPU performs the mathematical operation of adding 3+4=7.

When this task is completed, the processor returns to the starting point and searches for the next instruction in RAM,
in the same way that the chef follows the next steps of his recipe until he has gone through all the instructions

### Why the FDE is important?
Once we understand this process, writing more precise code can become an easier task.
In addition, it can make it easier to understand problems that are related to instructions.

source: [Ada Computer Science](https://adacomputerscience.org/concepts/arch_fe_cycle)


## BDI (Belief Desire Intention)
BDI is an approach used for decision-making applied to artificial intelligence agents.
This model has three pillars that guide how to apply it.

**Belief -** This represents the agent's knowledge base.

**Desires -** This is the objective that the agent wants to achieve.

**Intentions -** This can be defined as the action plan or path that the agent will take to achieve the goal.

### What would the BDI model look like applied to a chatbot?
Let's imagine that you work for a bank and are responsible for implementing electronic customer service in the bank's app.
In this case, you could use the BDI model to interact with the bank's customers. Giving the chatbot a knowledge base, such as which problems it can solve by guiding customers within the app, for example blocking/unblocking cards.

source: [Learn Microsoft](https://learn.microsoft.com/en-us/archive/msdn-magazine/2019/january/machine-learning-leveraging-the-beliefs-desires-intentions-agent-architecture)


## The C programming language

The C language is a programming language developed in the 1970s by Dennis Ritchie.
It is known for its high efficiency in low-level communication with hardware. The C language has been widely used to create other operating systems as well as influencing other programming languages such as Java and C++.
Using the procedural programming paradigm, C was created with the main objective of facilitating the creation of extensive programmes.

The C programming language is currently in its international version C17 (ISO/IEC 9899:2018) released in June 2018, replacing version C11 (ISO/IEC 9899:2011).

source: [Wikipedia](https://en.wikipedia.org/wiki/C_(programming_language))

## POST (Power On Self Test)
The Power On Self Test is a sequence of tests that is carried out the moment a computer is switched on.
This sequence of tests that the BIOS performs on the hardware aims to ensure that all the components are working correctly so that the operating system can be loaded.
for the operating system to load.

If a problem is detected during POST, the BIOS emits a sequence of beeps to alert the user that something isn't working.

Other electronic devices also use POST to ensure their proper functioning, such as some medical equipment and aeroplanes.
Similar to computers, this self-test routine is commonly applied the moment the device is initialised.

source: [Wikipedia](https://en.wikipedia.org/wiki/Power-on_self-test)

## Machine code vs assembly
Machine code and assembly languages are used to create very low-level computer programmes, close to hardware communication, but these languages differ.

* **Machine Code:** This is a programming language containing instructions that the processor can understand directly, represented in binary numbers (0s and 1s). Each machine code command corresponds to a specific operation that the processor performs. Due to the complexity of reading it for humans, we can compare it to a sequence of commands in a language that only the machine understands, without any translation.


* **Assembly:** This is a programming language at a ‘level above’ machine code. Instead of using binary numbers, assembly language uses mnemonics (words or abbreviations) to represent machine code instructions. For example, ‘MOV’ can mean ‘move’ a value. Although it is still considered a low-level language, assembly is more human-readable than pure machine code.

An analogy to understand this would be to think of machine code as your home address but written in barcode, while assembly would be that same address written in common words but more abbreviated due to its syntax (mnemonics).
Both have the same purpose, but assembly is easier to understand.

source: [Wikipedia](https://en.wikipedia.org/wiki/Machine_code)

---