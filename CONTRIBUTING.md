# Contribution Guidelines

The golden rules of developing on this repo are:

1. **NEVER commit directly to the master branch!** The master branch is sacred and should
   mirror exactly that which is in production.
2. **Branch everything!** Every feature, bug or change should be developed in its own
   separate branch.
3. Commit little and often.
4. Rebase from master into your branch (`git rebase master`) **before** pushing.


## Development & Git Workflow

At Quesbook we abide by the "[Github Flow](https://guides.github.com/introduction/flow/)" branching
model as detailed [here]. Please take time to read that post and digest it all, as we try to stick
as close as we can to it.

In summary:

- Anything in the master branch is deployable.
- Commit little and often into you local branch and regularly push your work to the
  same named branch on the server.
- When you need feedback or help, or you think the branch is ready  for merging, open
  a [pull request].
- Make sure the Jankins build is passing and if not investigate and fix the issues.
- After someone else has reviewed and signed off on the feature, you can merge it into master.
- Once it is merged and pushed to `master`, you can and should deploy immediately.


## Branching

Branch names must be structured as follows:
```
 <issue number>_<short name or description>
```
Only alphanumeric characters are allowed. Use underscores (`_`) instead of spaces or
hyphens.


## Rebasing & Squashing Commits

Rebasing is good! Squashing commits is good!

**But...**

Rebasing is only allowed at the right time:

 1. Rebase local commits that have not yet been pushed to the remote. Rebasing changes your history, so if you rebase commits that you have already pushed, this will affect other users of that branch, and will really screw things up.
 2. Squash your commits by rebasing *immediately* before merging a finished branch into master. This is good, because it will help encourage a useful history, by squasing useless, throwaway commits made during development. (which we all do.)


## Issues

Use Github Issues to manage issues for this repo.

- Issues labelled with [`urgent`] and [`showstopper`] should be tackled first as a priority.
- Assign yourself to an issue when you start work on it. That way, we know that an issue is taken.
- Use labels wherever possible, and ensure that the issue is assigned correctly.
- Issues in the same repository can be referenced with `#number`.
- If an issue relies on or relates to an issue or PR in another repo, then make sure you mention
  that in the issue body. For example, use `quesbook/other_repo#1` to reference issue number 1 in
  the `quesbook/other_repo` repo.


## Pull Requests

Creating pull requests (PR) should be done when your branch is complete, or when you simply
want to solicit feedback on your code.

- If a PR is not complete, please prepend its title with `[WIP]` to indicate that this is
  a work in progress. Once the PR is complete, remove the `[WIP]` prefix.
- If an issue already exists, you should [reference the issue to your PR].
- If an issue does not exist, you should create it, making sure you reference the PR as above.
- Please do NOT add labels to PR's. This confuses QA. Only issues should use labels please.

> Any comments related directly to the code should be left on the PR. All other comments should be
> left in the issue.


### Coding Style

#### Ruby on Rails Principles And Coding Styles

The Rails philosophy includes two major guiding principles:

> Don't Repeat Yourself: DRY is a principle of software development which states that "Every piece
of knowledge must have a single, unambiguous, authoritative representation within a system." By not
writing the same information over and over again, our code is more maintainable, more extensible,
and less buggy.

> Convention Over Configuration: Rails has opinions about the best way to do many things in a web
application, and defaults to this set of conventions, rather than require that you specify every
minutiae through endless configuration files.

Please refer to this passage:
[The Design Principles of Ruby on Rails](http://www.nascenia.com/ruby-on-rails-development-principles/).

As for Coding Style, please refer to this page:
[Rails Style Guide](https://github.com/bbatsov/rails-style-guide).
And there's also a Chinese Version（中文版):
[Rails 4 编码风格实践](https://github.com/JuanitoFatas/rails-style-guide/blob/master/README-zhCN.md).

#### C++ Coding Styles by Google

As for C++ development, basically we are using mainly C++ for the data structures and algorithms for
machine learning. Though we might use Python or R for specific algorithms, but the database I/O,
fundemental architectures are still using C++.

[Google C++ Coding Style](https://google.github.io/styleguide/cppguide.html)

For both Ruby and C++, we use ONLY spaces, and ONLY 2 spaces for indention.

### Collaboration And Team-Working

We are using Flowdock to communicate with each other, with quip.com as our online document
collarboration platform.

#### Code Review

We encourage every engineer to review others' code, and ask if you have any problem with either
algorithms problems, logical problems and so on. If all the codes in the commit has been approved by
an engineer, he/she needs to comment in the commit "LGTM", which means "Look Good To Me", or a
thumbs up emoji.
