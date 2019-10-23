---
title: Code Review
section: guides
layout: page
---

Code Review
============
Code reviews are done for the following reasons:

* To ensure a consistent style of code
* To check for any pieces of code that may cause a knock on to other areas of the code base
* To identify a potentially more efficient way of making the acceptance criteria pass
* To help each other improve

Code reviews are not for:

* Testing the acceptance criteria
* Fixing bugs
* Making the coder feel uncomfortable

When You Want Your Code To Be Reviewed
======================================
1. Move your task to the "Code Review" column in Asana, but keep it assigned to yourself
2. Open a Pull Request on Github and assign it to the code reviewer
3. Message the code reviewer directly on Slack

Who Can Do Code Reviews?
========================
* Anyone! We encourage everyone to review each other's code. If you are not confident, request the support of someone more senior to talk you through it but don't pass it to them to do.

When Your Code is Being Reviewed
================================
* Welcome comments from the reviewer as a positive
* Do not assume that what the reviewer is saying is always right. Code is a very opinionated thing and you may have done something in a certain way for a reason

When You Are Reviewing Code
===========================
* Assume that the acceptance criteria passes
* Read the acceptance criteria
* Check the code against the [Cleversteam Rails Coding Standards](https://cleversteam.github.io/guides/ruby_rails_style_guide.html)
* Identify any possible areas for efficiency improvements
* Suggest changes as a question - "Would it be better to pluck rather than map?"
* Do not give direct instructions. Remember, the coder has written the code that way for a reason
