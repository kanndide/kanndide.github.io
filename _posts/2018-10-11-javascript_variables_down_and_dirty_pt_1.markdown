---
layout: post
title:      "JavaScript Variables, Down and Dirty pt. 1"
date:       2018-10-12 01:15:44 +0000
permalink:  javascript_variables_down_and_dirty_pt_1
---


### First, the Basics

When I first started learning JavaScript one of the things that stumped me initially (and still occaisonally) was variables. Going from Ruby and JavaScript was like night and day. At least they use the word 'variable'.  

JavaScript has 3 different kinds on variables, `var`, `let`, and `const`. Prior to ES6 (ECMAScript 2015) the only way to declare a variable was with `var`. Since eveything is moving towards ES6 the preferred way to declare variables is it use `let` or `const` instead. Outside of working on legacy code, it looks like `var` can be, and should be, completely avoided.  

There are a few key differences between the three concerning scope, whether or not they can be hoisted, reassigned or redeclared.  

| Variable | Scope | Hoisting | Reassign? | Redeclare? |
| :--------: | :------: | :---------: | :----------: | :----------: |
| `var`       | fn()       | Yes            | Yes              | Yes              |
| `let`        | Block  | No             | Yes              | No                |
|`const`  | Block   | No             | No               | No                |

With this in mind it would appear to be preferable to utilize `const` when capable and use `let` inside of loops or any function that would reassign the value of the variable.  

Notice that `var` is function scoped. This means that if you declare a variable with `var` globally, it won't be recognized locally within a function. This is not the case with `let` and `const`. They are *block* scoped. This means that a new local scope is created for every type of block, to include any type of loop (`if`, `for`, or `while`). The stricter rules around `let` and `const` are what make them the more desirable terms to use. This makes understanding how they are going to be utilized that much easier and helps limit some debugging down the line.  

Whether or not a variable can be reassigned a value or completely redeclared is pretty self explanatory and easy to remember with `let` and `const`. Think of `const` as constant, never changing. It can be neither reassigned or redeclared. It is what it is, constantly. `let` on the other hand allows you to reassign it, making it the ideal choice for loops and conditionals. However, it can not be redeclared.  

Scope and hoisting are a different story all together and one I plan on getting into in the next blog post. 

