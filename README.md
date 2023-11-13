
# 🥋 All Chapter

| Chapter - | Topics             | 
| --------- | ------------------ |
| Chapter 1 | Code Quality Gates | 
| Chapter 2 | Coding Standard    |
| Chapter 3 | Code Review        |
| Chapter 4 | Testing Overview   |
| Chapter 5 | Unit Testing       |


## Code Quality Gates (The High Cost of Bugs)

<p align="justify">
So our plan for this lecture. We will talk about the sequence of bugs in the software. We will take a look on three different samples and we will talk about how much the error can cost for the company. Then we will talk about bug fixing efforts. After that, the advantage of early detection of bugs and in the end it rules so we can afford to prevent bugs. And we have to remember that bugs are unavoidable. But what we can do. Let's start from samples and the first one it's the Knight Capital Case. Knight Capital Group was American global financial service from engaging in market making electronic execution and institutional sales and trading in 2012. Nike was the largest trader in the US acquired this with the market share of around 70 percent of the New York Stock Exchange. There was a deployment mistake caught before algorithm verification on the testing environment was executed on the production. So when exchange was open this algorithm started buying sales. 
</p>

<p align="justify">
  And during the 45 minutes it bought the stocks for four billions of dollars and options that companies should solve this issue somehow and have to sell these stocks. And this mistake was cost four hundred fifty millions of united states dollars and just 45 minutes of selling and buying stocks. After that this company tried to solve the issue by buying these stocks again and in the end the company was the whole company was bought by another company. And right now there is. No such company on the market so this was a very expensive bug for this company. Another case is that Ariane five case its European rocket program which worth 7 billions of dollars as the first rocket was explored and why it was exported. After a few seconds after when it started there was error in software. When the 64-bit floating-point number was converted to a sixteen beat signed integer this code wasn't wrapped in try-catch section and the backup version of the code which should handle this problem was implemented
in the same way and software was turned off when it tried to convert this number and the rocket was destroyed. So the loss of the 500 million rocket made this possibly the most expensive computer bug in history. 
</p>

<p align="justify">
  And the third sample which I want to show you it's something that the cost of software defect can't be measured in dollars. Spare of fatal crashes that claimed the lives of three hundred forty-six people. There was a problem with Boeing 737 Max. And the first crash was an October 2018 and after a few months there was another crash. When the second plane was destroyed and the problem was in the outsourcing of software. Company bought the software in company where developers were paid by nine dollars an hour. So the code wasn't asked well and the cause of this badly written code was a crash of two planes with these death. Bug fixing efforts. What do we need. Do we need to fix the bug. So where bug was discovered during the testing. We need to spend a lot of time before reproduces this bug. 
</p>

<p align="justify">
  After that register this bug and need to assign to develop this bug. When we are assigned to. We need to discuss what was wrong and how we can solve the bug. And after that it did take some time for fixing it. So from my experience, it takes a lot of time for all of these steps to register bug, reproduce. Specially reproducing on the scent was one call it should be fix it. After that we need to see which is the context switch to another task or from another task. Try to fix these bugs and after that, we need to double-tested, verify and close. So all these steps require a lot of time. Also we need to remember that fixing familiar code. It's much more easier than fixing unfamiliar code. So if you work with code today we know how it works and it's much easier to solve the problem in code we know. But in code, which was developed a few weeks, months, a year ago - takes more time. So we need to remember that code that we need to remember is that fixing a bug today is cheaper than fixing
this bug tomorrow. 
</p>

<p align="justify">
  And here we can check that during the software development lifecycle on the each stage it takes a lot sometimes. So during the implementation stage fixing is a bug can take five times more efforts than on design stage and is the same time maintainance when you will find this bug on the maintenance stage it will can take 100 times more effort to solve the problem than during a design. So the latest time when you discover and try to fix this bug it will take more time and effort and it will take additional money. We can't avoid bugs. It's impossible to write an ideal code but what we need to remember that fixing bug is expensive. And we need to do everything to prevent bugs. So how can we do that. A lot of steps and rules we can follow. For example we can write a unit test. We can great code convention and try to follow this convention. Also, there are tools for static code analysis and practices such as continues integration and continuous delivery which help us to do the best we can and write much more cleaner code. That's why we had to use best practices and tools and try to do the best what we can.
