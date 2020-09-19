# Underwater Robotics Software Team Workflow

This repository exists to outline how our workflow operates.

# DOCUMENTATION

Documentation is useful, but the only thing worse than no documentation is incorrect doumentation! There is a concept/joke in programming called the "DRY" principle - Don't Repeat Yourself. If something is not outlined in the code, put it in the comments. That is, why dsomething was chosen over another option, other possible options, and some basic information about the purpose of functions and files. Avoid repeating what the code says in the comments, since they can quickly become outdated and do so without warning.

That said, code should also be reasonably legible; if the function which runs you main algorithm is named `a()`, maybe it's time change it.

Just remember that others will likely need to go through your work one day (or you may need to one day!), so it's best to keep it understandable.

# NAMING

Please check with a reviewer beore deciding on new repository names!

## Cases

### ROS

ROS is very inconsistent with this. We'll use all lowercase letters, numbers if necesary, and underscores for file names. (`file_name` is good, NOT `filename` OR `file-name`).

### GitHub

For GitHub things, like repository names and labels, use all lowercase and dashes. (`file-name` is good, NOT `filename` OR `file_name`).

# USING GITHUB

In Git and GitHub, each repository should be for one software package only. It can contain submodules, but other than that, it should be kept seperate from other pieces of code.

## Issues

Issues are very useful for tracking both TODOs and bugs. They can even be used for questions and the like. You cna refer to an issue almost anywhere on GitHub, and it will be linked automatically. That is, type `#1` into a comment, Markdown (\*.md) file, commit, pull request, or other issue, and it will link issue #1 to the GitHub location.

Not only that, but if you make a commit that solves an issue, typing `closes #1` will automatically close the issue. (The same goes for pull requests.)

Using `close` and issue numbers will also help with the "DRY" principle!

## Projects

We don't use Trello much for project tracking, like the other teams. Our project tracking happens on a more granular level. In you repository, create a Project (GitHub `Projects` tab) using the "Automated kanban with reviews" template. Try to keep this updated, since it will help us track what's going on i the repository.

If you make a card in a project just an issue number, like '#1', the project can **automatically move things around** when issues are handled. This keeps progress tracked without much need for overhead!

See the example project in this repository.

## Branches

We'll be developing with branches. Specifically, when developing any new features or making an changes, create a branch for it named `dev-[short-description]`. If you're doing a bugfix from `master` or `stable` branches, call them `hotfix-[desc]`. 

**Please do not commit directly to the `master` branch!**

When naming branches and any files, use lowercase letters and dashes (Ex. this-is-a-branch).

## Versions

If we want to create releases of certain code, which we will do for the more reusable code, we'll use GitHub Releases. These are also called Tags. We will be (loosely) following the standard called **semantic versioning**. You can read more [here](https://semver.org/), but here's all you need to know:

> Given a version number MAJOR.MINOR.PATCH, increment the:
> - MAJOR version when you make incompatible API changes,
> - MINOR version when you add functionality in a backwards compatible manner, and
> - PATCH version when you make backwards compatible bug fixes.

Our [arduino-port](https://github.com/CuUwrRobotics/arduino-port/releases) repository, for example has some releases and tags.

---

## Some GitHub Tips

- You can refrence issues and pull requests from anywhere in the repository using a #. For example: #1.
- Everything is written in a language called `Markdown`. It's a readable markup language that makes stuff look nicer when rendered by GitHub. You don't need to render it to easily read it though, unlike HTML for example. It might be good to brush up on what Markdown can do! Most version control servers use it, and MS Teams will even interpret it to some extent.
