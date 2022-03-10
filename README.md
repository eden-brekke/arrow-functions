# arrow-functions

This assignment is designed to introduce you to some features in [ECMAScript 2015](https://www.ecma-international.org/ecma-262/6.0/){:target="_blank"}, otherwise known as ES6. From this point on, you are expected to use these features.

## Overview: Arrow Functions

- [MDN docs](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/Arrow_functions){:target="_blank"}
- [caniuse.com](https://caniuse.com/#search=arrow%20functions){:target="_blank"}

By now you should be comfortable writing [function expressions](https://developer.mozilla.org/en-US/docs/web/JavaScript/Reference/Operators/function){:target="_blank"} and [function declarations](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/function){:target="_blank"}. Arrow functions are a shorter, more concise way to write a JavaScript function. The syntax might seem strange at first, so try to use arrow functions wherever you can and they will become second nature in no time.

There are a few caveats with arrow functions, though. Most importantly, the `this` context is not reset within an arrow function. The value of `this` is therefore the same as the `this` of the enclosing scope (the surrounding non-arrow function). If there isn't a non-arrow function scope surrounding, the `this` context will be, in the browser, the global window object.

Why does this happen? It happens because arrow functions retain the `this` value of the enclosing functional scope. Therefore, you will want to avoid using an arrow function in a constructor (where we need the contextual `this` to be the object we are building) or any method that needs to use `this` to behave properly.

## Assignment Tasks

1. Create a new repo in your GitHub account called `arrow-functions`. Clone the empty repo to your dev environment.
1. Navigate to the `prework` folder in the root directory of the class repository.  Then navigate into the `arrow-functions` folder.
1. Copy the contents of the folder named `starter-code` into your newly-created repo. Make an initial commit with the unchanged starter code. 
1. Proceed to work on a well-named branch. As you work, remember to add, commit, and push regularly.
1. The `app.js` file contains examples of function expressions, as you are accustomed to seeing. Work through steps 1-9, reading the notes and reviewing the refactored samples. 
1. For each of these steps, uncomment the console.log line. Open the `index.html` file in the browser and verify the correct output in the developer console.
1. To complete step 10, refactor the function expressions one at a time. Uncomment the console.log line and use it to check that the output is the same after you have completed the refactoring process.
1. To complete step 11, uncomment the two console.log lines and observe the output in the developer console in the browser. Answer the corresponding questions.

## Additional resources

- ["JavaScript Arrow Functions" by Wes Bos](https://wesbos.com/arrow-functions/){:target="_blank"}

## Submission Instructions

1. When finished, make a PR from your branch to main, and merge it.
1. Submit a link to your PR. You can link to a pull request even if the pull request is already merged or closed.
1. Add a comment in your Canvas assignment which includes the following:
    - A question within the context of today's lab assignment
       - I didn't have too many questions in regards to this lab, I was a little confused about refactoring the functions into arrow functions in the context of knowing that arrow functions weren't meant for that purpose. However, through working through it I think I understand the purpose. Since some of them didn't return a straight "syntax error" within the console instead just didn't properly call aspects of the code that it would, had it been a normal function declaration. This will help down the line in identifying errors when we're using arrow functions in other programs, and may forget the small limitations of them.
    - An observation about the lab assignment, or related 'Ah-hah!' moment
        - I really liked the scope versus scopeArrow calls at the end of the lab where within the arrow function usage of the term 'this' you see the console log call to the window object. It really solidified that when using arrow functions you lose the reference to the object and can no longer use 'this' effectively. 
    - How long you spent working on this assignment
        - It took me about an hour to work through everything within the lab. 
