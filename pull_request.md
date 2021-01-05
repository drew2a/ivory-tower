## PR

* PR should improve overall code health of the system, even if the CL isn’t perfect
* Instead of seeking perfection, what a reviewer should seek is continuous improvement
* Review should be fast (1 day maximum)

Ref: [Google Engineering Practices Documentation](https://google.github.io/eng-practices)
Ref: [Speed of Code Reviews](https://google.github.io/eng-practices/review/reviewer/speed.html)

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
* Use [conventional: comments](https://conventionalcomments.org/)


Ref: [How to write code review comments](https://google.github.io/eng-practices/review/reviewer/comments.html)

#### Resolving Conflicts

1. Try to come to consensus
1. Have a face-to-face meeting
1. Escalate

Ref: [The Standard of Code Review](https://google.github.io/eng-practices/review/reviewer/standard.html)