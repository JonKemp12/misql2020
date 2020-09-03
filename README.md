# MiSQL

### About this repository

This command line utility was first written 15 or 20 years ago for me to practice Java.

Unfortunately, I was (am)  _not_  a skilled Java developer and it is embarrassingly badly written.

I plan, now, to refactor it completely, in "Clean Code" terms with jUnit tests etc until it is something I am proud to own!

## Introduction to MiSQL

TODO: This version will be pure JDBC and (hopefully) driver agnostic. Therefore, this section needs to be re-written as such.

Multi-ISQL is a Java application designed to look like the traditional Sybase (now SAP) ISQL 
utility as much as possible but contains a number of extensions. All of the 
ISQL command line options are allowed but some have yet to be implemented.

MISQL is completely 'stand-alone' and does not require a Sybase installation 
but does require JRE 1.5 or later.

MISQL can be started with no command line options but if started with 
'-U <username>' then it starts as a traditional looking ISQL. 
However it has been extended to:

 * Support connections to multiple servers
 * Directly 'run' script files
 * [Make RPC calls to servers that do not have a language interpreter.]
 * Log result output to named files.
 * Set output format: row and column terminators, vertical rows, prompts etc.
 
All MISQL commands start with : as the first character of a line.
Multiple commands can be on a single line separated by ';'.
The environment variable MISQL_CMD may contain one or more of the MISQL 
commands, separated by ';', which are executed immediately on start up.

### Author
jonkemp12@gmail.com
