---
layout: post
title: Creating A Template (Self-Governing Code: Using Static Analysis and Automated Testing to Eliminate Word-of-Mouth Standards)
tags: [All Things Tech
image: /blog-prototype/public/images/Ben-Gibson-pic.png

bio: Ben Gibson has been at Edmunds for one year working as a Front End Engineer. He is currently working on a User Generated Content project that aims to improve user experience submitting reviews for consumers, auto repair services, and dealerships. In his spare time he enjoys recording music and traveling with his wife.
 
biopic: Ben-Gibson-pic.png

featured-summary:
    <p>Have you ever submitted code for review that is working perfectly and has great unit tests, but the response you get is, "Oh, we use tabs for indentation" or "We use ALL_CAPS_WITH_UNDERSCORES for static variable names. Please change, thx!"?</p>
    <p>Have you ever submitted code for review that is working perfectly and has great unit tests, but the response you get is, "Oh, we use tabs for indentation" or "We use ALL_CAPS_WITH_UNDERSCORES for static variable names. Please change, thx!"? Even though these fixes are easy to make, it can still frustrating that you didn't know about these standards beforehand.  Or maybe you tried to figure them out by searching the company wiki but you found conflicting results.  Either way, it can be painful that word of mouth was needed to figure out something so trivial.</p>

summary: Have you ever submitted code for review that is working perfectly and has great unit tests, but the response you get is, "Oh, we use tabs for indentation" or "We use ALL_CAPS_WITH_UNDERSCORES for static variable names. Please change, thx!"?
---

<h2 class="question-heading">The Problem</h2>

Have you ever submitted code for review that is working perfectly and has great unit tests, but the response you get is, "Oh, we use tabs for indentation" or "We use ALL_CAPS_WITH_UNDERSCORES for static variable names. Please change, thx!"?

Even though these fixes are easy to make, it can still frustrating that you didn't know about these standards beforehand.  Or maybe you tried to figure them out by searching the company wiki but you found conflicting results.  Either way, it can be painful that word of mouth was needed to figure out something so trivial.

And It can be even more painful when developers remember different versions of the standards.  When that happens, you get something like this: 

Finish changes. Assign for code review.  Implement changes based on first code review.  Submit for second code review.  Second reviewer tells you a different "right" way.  Interrupt everyone's day for a discussion between you, reviewer #1, reviewer #2, the most senior developer on your team.  Agree on something.  Update wikis.  Write an email to the team.  Cross your fingers and hope people read it.  Wash.  Rinse.  Repeat...

Now, that's enough to make you tear your hair out!

<h2 class="question-heading">The Solution: Never Fear. Automated Tests Are Here!</h2>

It doesn't have to be painful.  Many (or all) of the standards that we share by word of mouth or wiki documentation can be enforced with static analysis.

> "You want to name your file that way?..." BZZZ! Automated test failure!
    
> "You put a space in between your function name and the open paren?..." BZZZ! Automated test failure!

<h2 class="question-heading">If You Still Need Convincing</h2>  

Here are just a few of the benefits of using automated tests to enforce standards. 

* Faster and easier rampup for new developers.
* Less back and forth during code review.
* Consistency in code and code reviews.
* Reviewers can focus on important feedback.
* Quicker time to market (because of less back and forth).

<h2 class="question-heading">Examples at Edmunds</h2>

These are early examples from our JavaScript where everyone knew the rules/conventions, but they were often overlooked or were not easy to spot.

* Indenting:  Not 1 tab.  Not 2 spaces.  Not 8 spaces.  4 spaces. 
* Semicolons to end statements: ALWAYS.
* Global variables:  NOPE.  Not allowed.

Here are more early example where everyone knew the rules/conventions, but because we did not automated tests we always had inconstancies.  The typical excuse for these failures was laziness... I mean time-crunch.

* Monolithic classes
* “Paul Bunyan tall” functions
* Thirty-nine argument functions
* If and callback nesting and nesting and nesting and nesting... (Pyramid of Doom anyone?)

These are some of the scenarios that we now catch with automated tests.

<h2 class="question-heading">Going Further</h2>

You don't have to stop at trivial tests either.  Why not go farther and implement source lines of code validations (ie. "Your function/class can only X lines long")?  Or you can add cyclomatic complexity checks (ie. "You want me to read _that_ spaghetti code?").  We have recently added these tests to our front end code and it has made our lives and code much more beautiful.

Think of self-governing code as the logical extension of self-documenting code.  Use automated tests whenever possible, and make sure you have tests for any "standards" you put in place.






Here's a template table:

| Things I like to Eat | Reasons Why |
| ------ | ----------- |
| Frozen Peas | I love frozen peas because they are refreshing and cold.  What a great summer snack! |
| Fish Sticks are great too| I mean... they go well with frozen peas |
| Peanut Butter and Jelly Sandwiches and other types of sandwiches | Who doesn't like sandwiches|
| Frozen Peas | I mean come one.  Who doesn't like them?  Most people maybe... |

Here's an example of a numbered list.

1. Proactive - take ownership of your own work
2. An adult - gives you responsibility and holds you accountable
3. Communicative - requires you to actually talk to your teammates

Here's an example of a blockquote:

> This is a blockquote.  It's where you are quoting something and you want it to look like this.  So there it is.

Here's an example of inserting an image:

<img src="{{site.baseimagesurl}}/edmunds-technology.png" />

Here's how you can do headers

## Here's an H2
### Here's an H3
#### Here's an H4



