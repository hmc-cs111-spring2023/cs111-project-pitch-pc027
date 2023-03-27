# Contract

## Goals

_At a high level, what do you most want to get out of this project, and why?_

I want to design a language that makes sense for non-programmers to explore a DSL as a potential way of guiding people who may feel intimidated by programming to do things they are familiar with programmatically. The language can also be a foray to help people get into programming (similar to the way HTML/CSS are a sort of "jump pad" for learning coding for many people). I am also intrigued by various text processing tools I see on the internet (ex. resume parsing, pdf to word doc, etc.) and would like to explore the domain more through this project.

On a more operational level, I want to complete my project to a point where if I set up the language's peripherals for my user, they can use the language easily even if they are unfamiliar with computer science-specific ideas like compiling. I would also love to show off this project in my Github profile!

## Concepts / skills

_What concepts and / or skills from class would you like to work on, as part of your
project? Are there any concepts / skills that we haven't covered in class that you would
like to work on, as part of your project (for example, other things related to DSLs that
you have come across, or topics from other classes)? Why are you interested in working on
these things?_

I want to give more time on the parsing process, especially the front/middle "part" of designing external DSLs. I enjoyed the process to implement an external DSL via the Piconot assignment, but didn't have as much time exploring ways to get to my ideal syntax and had to make a lot of adjustments. This will likely involve digging deeper into the parsing libraries. I would also like to be able to evaluate ambiguity in a DSL more intimately - things like left-recursiveness, precedence, and associativity was not at the forefront of my mind in previous homeworks, but is important to critically analyze a DSL.

I have initially chosen to work with Scala because I want to be more familiar with the language and leverage the fact that it is very suitable for creating DSLs. I will also leverage many libraries that were initially built on Java, but should work in Scala. Nonetheless, I have never tried hooking libraries up across language before, so this will be a learning point for me in this project.

## Time management plan

_How do you plan to set aside time outside of class, to work on the project? Are there
intermediate milestones that you can create, to help you make consistent progress?_

I plan to set aside 6-8 hours per week outside of class to work on the project. I will be spreading my time so that I spent at least 1 hour before Wednesday studio sessions so that I can get help quickly on any initial questions I have for the tasks that week. I also plan to write clear documentation as I go in my GitHub repo, as a Wiki page or through markdown docs. This would help me and my review group clearly see my progress within this project.

Here is a timeline that I plan to follow with intermediate milestones as indicated in bold.

Mar 26 | project plan and contract (this github)
    
Apr 2 |
- **create first draft of ideal dsl syntax and AST**
- deeper research into libraries for operations to parse documents in Scala and Java
- **set up project and test functions**: writing the necessary operations in GPL with the help of imported libraries, ex. I/O: open and read file in (format) + generate new file in same format
- design start symbol, production rules, terminals from ideal syntax to formalize the DSL

Apr 9 |
- **implement parsers to generate AST for basic workflow**
-	edit ideal syntax to balance with capabilities of Scala
-	implement functions needed for other workflows
- stretch goal for week: complete “base level” requirements for dsl and project - takes a file written in my DSL with keywords and instructions for organization, another word file as doc to organize, and outputs a file as structured based on dsl commands.

Apr 16 | 
- **Complete base level requirements for dsl/project, and revise documentation in and outside of code for ease of use.**

Apr 23 | 
- **Complete low-difficulty extensions to project** - ex. handling other documentation formats
- (Stretch goal) Complete other extensions to project depending on time. I would like to create a CLI or GUI of some sort!

Apr 28 | Complete any started extensions to the best of my capabilities!

## Teamwork plan

_If you plan to work with someone else on the project, what is your plan for
collaborating? What part(s) do you think you might do together? What part(s) are you
considering doing separately? How will you hold one another accountable to make regular
progress?_

(working individually)

## Critique plan

_What will you do to make sure that you can give consistent and actionable feedback to
other people in the class?_

In terms of consistency, I will read the week's work early over the weekend if possible to generate some initial discussion questions in my head before heading into review groups on Mondays. Depending on the critique format, I may also create a google document for myself to keep track of any domain knowledge/assumptions of the project I learn along the way so that my feedback is created in consideration of those ideas. When giving comments, I would also want to list out any assumptions I am making so that the person working on the project can gain more insight to any points of confusion that may not be immediately apparent to a potential new implementer or end users of the language. 

To make my feedback actionable, I will make sure that my comments are directed at the content of the project and that my discussion is as specific and constructive as responsible. When talking about language design, I can suggest ways to document or adjust the code to make things clearer if I am familiar with the domain or the intended end-users. When discussion implementation, I can suggest useful packages (or ways to use the ones already imported) to help reduce complexity in system aspects of the project. I will also use the compliment-sandwich format to recognize any peripheral work related to my feedback that is done well.

## Success

_At the end of the semester, what would you be proud to show or tell someone about your
project?_

I would be proud to show off a working DSL that would work really well for making first-draft outlines for academic papers/digital articles. It would be awesome if my DSL worked for other types of organized documents with more definitive structure (ex. itineraries), even if my DSL is less focused on that aspect. I would also be proud to tell someone that I wrestled with parsing, especially creating a system that reports errors as finely as possible given the general difficulty of creating error messaging along with parsers. Since this is my interview project, I would also be proud to show it off to my interviewee and hopefully see her use it without much confusion or hassle. 

I think it would also be cool to know more about Scala projects and sbt in general, similar to the way Java tend to have a basic file structure/workflow applicable to many projects. If I have time, I would also want to do some quick user testing during this project to make sure my ideal syntax makes sense for non-programmers - and the results from those studies would be an interesting and motivating addition to my project.

## Assessment

_Looking over your responses to the previous questions, what would you consider to be an
"A-" for your project? What would you consider to be an "A"?_

Some lower difficulty extensions would be extending the DSL to include multiple file formats (.doc, .pdf, .txt). Java has many libraries for parsing these different file types, but they do require different operations to be written. Another low-hanging fruit would be to handle embedded image data, or a user testing session with my interviewee to iterate on my ideal syntax.

Higher complexity extensions include implementing a CLI/GUI wrapper over the DSL. At the end of the day, it might simply be easier for non-programmer end-users to have more visual cues to reassure them about the validity of their writing, and if invalid, an easy way to see which general parts are missing for the program they are writing to work. I also came to learn that videos can be embedded in many document formats - exploring a simple way of parsing and placing videos in a generated document would be another difficult, yet functionally rewarding extension for the project.

I consider an A- to be completing 1-2 categories of the lower difficulty goals. An A would be completing all lower difficulty goals to a near-complete extent, or 1 high difficulty goal.