</p>

## COde Quality Gates (Code Quality)

<P align="justify">
We'll talk about Code quality. What is Code quality and why it's so important. Let's take a look on our plan today. We will talk about what Scott's quality characteristic of a good coach why it's important time and cost. And we'll talk about general guidelines how we can use it. Also we will cover tools which help us to do our code better. So first of all let's take a look on this image. 
</P>

<p align="center">
  <img src="https://github.com/bahrulrozak/Best-Practices-In-Software-Development/assets/141661830/abedf82c-ef73-487a-b3af-c83c35cf37dd" alt="Centered Image">
</p>

<p align="justify">
Or do we see. Usually it's a very common case when we had to developers and the both of them working on the same court. One created code and nobody knows how this court works. Even the man who created it so it's a problem. And we need to avoid such problems. So talking about code quality we can split it into two different parts. It's a far from code quality and structural code quality. So what is functional code quality functional code quality. It's a meeting two functional requirements we have requirements to create some software and we have some requirements functional requirements. What the software should to do this quarter will be high quality if we will implement these requirements. And this also will do what should do. We can use the unit test to implement functionality as it's expected. The structural code quality it's how well is the sofa code is the region. How how do you write this code and did you follow our guidelines in the process or not. So the next what we're going to discuss we mostly we will talk about structural code. How do you write it. 
</p>
<p align="justify">
How do you write the code maintainable and the code you can use. We all talk about structural code quality mostly in the next part of this section so to understand the importance of this code to we can describe the difference in two terms such as reading the code and working code so working code because some requirements. And in case the fulfill its these requirements because as that code is working and it work with what should you do the code develop its a regional code. So it can be great but it might not work as expected. How can we say that God is good. We need to take on some requirements so or characteristics of a good code. So the most important is it works because the requirements go to works and the requirements are fulfilled is a great but another important part is a thousand to look at this court. Really is very important when you can take a look at the code and to understand how it works code looks beautiful without different without the useless comments without users parts of code and they do need to spend some time for understanding how it works. 
</p>
<p align="justify">
It's a part of easy to read so you can read it as a novel as a text or some nonfiction literature you read and you understand what is there and how it works why it works in this way and this why it should be simple and single single good means without copy paste. You don't need to carp is caught in different place and it should do some one single task. Its single responsibility. So when you create a function it should do just what the swatch is created for nothing else then it's much more easy to understand this function and test. So in this case you will create software with an approach which calls testable in mind. It means then when you create unit tests for this code you will create your code easier to read easier to understand and easier to test because that I think is important stage. And when you create the code with this approach you will try to do it without some useless dependencies or resource on global variables. You will try to do it as easily as it's possible and the result of the steps is is in maintaining and changing. So we have a code. 
</p>
<p align="justify">
We have some new requirements or we knew about a new mark. We need to solve this bug and if caught was written in a good style and it's a good code we can easy to change samples or updates on functionalities. Why is it important. So let's take a look. How we work with code I will tell you a truth about writing of course when you are a software developer. So mostly you don't write code we can see here that 85 percent of the time we just understand in court.
  
<p align="center">
  <img src="https://github.com/bahrulrozak/Best-Practices-In-Software-Development/assets/141661830/ad10da70-a010-4370-bc16-e9b0c4694600">
</p>

We read what was already written. From my experience I can say that sometimes you can spend a day and just write one or two lines of court and all the time you spend for reading because the court understand how it was written why it was written in this way and what requirements this court tried to implement and how it works. And also that when you understand how it works then you can change something you can implement new requirements. That's why right in court it takes us to persons of our time. Also we have more defined out of existence court ban. We have already written code. We will find the bank. We can modify already existing code and add something new. But mostly we read this code of causes. The percentage is depends on a time of lifecycle development of your project. 
</p>
  
<p align="justify">If you just started your project you will write new code mostly but with the time in a few weeks months there will be a lot of code and you will read code of other developers because mostly you will work in team with other developers. Why is important. Of course, it's about who court quality may and I will sure that it will lead to the next problem it's finding out the facts.</p>

