# UI Berry

This is a repo focused on a vendor neutral agent to help me automate some of my work on the UI Berry Project.

This project involves an automation of the chrome browser. Before anything, check if you can access an instance of Google Chrome. If not, stop and inform the user.

The basic loop of this workflow consists of three steps:

1. [Claim a task](./docs/claiming.md)
2. [Work on the task](./docs/work.md)
3. [Submit the task](./docs/submission.md)

The user will typically inform you how many times you should run this loop, but you must never run this more than 30 times on a single day.

> Be very conservative when it comes to errors in the first and the last steps, for any unexpected outcome you should stop immediately and inform the user. Do not attempt to "fix" the situation by yourself.
