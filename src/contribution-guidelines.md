# Contributing Guidelines
Contributions are subject to the Code of Conduct.

## Reporting bugs
When reporting bugs, you should include information needed to understand, 
reproduce, and fix the issue.

You don't need technical understanding of the system(s) the bug is occuring in,
but you should at least provide the following information:
- Version information (i.e. version number, commit, etc.)
- Minimum amount of steps needed to reproduce the bug
- A description of the unintended behavior and the intended behavior

If you have the relevant skills and liberty to investigate the bug yourself,
it's very helpful to include any of the following:
- What could be causing the bug
- What can possibly be done to fix the bug
- A pull request that resolves the issue

## Submitting pull requests
Pull requests should be implement desired features, given adequate thought and 
design, and useful even if it is not accepted.

When you are updating your fork with upstream changes, please rebase 
(ex. `git pull --rebase` in the command line) to avoid creating merge commits.

If your pull request has a bug/typo that you fix in a later commit, try to merge
those commits into one so there is just one correct commit.

### Documentation
You should document your code so reviewers can understand how your code works
and where certain functionality exists within your code. Even if your code is
clear in what it does by itself, documentation lets people quickly orient
themselves in a codebase.

### Unit tests
Unit tests increase confidence in your code, improve long-term maintainability,
and are generally part of correct development processes. Unit tests make your
contribution more likely to be accepted.

### Formatting
Try to keep lines below 80 characters. This ensures readability on a wider
range of displays. 

### English language
Use proper English grammar, capitalization, and punctuation. 
If English is not your first language, try your best to get the important 
details across in your documentation. You are welcome to use translation
services to aid in your writing, but please prefer translation methods not 
based on Large Language Models (LLMs). Note that generating *code* with LLMs
is **not** allowed. 

### Use of Generative AI
xpans values quality contributions that are maintainable long-term. At the time 
of writing, other open-source projects have been weighed down by the cost of 
low-quality contributions evidently generated entirely or partially by Gen AI. 
It's apparent that some restrictive policies must be preemptively implemented 
to keep the xpans Project on the right path.

Using Gen AI / LLMs as a tool to assist in your workflow (i.e. searching docs,
translation, etc.) is perfectly fine. We are in no place to dictate how you
work.

Using Gen AI to *generate* code *and* submitting it crosses a line. This raises
copyright concerns and impacts how other people in the project work. As a
competent programmer and learner, you are expected to write code using your
own experience, knowledge of language idioms, understanding of larger
project scope, etc. when contributing to this project.

Please respect our time and your own. Suspected LLM-generated contributions
may be subject to rejection.
