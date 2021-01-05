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

## Branching Model

* Use [OneFlow](https://www.endoflineblog.com/oneflow-a-git-branching-model-and-workflow) by default
* While merge, use `rebase + merge –no–ff` ([more information](https://www.endoflineblog.com/oneflow-a-git-branching-model-and-workflow#option-3-rebase-merge-no-ff))
* [Merge or rebase](https://www.atlassian.com/git/articles/git-team-workflows-merge-or-rebase)


## Branch naming convention

* Use slash to separate groups of branches
* Use a ticket key in a branch name

Example

```
feature/123
feature/657-add-travis-ci

fix/741

release/1.2
```

## PR

* PR should improve overall code health of the system, even if the CL isn’t perfect
* Instead of seeking perfection, what a reviewer should seek is continuous improvement
* Review should be fast (1 day maximum)

More information: [Pull Request](pull_request.md)