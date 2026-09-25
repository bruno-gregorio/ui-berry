# Claiming a Task

Documentation on how to claim a task.

1. The process starts at `https://linkedin.com/ai-trainer/tasks`. Authentication is necessary to operate this page if it's not already authenticated on LinkedIn, stop and ask the user to authenticate first.
2. Once on the the page, we have to select the right project. On the left part of the page there are three dropdowns in a row. The first must be set to "UI Berry" (this is the one with the project). The second dropdown contains the batch, usually we select the last one on the list, but be careful, at the end of some batches theres a tiny icon with two vertical bars, this informs us that batch is paused. We should never select a paused batch. If there are no batches that aren't paused, stop and inform the user. The last dropdown contains checkboxes with task status, and none o them should be selected when claiming a new task.
3. Once we have selected the right project and batch. On the right side of the screen there's a button called "Claim task" (this button is usually disabled if we didn't select properly). Click it to claim a task. By clicking it, two things can happen:
   - a new task will appear on the list with the "Not started" status. IMPORTANT: NEVER claim a new task while we still have a task "Not started" or "In progress" in the same project.
   - A toast message will appear telling us that there are no tasks available or some other error. If this happens, try another unpaused batch, if there are no more unpaused batches, stop and inform the user.
4. By clicking on the task with the "Not started" status we navigate to the task page. There we'll have a section "Attempt URL" and on it we'll have a link for the Feather platform. Click it and Feather will open on a new tab.
5. Once the task loads on Feather we have three scenarios:
   - The user isn't yet authenticated on Feather, in this case, pause and ask the user for authentication.
   - The Feather page shows a "Task not found" error. In this case, we close the tab, go back to the task page, click on the "Skip" button (top right). A modal will appear, there we type the reason "Task not found" and confirm the skipping of the task. We'll then be sent to the task list where we'll go back to step 2.
   - Feather loads a valid task, in this case look for the drop down on the top right of the screen, the task should be marked as "unclaimed" there (if it's not repeat the scenario above with changing only the skip reason to "The task is not unclaimed"). If the task is unclaimed, change it on the drop down to "In progress".
6. Whe you change the task on Feather to "In progress" the URL of the Feather page will change. Copy the new URL and go back to the task page on LinkedIn.
7. Once there look for the button "Start annotation" and click it.
8. On the section to the right side of "Attempt URL" (the one with the label "After claiming the task, copy the URL link from the browser.") the text box is no longer blocked, paste the Feather URL (the one copied on step 6) there.
9. Click on the "Save" button.
10. The task is now claimed, go back to Feather.

> Important note: this is a critical part of the workflow, if you find any unexpected circumstance outside of what's documented here, stop and inform the user.
