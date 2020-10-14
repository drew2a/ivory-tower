# Ivory Tower

🗼 collection of software development tips and principles

## Principles of Design

> “It is not enough for code to work.”
>
> ― Robert C. Martin

1. DRY – Don’t Repeat Yourself
1. KISS – Keep It Simple Stupid
1. YAGNI – You Aren’t Gonna Need It
1. SOLID:  
    * S – Single Responsibility Principle
    * O – Open-Closed Principle
    * L – Liskov Substitution Principle
    * I – Interface Segregation Principle
    * D – Dependency Inversion Principle

Ref: [SOLID in wikipedia](https://en.wikipedia.org/wiki/SOLID)

Ref: [Summary of 'Clean code' by Robert C. Martin](https://gist.github.com/wojteklu/73c6914cc446146b8b533c0988cf8d29)

## Code Style

If you don't have your own guide, it's a good idea to 
[adhere Google code style guides](https://google.github.io/styleguide/).

If you have your own guide, please keep it as general as possible.

### Commit message
> Describe your changes in imperative mood, e.g. "make xyzzy do frotz" instead of "[This patch] makes xyzzy do frotz" or "[I] changed xyzzy to do frotz", as if you are giving orders to the codebase to change its behavior.

As is described at [Documentation/SubmittingPatches in the Git repo](https://git.kernel.org/pub/scm/git/git.git/tree/Documentation/SubmittingPatches?id=HEAD#n133)

## TODO Comments

TODOs should include the string TODO in all caps, followed by the name, or other 
identifier of the person who can best provide context about the problem 
referenced by the TODO, in parentheses.

Example:

```
// TODO(drew2a) Add todo convention to CONTRIBUTING.md
```

## PR

* PR should improve overall code health of the system, even if the CL isn’t perfect
* Instead of seeking perfection, what a reviewer should seek is continuous improvement
* Review should be fast (1 day maximum)

Ref: [Google Engineering Practices Documentation](https://google.github.io/eng-practices)
Ref: [Speed of Code Reviews](https://google.github.io/eng-practices/review/reviewer/speed.html)

### Branching Model

* Use [OneFlow](https://www.endoflineblog.com/oneflow-a-git-branching-model-and-workflow) by default
* While merge, use `rebase + merge –no–ff` ([more information](https://www.endoflineblog.com/oneflow-a-git-branching-model-and-workflow#option-3-rebase-merge-no-ff))
* [Merge or rebase](https://www.atlassian.com/git/articles/git-team-workflows-merge-or-rebase)

### Creating PR

> Reviewers rarely complain about getting CLs that are too small.
>
Try to create only [small PR](https://google.github.io/eng-practices/review/developer/small-cls.html).
PR should makes a minimal change that addresses just one thing.

#### Process

1. Don't forget to actualize a documentation and dependencies
1. Increase the version numbers if it needed ([SemVer versioning](http://semver.org/))
1. You may merge the Pull Request in once you have the sign-off of one other developer
1. Don't forget to link the PR, and an issue [by using keywords](https://help.github.com/articles/closing-issues-using-keywords/)

#### PR Description

* First line: short summary of *what* is being done (an imperative sentence)
* Body: brief description of the problem and why this is the best approach

Ref: [Writing good CL descriptions](https://google.github.io/eng-practices/review/developer/cl-descriptions.html)

#### Handling comments

* Don’t Take it Personally
* Never respond in anger to code review comments
* Often it is better to clarify the code itself than explain in comments
* Think for Yourself

Ref: [How to handle reviewer comments](https://google.github.io/eng-practices/review/developer/handling-comments.html)

### PR Review 

Make sure that:
* The code is well-designed
* Code has appropriate unit tests
* Tests are well-designed
* Comments are clear and useful, and mostly explain why instead of what
* Code is appropriately documented
* The code conforms to style guides

Don't forget:

* To review every line of code you’ve been asked to review
* To look at the context
* To compliment developers on good things that they do

Ref: [What to look for in a code review](https://google.github.io/eng-practices/review/reviewer/looking-for.html)

Ref: [Navigating a CL in review](https://google.github.io/eng-practices/review/reviewer/navigate.html)

#### How to write comments
> Be sure that you are always making comments about the code and never making comments about the developer.

* Be kind.
* Explain your reasoning.
* Balance giving explicit directions with just pointing out problems and letting 
the developer decide.
* Encourage developers to simplify code

Ref: [How to write code review comments](https://google.github.io/eng-practices/review/reviewer/comments.html)

#### Resolving Conflicts

1. Try to come to consensus
1. Have a face-to-face meeting
1. Escalate

Ref: [The Standard of Code Review](https://google.github.io/eng-practices/review/reviewer/standard.html)