
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



