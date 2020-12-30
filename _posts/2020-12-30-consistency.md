---
layout: post
title: "6. Repetitive commands & the importance of consistency "
description: "consistency"
keywords: "loops, foreach, consistency"
---
**Code speak**: How to loop over variables, looping, foreach
**Context Example**: How to be be more consistent when coding repetitive tasks 

# Consistency and avoiding errors is key in coding
In some jobs, it’s important to ensure consistency and minimizing the risk of errors. In coding, we'd like to do the same thing, especially when we are doing repetitive tasks.

_To do this in coding, we can use loops._

```stata
forvalues x=1/25
  gen bagel `x'=plain if marmalade==`x'
```
## Break down 
* forvalues is a command commonly used in coding repetitive tasks
* 1/25 means we want to list 1-25 values in increments of 1 
* gen means we want to _generate_ or create a new variable called bagel, that will represent _plain_ (or contain the value plain) **IF** the marmalade variable is equal to ``x'`
* == means "equal to". It's a type of [syntax](https://www.stata.com/manuals13/psyntax.pdf)
* `x'` means . _Note_: You must  

## Practical takeaways 
* Consider using [loops](https://datacarpentry.org/stata-economics/06-loops/) for any tasks you have to repeat 2+ 
* Looping helps you achieve consistency and reduce risk of coding errors (not necessarily to save on typing)

###### Sources: 
https://datacarpentry.org/stata-economics/06-loops/
https://data.library.virginia.edu/stata-basics-foreach-and-forvalues/
