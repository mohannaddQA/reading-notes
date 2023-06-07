# EXPRESS , TDD , CI-CD , NPM

## 1- Midleware

### Explain middleware, answer as though I were a non-technical recruiter ??

so basically middlewares are in-between functions that do a certain task.
for example , if the user wanted to send a message to someone on the website, first a request will be sent but before the response we have to make sure ⇒ is he authenticated ? is he on the friends list ?
**_this is done by middleware functions_**
these functions will get executed before the server sends the response , and the response could change depending on the result of these middleware functions.

## 2- express js

**_it's the most popular framework for Node.js_**

### Express is “unopinionated.” What does that mean?

it means that it doesn't force a specific structure that the developer have to work with, It allows developers the freedom to structure their code how they choose instead of forcing a particular code structure. One place where this un-opinionated idea can be seen is with the application of middleware. Middleware allows for operations to be performed on requests and responses

### What is a module and why is modularity useful to us as developers?

A module is like a box of code (codded file) that contains related functions, classes, or variables and other stuff. It helps us organize and separate our code into smaller, reusable parts.
for example, you have a feature that you created from scratch, and you want to use it in multiple projects in the future.
it's not a good practice to rewrite the same code again and again, you can simply create a file that will contain this feature (a module)
and import the module to whatever project you need.
in fact, this idea is the basic idea behind packages and libraries, **always reuse code when you can**

## NPM

### What version of npm are you running on your machine?

`9.5.0 `

### What command would you type to install a library/package called ‘jshint’ into your node project?

`npm i jshint`

## TTD

### Explain why tests are important. Please explain as though I were your non technical elder?

Tests are like checks we perform to make sure that something is working correctly. In the context of software development, tests are like a safety net that helps us ensure that our software functions as intended. They give us confidence in the software, help us find and prevent problems, ensure correctness. and we must make sure that the software is working as we want so the client is happy.

### What are three expected benefits of testing?

1.  Bug Detection: Testing helps identify and catch bugs or issues in the software, allowing developers to address them before they impact users.
2.  Software Reliability: Testing ensures that the software functions correctly and reliably, providing confidence to users that it will perform as expected.
3.  Code Maintenance: by serving as a safety net, enabling developers to make changes or improvements without breaking existing functionality.

### Name at lest 2 individual pitfalls and at least 2 team pitfalls commonly encountered while writing tests ?

still i didn't write any test myself or with a team but i will make sure to update it .

## CI/CD

### What are three benefits of Continuous Integration?

1.  Early Detection of Integration Issues: CI allows for frequent and automated integration of code changes into a shared repository. It helps catch integration issues early on by quickly identifying conflicts, build failures, or compatibility problems between different parts of the codebase.
2.  Faster Feedback Loop: CI provides a fast feedback loop by automatically building and testing code changes. Developers receive prompt feedback on the impact of their changes, allowing them to address issues and make necessary adjustments promptly. This speeds up the development cycle and reduces the time between making changes and identifying potential problems.
3.  Improved Code Quality and Stability: With CI, code changes are regularly tested, ensuring that new features or bug fixes do not introduce regressions or break existing functionality. It promotes better code quality, stability, and reliability by enforcing consistent testing and quality control measures.

### What is the difference between Continuos Delivery and Continuous Deployment?

Continuous Delivery (CD): Continuous Delivery is an approach where software is built, tested, and prepared for release in an automated and frequent manner. It focuses on ensuring that the software can be deployed to a production-like environment at any given point in time. With Continuous Delivery, the software is ready for release, but the actual release decision is made manually.

Continuous Deployment (CD): Continuous Deployment takes Continuous Delivery a step further. In Continuous Deployment, the software is not only built, tested, and prepared for release automatically but is also automatically deployed to production once it passes all the necessary tests. This means that every successful change or update to the software is automatically released and made available to users without manual intervention.

In summary, the main difference between Continuous Delivery and Continuous Deployment lies in the release process. Continuous Delivery prepares the software for release but requires a manual decision to actually release it, while Continuous Deployment automatically deploys the software to production once it passes all tests, without the need for manual intervention.

### Explain how GitHub fits into this process assuming the listener comes from a non-technical background

With tools like GitHub Actions or integrations with CI/CD platforms, developers can automate the process of building, testing, and deploying their code.
so basically it provides simple tools to do the CI/CD
