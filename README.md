# spa
TIC2003 Software Development Project

Some companies spend as much as 80% of software budgets on software maintenance. During software maintenance, programmers spend almost 50% of the time trying to understand a program. Therefore, methods and tools that can ease program understanding have a potential to substantially cut development costs.

During program maintenance, programmers often try to locate code relevant to the maintenance task in hand. 

A Static Program Analyzer (SPA for short) is an interactive tool that automatically answers queries about programs. In this project, we design and implement an SPA for a simple source language.

To answer program queries, the SPA must first analyze a source program and extract relevant program design entities, abstractions that are stored in a Database. Secondly, the SPA must provide the user with means to ask questions about programs. These questions are written in a formal Program Query Language (PQL). SPA processes the PQL queries based on the information found in the Database and returns the results to the user.

Refer to the report for the main components of SPA. The users use the User Interface (UI) to enter a source program written in a simplified programming language called SIMPLE. SPA Source Processor parses the source program according to the SIMPLE grammar, extracts information, and stores it in Database. These design abstractions include relationships (such as Calls, Modifies, Uses, etc) defined for program design entities (such as procedure, statement, variable). Furthermore, the user inputs queries written in PQL grammar using the SPA’s user interface. The queries are validated and evaluated by a Query Processor (QP). To answer queries, Query Processor makes use of the program design abstractions stored in the Database in table form. Finally, the query results are displayed by the UI to the user.