<p align="justify">So as I've mentioned before code works when it implements some functional requirements. If we write code better it might not implement its requirements and your sorter won't work as expected because of some problems. And the next one it's a cost and time to make changes. It calls meant maintainability.</p>

<p align="justify">How much time do you need to implement some new feature or fix a bug if your code was written. Well according to some code style you can fix it in a short time and maintain a long period of time. But if your code was created without code qualities without code conventions I'd got style and you don't know how it works. You can spend it will spend more time to understand it for good quality may cause additional application performance issues which we need to remember about it. Because the useless part of code may do some users request in network and to take some time and you will decrease the quality of your application in general so also modify ability it's a requirement for a code which calls how easy it can extend or update your code so if you out new requirements you need to implement some new functionality.</p>

<p align="justify">You need to understand this code and modify ability will show you how much time you need to implement new functionality. Also poor code quality will increase your technical that technical that it's here. It's what you should do. But right now you have the time or you can do it. For example use keeping writing unit tests. It may be your technical debt that you will need implemented in the future. But right now you can do it. Also some problems with your code. The same application performance it can be your technical debt which you should do handle.</p>

<p align="justify">And so in the future and many other programs can be created by poor code quality him so keeping code quality it's the commitment of each team member of your team his teammates should understand why we have to do the best we can. Why we can't. Why do we have to create high quality code and what is the reason we need it. Agreed and then motivate people to write this code according to our agreement according to our code style because of we will know that in the future it will decrease the time for supporting and maintaining this code quality and it should be your regular activity. It should be your habit every day when you write code you write it with these code style and try to do it as good as possible without wasting time for some additional talking and discussion of why it should be done in this way or another way.</p>

<p align="justify">So how can we do it. Do the court with the high quality we can follow the next rules or best practices. 

<p align="center">
  <img src="https://github.com/bahrulrozak/Best-Practices-In-Software-Development/assets/141661830/1d0214d4-2d27-490d-b862-f3217678e762">
</p>
And the first one is a code review code review is a process when you manually check your code is it okay. Is it. According to requirements you discussed. And if everything okay you can manage it or not. If not you can discuss it and solve problems.</p>

<p align="justify">Another technique is the unit testing unit test will fulfill to your functional requirements so you know what you should implement how a trick works and what you create unit test which tests your functionality and you're expecting and and other techniques such as functional testing or continuous integration and continuous delivery. Also we will cover these techniques such as the code review process testing Continuous Integration stated code analysis. It's important part of automating automated analysis of your code and bit of development and also training and onboarding. You need to share knowledge in your team how it should be done and it will help for each team mates to do to fall off the code their requirements.</p>

<p align="justify">Let's talk about general recommendation and of course this follow coding standards in India. Create your standards for your own team for your own project and each teammate should follow those standards. Also need to try to follow design principles such as this solid or another piece. Just keep it simple. We need to create a code is a minimum effort. Why do we need it. Because it is the same requirements. Each developer can create a solution in absolutely another way. It would be another record with another syncs with another minds behind and it can implement as he or she wants. So we needed to do it as simple as possible to reduce the amount of time for understand is this code.</p>

<p align="justify">Of course we need to introduce code review practice on our project to check the code. And was it region as you expect it or not. And a good practice is introducing automated unit tests or integration test for your code. And it will increase your code quality as much as possible and a severe developer we do not want to spend a lot of our time in case if we can delegated to computers so actually what can computer do it should do. And in this case we have tools to assist. There are a lot of different tools for different programming languages. You can use for example sonar cube is a very popular tool. We should all follow your rules. You will create some rules and these two can check your code according your rules as you want this code should be done.</p>

<p align="justify">And the conclusion of what is important. It's important for each developer it should understand the importance of code quality. Why do we need to follow code convention and try to write code as good as possible. We need the defining guidelines for the project how we are going to create a report and make sure you follow them. So is developer should have to follow these guidelines and try to write code according to this code style and act on issues in your code. It doesn't matter created you co-star or guideline it doesn't matter in case you don't follow this convention and you do not act on issues. So there wasn't create a unit test or code was written not as they expect you have to act and prevent such problems in the future.</p>



