# clean-code-summary
Clean code by Robert C. Martin - summary

### Chapter 1: Clean code

-This first chapter is all about knowing the difference between bad and good code. How to find bad code and transform it into good code. 

-First thing is how bad code is written. Usually is the need to rush the product to market, to meet the schedule proposed and mostly laziness. We all have done this things and when we have the time to check the code we just leave it for another day because we know it's more difficulty to rewrite code that is bad then actually write good code in the first place. 

-Bad code and productivity are two different things over time. If a project starts with bad code you know you are just add more work in the future so as the project goes the bad code will rise and the productivity will go lower until the point where it's just impossible to write new code without rewrite all the bad code. As the example given in the book, a company as rushed a product to market and at the time could be the best product in the market but when they start adding new features the code started become even more bad that was impossible to manage such a messy code and brought the company to bankruptcy.

-Always be the first to say that it's better to add more days to the task so you can have a readable and manageable code. Delaying the deadline can save time and money by just writing good code, because bad code will just make you write more bad code until you go crazy. 

-A side all rules and principles if a code isn't tested isn't clean code. Every code should be test to be certain that the code actually works and does what is expected to do. The programmer have to care of the code, do it with passion, take time to read every line and rewrite if needed including making all the tests.  

-The principles of clean code are simple, follow all the rules, be meticulous, be precise in every name you give, everything in your code should have only one responsibility and be as simple as possible. There are four rules for simple code:
* Run all the tasks;
* Contains no duplication;
* Expresses all the design ideas that are in the system;
* Minimizes the number of entities such as classes, methods, functions, and the like.

-The boy scout rule applies to clean code, so it's not enough writing good code but you need to maintain it and keep it clean too.

	Leave the campground cleaner than you found it. (The boy scout rule)
As Robert says "If we all checked-in our code a little cleaner than when we checked it out, the code simply could not rot."

### Chapter 2: Meaningful Names

-Like clean code, choosing good names can be hard but in the end saves you a lot of time, especially when you work with others programmers. Take time to think about good names, and give them context so when you read them the next you will need just a second to understand why it exists and what it does.


-To choose a good name you need to be careful not to give names with little differences so in the future you might confuse them. Choose names that people can really pronounce without sound like an idiot as an example in the book "Well, over here on the bee cee arr three cee enn tee we have a pee ess zee kyew int, see?". Use names that you can easily search for, like names with more than 4 letters would be nice.

-As author says "One difference between a smart programmer and a professional programmer is that the professional understands that clarity is king". When you are working with colleagues you need to give names that everyone understand so if you are thinking about some jokes to name think twice.
