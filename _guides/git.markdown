---
title: Git Protocol
section: guides
layout: page
---

Git Protocol
============

A guide for programming within version control.

Maintain a Repo
===============

* Avoid including files in source control that are specific to your
  development machine or process.
* Delete local and remote feature branches after merging.
* Perform work in a feature branch.
* Rebase frequently to incorporate upstream changes.
* Use a pull request for code reviews.

Write a Feature
===============

Create a local feature branch based off current working branch. Branch name should be as descriptive as possible and preferably include the name of the ticket.

    git checkout current_working_branch
    git pull
    git checkout -b <branch-name>

Rebase frequently to incorporate upstream changes.

    git fetch origin
    git rebase origin/master

Resolve conflicts. When feature is complete and tests pass, stage the changes.

    git add --all

When you've staged the changes, commit them.

    git status
    git commit --verbose

Write a [good commit message], prefixed with the name of the case. Example format:

    Fix User Login: Summary under 50 characters

    * More information about commit (under 72 characters).
    * More information about commit (under 72 characters).

If you've created more than one commit,
[use `git rebase` interactively](https://help.github.com/articles/about-git-rebase/)
to squash them into cohesive commits with good messages:

    git rebase -i origin/master

Share your branch.

    git push origin <branch-name>

Submit a [GitHub pull request].

Ask for a code review from someone else in your sprint team.

[good commit message]: http://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html
[GitHub pull request]: https://help.github.com/articles/using-pull-requests/

Review Code
===========

A team member other than the author reviews the pull request. They follow
[Code Review](/guides/code_review.html) guidelines to avoid
miscommunication.

They make comments and ask questions directly on lines of code in the GitHub
web interface.

For changes which they can make themselves, they check out the branch.

They make small changes right in the branch, test the feature on their machine,
run tests, commit, and push.

When satisfied, they merge.
