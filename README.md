# Calculator Assignment

## Setting up the pipeline
### Basic Setup
To set up the pipeline, I first created a new project in CircleCI and linked a new GitHub repository to it, enabling automatic code pulls for building. I then cloned the provided code, created my `config.yml` file, and defined a new executor based on `cimg/node:21.0`. With these initial steps, the pipeline was ready for further configuration.

### Challenges Faced
I encountered challenges while configuring the `config.yml` to export artifacts. My unfamiliarity with Istanbul and Mocha, as well as my limited experience with Node.js, made this part of the setup somewhat challenging.

### Coverage and Artifacts
The code coverage and testing artifacts were useful as they provide assurance that the code functions as intended. In our case, the tests verified the calculator's functionality when given various calculations. If there are problems with the code, collaborators can examine the artifacts to identify and understand the problems.
Artifacts provide an important way of getting files and data out of a pipeline for further review.

## Processes
The configuration instructs the pipeline to execute these commands within the job:
- `npm install`: Installs necessary packages.
- `npm test`: Runs defined tests.
- `npm run test:coverage`: Runs the coverage testing framework.
- `store artifacts`: Preserves the files generated by the coverage report in CircleCI.

This was a relatively new process for me, as I hadn't previously worked with JavaScript or Node.js.