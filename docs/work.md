# Working on a task

Once you successfully claimed a task and is now back on Feather, time to work on it. This workflow should run as a separate sub-agent.

This is a UI Berry task in which you must compare two websites across three different dimensions: aesthetics, functionality and overall, taking as the main source of truth the user prompt present on the page. This document is just a quick guide, the full documentation can be found at on the [PDF](./UI%20Berry.pdf).

On this page there are two button "Website A" and "Website B", those will take you to a partial view of each website. Once there you must look for a button with a tooltip more or less like this "Open preview in a new environment", it's located below the iframe of the preview, to the right side of the "Capture" button. This button will open the site on a new tab, all of your tests must be conducted there.

Before comparing, list what the prompt requires: content, behavior, data, and visual style. Keep extra features separate. Do not treat an extra as a requirement or assume a feature is missing until you check the full workflow.

Test the requested controls through their results, not just their first click. Check forms, navigation, counts, values, and visible defects. Confirm each claim in the live site, including problems on the website you prefer.

Make four problem lists: aesthetics and functionality for each website. Display them, then check every item against the live sites. See the [PDF](./UI%20Berry.pdf) for what each dimension covers.

Now that we have the four lists, we have to condense them in three prose fields:

- Aesthetics: compare visual quality and the requested style, separate from behavior and prompt coverage.
- Functionality: compare requested content and working behavior, wherever they appear in the workflow.
- Overall: weigh both dimensions independently. There is no automatic winner when they disagree.

Those prose fields must follow some very specific rules, please check the attached [PDF](./UI%20Berry.pdf) for the whole context. But here are some of the most notable ones:

- Do not use — or ; on the prose. There are also mentions of other special symbols you should avoid in the [PDF](./UI%20Berry.pdf) file. Usually, letters, numbers, colons, and periods are all that you can use.
- Always prefer objective descriptions of things in the original report instead of adjectives.
- When referring to the Websites, never shorten "Website A" to "A", same thing for "Website B".
- Some points might include specific time lengths, for example, "Website A does X in 25 seconds", when writing your report, try to use a more human way to describe those time lengths, as it's unlikely a human would've gotten the exact second.
- Sometimes, even though one of the options has a higher number of problems in a dimension, it is chosen as the better option because the other option has more severe problems; when this happens, you must explicit this weight-based choice on the prose.
- Always start each prose field with this pattern: "Website X is better because..."
- The overall field must whenever possible try to avoid just quoting the other two fields, this field should focus on why the disadvantages of a certain option make it inferior to the other, focus on explanations.
- All prose must be written in english.

Once you have all three prose fields, display them on the chat and look at the page and fill the three text fields with the right prose and tick the appropriate button above it. Once done, the work here is done, don't do anything else.

Extra notes:

- The review should reflect the experience of a hypothetical final user, avoid using problems from overly synthetic situations like: the UI breaks if we render it at height 650px.
- Unless asked on the prompt, only test the application in desktop mode.
- Be careful when judging a page by things not explicitly mentioned on the prompt. You might still do this as long as you think it's relevant for the end user (for example: bad contrast might not be on the prompt, but it's still a bad design choice). When composing the prose always give priority for problems you can trace back to the prompt.
- Do not use non-ASCII characters on the prose fields.
- Do not write in the first person on the prose fields.
- Each prose field should be self-contained, do not assume access to your internal context to verify, for example, test values.
- Before entering the prose, remove repeated or unverified claims and use any exact category names required by the task.
