Questions:
1.When this code is run in Node, e.g. node index.js, what are the two stages of execution for this file called, and which order do they happen in?
    The first stage is compiling and hoisting.

    The second stage is interpretation and execution.

2. Write an explanation, using as much space as you need, relating to how the first stage of execution for this file operates.
    The first stage of execution begins with finding all declarations and associating them with their scopes.
    Node hoists the declarations including functions to the top of it's scope
        line 3: var foo is hoisted to the top and awaits assignment


3.Write an explanation, using as much space as you need, relating to how the second stage of execution for this file operates.
    Javascript engine looks for right-hand assignment. This assignment takes place in the 2nd stage of execution.


4.During the second stage of execution how many scopes have been registered by the engine?
3 scopes have been registered

Which segments of the code do they belong to?
Please identify any variables/refs and which scope each belongs to?
global scope: var foo = 'bar'
    function bar()

function scope: var foo = 'baz'
    function baz belongs to function bar()
    foo = 'bam'; bam = 'yay'; - both belong to function baz scope

5. When line 13 invokes the baz function, which foo will be assigned a value of bam? More specifically, bam will be assigned to the foo in ??? scope. Give a brief description in your own words to support your conclusion.

    

6. Which scope, if any, will the variable bam on line 11 be registered to when the first stage of execution occurs on this file? Provide a brief description in your own words to support your conclusion.

7. For each line, 16 through 19, what is the return value for each?

