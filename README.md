# Procmarker
Program to flag Pascal programs for begin / end statements in procedures and functions

# Introduction
If you have ever worked on a reasonable or larger sized Pascal program where you have very long procedures or functions - or nested procedures and functions - remembering where the start of one that has nested functions and procs inside of it, it may be difficult to tell where you are in one, or if looking at the end of a procedure or function, which one it is. Well, Procmarker will try to fix that. Procmarker will read a program - program, unit, library, etc. - and every include file, and if there is at least one nested procedure or function before the first BEGIN (or there are more than about 60 lines between the signature and the BEGIN), it will mark that with its name as a comment. When Procmarker gets to the last END it will mark that too.

Well, at least it will once I have written it. That may take a while, but I have an advantage. I did some work on a small full Pascal compiler, and I can use the scanner and (to a limited degree) the parser to follow a program through its operations to find the information.

More to follow.

Paul Robinson
October 10, 2024
