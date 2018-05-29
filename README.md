# Pull Requests / Code Reviews
## Motivations
+ It is an opportunity to spot defects early on, such as potential errors, bugs, dead code, typos. Basically anything you just worthy of being raised,
+ It helps enforce consistency and legibility across our codebase,
+ Naturally raise team's standards:
++ It is a way for everybody to learn (committers and reviewers),
++ Increase commits/code quality.
+ Besides ensuring quality, it is also a sharing tool:
++ Communicates on what has changed.
+ Pride
++ Quality begins with a sense of pride in what we do. The reviews you push are a way to share your knowledge, your commitment and further improve the codebase and our product.

## Submitting a Pull Request
When submitting a Pull Request, make sure the following has been thought through:
+ Context
++ Without writing an essay, try to include as much context as useful in the commit message/pull request description. When well done, it will help reviewers better understand what is your Pr about,
++ Consider discussing design decisions beforehand,
+ Test Plan
++ Provides a thorough Test Plan. By doing so, you will help reviewers process your review more timely. The easier it is to understand your changes, the more chance your PR has to be picked up first,
++ Think of the various scenarios that need to be covered,
++ Writing a Test Plan will also help you spot any edge cases you could have missed to support in your change.
+ Keep your diff under 200 lines (+ tests):
++ If you want your PR processed timely, try to keep it under 200 lines change (500 HUGE MAX, probably need a valid reason).,
++ Big PRs are more difficult to review,
++ Keep them single goaled,
++ Consider splitting up your review: platforms, goals, areas of code changed,
++ Again, this is in trying to make your PR quickly digestible.
+ Feel free to annotate your diff if you think that would be helpful
++ Some will say “if your code is well written, this shouldn’t be necessary”. The truth is, with 60+ engineers in Mobile, processing all PR in due time isn’t anything easy, even if the code is well-written. Annotating your code will help whoever picked your PR, might even make it #1 in the list thanks to its quality.
+ Auto-generated/Refactored code should be separate
++ Usually massive, requires more attention but doesn’t get it.
++ As much as possible, try to keep auto-generated/refactored code in a separate PR. Having it part of a single PR will only increase it’s complexity and the amount of time required to review it. Keeping it separate will help you expedite the review process of these kinds.
++ Should not contain any behaviour changes.
++ If covered by tests, it should be enough.
+ 3 reviewers max + team
++ We ALL met this case when we wanted our review to be done ASAP. And in the past, thought “let me add everybody to grab attention”. What usually happen, each of these names will stare at it for a few secs and think “probably someone will look at it or might even be looking at it already”.
+ Review scope and size


+ Complete, self-reviewed, self-tested code only
++ Make sure your changes are complete. This does not mean you can’t reach out individually to ask for advices before continuing but when assigning reviewers, your code should be done. 
++ Make sure it contains clear ACs.
++ Review your own code once you have a diff.
++ Test your changes.
++ Make sure tests pass.
++ Then assign reviewers.
+ Check the commit history is clean
+ Check the commit message is clear
++ Anyone in the company could be reading it at some point.
++ Your description should contains:
+++ Context of the changes, why was it necessary.
+++ Test Plan
+++ ...
+ It is not an exam
++ Remember that a PR/CR isn’t an exam. It is simple a tool to give others an opportunity to spot issues and provide suggestions on how to do better.

## Reviewing a Pull Request
+ Understand context and why
++ To perform good reviewing, you need to understand what this change is about. If there is nothing helping you understand that, you should reach out to the committers / politely reject the PR stating a bit of context would be appreciated.
++ Understand why this change was necessary and feel free to discuss it with the committer.
+ Be mindful, aware of online communication
++ Especially when disagreeing, by mindful of how you communicate that in the PR. Remember that neutral communication is often seen as negative when online.
++ Avoid using “stupid”, “crazy”, “NEVER DO that”.
+ Offer suggestions to improve
++ Don’t simply point and reject a PR. Try to offer help and suggestions to improve.
+ Aim to develop skills and product quality
+ Consider reaching out to submitter
++ It is always a good behaviour to determine what is the best channel to communicate feedback on a PR. If you are about the type down an essay, it might be worth reaching out to the committers to discuss the matter. 
+ No more than 300-500 lines per hour
++ Above that, the quality of your review decreases.
+ No more than 60 minutes at a time
++ Above that, please take a break, for your own sanity.
+ Try to be proactive
++ 60+ engineers, 1 goal, the same: ship a product of quality.
++ When you see something in review, consider taking a break in your current task to focus on pending reviews. One will say “context switching” reduce velocity and quality, but the cost of something sitting in review is greater.
++ Do not hold a review too long if it is making things better.

## References
+ https://github.com/palantir/gradle-baseline/blob/develop/docs/best-practices/code-reviews/readme.md
+ https://blog.github.com/2015-01-21-how-to-write-the-perfect-pull-request/
+ http://blog.cleancoder.com/uncle-bob/2015/11/18/TheProgrammersOath.html

	



