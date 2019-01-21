# Clean Code: A Handbook of Agile Software Craftsmanship Summary

[Check out the book!](https://www.goodreads.com/book/show/3735293-clean-code)

**Author:** Robert C. Martin

### Chapter 1: *Clean code*

-This first chapter is all about knowing the difference between bad and good code. How to find bad code and transform it into good code.

-First thing is how bad code is written. Usually is the need to rush the product to market, to meet the schedule proposed and mostly laziness. We all have done this things and when we have the time to check the code we just leave it for another day because we know it's more difficulty to rewrite code that is bad then actually write good code in the first place.

-Bad code and productivity are two different things over time. If a project starts with bad code you know you are just add more work in the future so as the project goes the bad code will rise and the productivity will go lower until the point where it's just impossible to write new code without rewrite all the bad code. As the example given in the book, a company as rushed a product to market and at the time could be the best product in the market but when they start adding new features the code started become even more bad that was impossible to manage such a messy code and brought the company to bankruptcy.

-Always be the first to say that it's better to add more days to the task so you can have a readable and manageable code. Delaying the deadline can save time and money by just writing good code, because bad code will just make you write more bad code until you go crazy.

-A side all rules and principles if a code isn't tested isn't clean code. Every code should be test to be certain that the code actually works and does what is expected to do. The programmer have to care of the code, do it with passion, take time to read every line and rewrite if needed including making all the tests.  

-The principles of clean code are simple, follow all the rules, be meticulous, be precise in every name you give, everything in your code should have only one responsibility and be as simple as possible. There are four rules for simple code:
* **Run all the tasks**
* **Contains no duplication**
* **Expresses all the design ideas that are in the system**
* **Minimizes the number of entities such as classes, methods, functions, and the like.**

-**The boy scout rule** applies to clean code, so it's not enough writing good code but you need to maintain it and keep it clean too.

    Leave the campground cleaner than you found it. (The boy scout rule)
As Robert says *"If we all checked-in our code a little cleaner than when we checked it out, the code simply could not rot"*.

### Chapter 2: *Meaningful Names*

-Like clean code, choosing good names can be hard but in the end saves you a lot of time, especially when you work with others programmers. Take time to think about good names, and give them context so when you read them the next you will need just a second to understand why it exists and what it does.


-To choose a good name you need to be careful not to give names with little differences so in the future you might confuse them. Choose names that people can really pronounce without sound like an idiot as an example in the book *"Well, over here on the bee cee arr three cee enn tee we have a pee ess zee kyew int, see?"*. Use names that you can easily search for, like names with more than 4 letters would be nice.

-As author says *"One difference between a smart programmer and a professional programmer is that the professional understands that clarity is king"*. When you are working with colleagues you need to give names that everyone understand so if you are thinking about some jokes to name think twice.

### Chapter 3: *Functions*

-Functions are other fundamental part of the code that is very import for keeping the code readable and clean. Like variables, functions are very common along the code, so giving context to function name helps a lot developers to understand what the function does and why it exist.


-When you start coding the most common thing is to write big functions, but you will see that the best is to keep things simple as possible. In this case when you have a big function, the ideal is to refactor the function in small functions. Each one with one story and one purpose, so when you read them in order you will immediately understand what the main function does. This way your code will be more organise and help you prevent using duplications. Also replacing a piece of code for a function is better then just comment the code because you can give a better descriptive name.

-One principle that you should respect about functions is that every functions should have only one job, if one function have more than one job then probably you need to split that function in two or more. The problem is to figure it out what the function was design to do. You can easily find out by read the function and see if you can extract one function from it.

-Regarding the names that you give to each function, this is what you should take in consideration: *"Don’t be afraid to make a name long. A long descriptive name is better than a short enigmatic name. A long descriptive name is better than a long descriptive comment"*.
It's better to take time and think in a good name to your functions, can actually saves time for you and your colleagues.

-Function arguments can bring you a lot of problems, so if you keep functions with no arguments or only one arguments it's perfect. Like Robert C. Martin says: *"One input argument is the next best thing to no arguments"*. Arguments can complicate your tests and they implied a lot of conceptual power, the more arguments the more harder to understand. When it takes a lot of time to understand things you just ignore them and then usually the code you miss is the one that have bugs. Try every time to think twice when create a function with arguments and see if is possible to find a solution that let you just have a simple function with no arguments.

-The objective of a function should only be one, change something or return something. Having both can be confusing to understand the purpose of the function. To handle errors is better use a function only for returning exceptions or error codes.

-Try to respect the **DRY Principle** (Don't repeat yourself). At the beginning most of the developers just write code to put things working but when you are reviewing your code just take some time and clean all does duplications that you have and create small functions for it. Those duplicates can create you a lot of problems and that's why people create principles regarding this problem.

### Chapter 4: *Comments*

-Comments are a bad practice and they will mostly not help you and in the worst case they will lie to you. If you think you need to comment something you already know that you failed to express what your code actually does. Like Robert C. Martin says: *"The proper use of comments is to compensate for our failure to express ourself in code"*. So before writing any comments think where you can express your code better. A comment with time becomes outdated and can only bring you problems and pain in keeping comments in sync with your code. In general comments are just impossible to maintain.

-It's a lot better waste more time in keeping the code clear and understandable then writing comments that can mislead you at any time. Sometimes is even better to not write any comments than just write inappropriate comments. One of the good things about comments is that you know that probably your code need some changes, because what motivates you to write comments is bad code.

-Of course there are times comments are useful, for example: when you need to warn other programmers for a specific change you made, or some consequences of a function. But know with VCS is a lot easier to inform programmers about any change or problem or even a TODO.

-There a lot of types of bad comments, they all represent bad coding, failure in express the meaning of things, misleading others programmers and just pure noise in general. If you are going to comment something make sure that is relate to the code that is near and not global information. Be the most specific as possible, otherwise the code will become just another mess and will lead to disorganization.

-Don't comment functions or variables that are well described with their names, usually will end up writing the same thing twice and the comment will be useless. In general, try to avoid comments as much as possible, they will just make your life harder.

### Chapter 5: *Formatting*

-Probably some tiny details make the difference in the end, like formatting, a space missing can lead to a lot of pain. Formatting code is about communication and what a developers should do best for the business is communicate. Like Robert says: *"Perhaps you thought that “getting it working” was the first order of business for a professional developer. I hope by now, however, that this book has disabused you of that idea"*. The code style and the formatting is so important that can affect future decisions and the maintainability of the code, because you can't change what you don't understand.

-There are some few things that you should consider when you want to make your code formatted, first is vertical vertical formatting. This one is about number of lines that one file have, the overall size of a file. There is not a number where you should guide but the rule is that small files are easier to read than larges files. Still about vertical formatting, try to leave blank lines to separate different groups of thoughts, that way you can understand what is the line of thought for that function. The functions that are related should be near each order if possible and the the most important ones should always be on top.

-About horizontal formatting, is the same thing as vertical formatting, there is no number to guide you but a small line is always easier to read and reten information that a longer line. This limits of characters normally depends on the person or the rules that you set with your time but for example for PHP the limit is usually 120 characters. About the line itself, blank spaces are used to separate elements that are not important to each other, so if two elements are together you already know they are related when reading.

-In general code style is discussed with the team, so all the developers should follow the rules that the team agrees to. That way it's more easy to everyone have the same limits and rules and at end the code is formatting the same way. This is needed because each developer have their own rules.

### Chapter 6: *Objects and Data Structures*

-Is important that each object isn't depending on others objects, you don't want to change one object and then need to replace them in every place where you use them. You need to keep everything independent so you only need to change one thing. It's important to always hide the implementations using abstract interfaces, this way the user can access the data but doesn't know the implementations.

-When naming implementations be as abstract as possible, do not give way data details in functions names for example. Try to give less information as possible.

-In oriented object language it's easier creating new classes without changing existing functions but in the other hand adding a functions is more hard because you need to change all the classes.

-There is one principle that put all this information together, it's called **Law of Demeter** that says:

    Each unit should have only limited knowledge about other units: only units "closely" related to the current unit
Basically a module should only know the basics of the object that manipulates. A module can only use the methods of one object but can't use the methods of objects that are returned by the functions.

    Each unit should only talk to its friends; don't talk to strangers.
    Only talk to your immediate friends.
Conclusion, hide all your objects data and only show methods, this way you can manage your objects and classes more easier.

### Chapter 7: *Error Handling*

-Error Handling is one of those things that all the developers have to do. Can be hard but if something goes wrong you can easily fix it by looking at the error message or error log. Use exceptions to handle your errors, but when you do give some context to it so in future you will know the location and source of the error.

-Try to start with try-catch-finally, that way you can define what the user should expect if something goes wrong.

-Handle errors is about writing robust and clean code and try to separate this handling from the main logic of the code. So you can easily reach the main logic of the code or the error handling.

### Chapter 8: *Boundaries*

-When using third-party code you need to be careful and organize the code very well so when you need to fix errors or update code you know where everything is. Because what is worst than losing time to understand all the code from third-parties? The solution to this problem is just create boundaries between your code and third-party code.

-Before losing time reading documentation and try to understand the third-party code is better to write some tests, that way will be easier to use the code and understand if there is any error or bugs in the code. Also the test let you figure out what the actually part of the code that you need for your project. When there is an update for the API you are using does test will let you know if there are any changes to the code that you are currently using.

-When using code that is most out of our control we should be careful to protect us from changes in the future that can cost a lot of money. That's way there is boundaries, so you can depend in something you have more control over.

### Chapter 9: *Unit Tests*

-**Test Driven-Development** (TDD) is starting to be a more efficient way of coding and be able to create manageable and readable code. The good thing about writing tests is not only to make sure the code does what is meant to do but to be easier at any point change any part of the code and still be possible to just run the test and make sure the things you changed didn't break anything else.

-There are three laws to follow a Test Driven-Development:

   * First Law You may not write production code until you have written a failing unit test.

   * Second Law You may not write more of a unit test than is sufficient to fail, and not compiling is failing.

   * Third Law You may not write more production code than is sufficient to pass the currently failing test.

The focus in TDD is always to have in mind a simple cycle where you write a test then the code to pass the test. Never write production code before writing a test, this way you will write so many tests every day that in the end your code will have tests to cover every bit of code.

-Test code is important as the rest of the code so it's better to keep it clean so your production code can be flexible, maintainable, and reusable. So when you are making changes to the code you can always check by doing the unit test and that way you will be sure that everything is still working as expected.

-All tests need to be clean, readable, small and say a lot with less expressions. Try to keep every test small and testing one thing at the time. Each test should only test one thing, you can use **Build-Operate-Check** pattern to help you with that. With this pattern you should respect three steps:

     1. Build the test data
     2. Operate the test data to run the function you are testing
     3. Check if the results are what you expected


-There are five rules that you should follow to have clean test code, **F.I.R.S.T**:

   * **Fast** Test need to be fast so you can do it more often, if they take to long you will start doing test less often and then bugs will start to emerge.
   * **Independent** Every test should be independent, they should not depend on other test because if somehow one test fails then others will fail too.
   * **Repeatable** Your tests should be repeatable in any environment, can be test environment, production environment, QA environment or even offline.
   * **Self-Validating** Tests should have a boolean output, a test can pass or can fail the test. You shouldn't search for a result on a log file.
   * **Timely** Write test before production code, will be more easier to test the code because you are writing production for a specific test that already exists.
