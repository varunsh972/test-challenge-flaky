# Solution
I found that in code we were creating a dummy response with settimeout so in cypress test cy.get('li') was not waiting for time out and it shows error.
To fix it i added a max timeout in cy.get() so that cy wait till max timeout as added in localstorage saving api. If cypress found li within timeout time it will sow "test" as success or else it will show error.
 

# The Flaky Test Challenge

As an engineer, you will be expected to ensure that all new features and fixes do not cause regressions or headaches for active users. Tests are an important tool for keeping our apps usable and bug-free. However, tests are only useful if they are reliable. This challenge will test your ability to understand and fix a flaky test of a React app.

## The Challenge

The test for this app sometimes passes and sometimes fails. You should be able to quickly figure out a change that will make the test 100% reliable.

You may modify any file or files *except* those in the `src/` directory.

## Instructions

_You must follow these steps for your solution to be accepted_

**Forking this repo is an immediate disqualification**

How to attempt this challenge:

1) Clone this challenge repo
2) Solve the challenge locally
3) Create a new repo in your GitHub account and note the git url
4) Set your new repo as the origin for your local solution: `git remote set-url origin ${your repo url}`
5) Push the solution to your repo
