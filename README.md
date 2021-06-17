# Epion Dev Ops Interview Project

Thanks for being interested in coming to work here at Epion Health.

In our technical interview, we'll work on this simplified version of our
mono-repo. We will use Slack to share your screen unless that wouldn't work for
you. Please make sure you have the desktop app installed beforehand.


## 1. Take home section

We'll work with our two main branches:

- `develop`, where developers merge in their work after code reviews
  and CI pipelines pass. Their work may not be tested by QA yet.
- `main`, which we freeze every week to test any remaining commits, where QA
  performs full regression testing, and then we deploy to production.
  (Meanwhile, devs may continue to add work to unfrozen `develop`).

Cutting a release (updating `main`) involves:

1. Merging `develop` and `main` together (typically happens on Tuesdays at
   midday).
2. Preparing a report: list all Jira cards linked in the commit descriptions,
   and show to interested parties (by Slack, Email, GitHub; whatever makes the
   most sense to you).
3. Pushing the updated `main` branch to our `staging` server.

**The goal is to automate our release cut.**

Please add your automation script to the project and send us a
`git format-patch` with your suggested solution.

(If you are interested in learning the thought process that led us to this git
workflow, you may read https://withatwist.dev/our-git-branching-model.html).


## 2. Technical discussion

After you send us a solution for the Take home section, we'll schedule a call so
you describe your solution, and we ask some questions, discuss potential
alternatives, the pros and cons of different approaches, and we may pair on a
change.

----

Please note that there’s no single correct answer. We are looking to understand
how you approach automation problems and what is important to you in a solution.
Take your time and show us your best work.

Most of all, don’t hesitate to ask any questions. We’re looking forward to
seeing your solution and talking with you about it.
