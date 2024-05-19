**# First-Repo
# Week 2 Assignment
## Quest 1: Explain Version control
Version control is a system that records changes to a file or set of files over time so that you can recall
specific versions later. It is a system that tracks and manages changes to software code, allowing developers
to work on projects more efficiently. It helps in managing the changes made to the source code in development
environments. Version control systems keep track of modifications to a database of source code, enabling
developers to compare current versions with earlier ones easily. Version control systems enable multiple
developers to work on the same codebase concurrently by managing changes efficiently and facilitating
collaboration through features like branching and merging.

## Quest 2: Explain the difference between Git and GitHub
Git is a distributed version control system (DVCS) that tracks changes in source code, coordinates work among
multiple developers, and helps manage code modifications efficiently. It is designed to offer speed, data
integrity, support for distributed non-linear workflows, and efficient tracking of changes in source code. On
the other hand, GitHub is a web-based hosting service that utilizes Git as its underlying version control
system. It offers a cloud-based platform for developers to store repositories, collaborate on projects, manage
tasks, and track issues related to their codebase.

## Quest 3: Three other alternatives to GitHub include:
(a)	GitLab
(b)	Bitbucket
(c)	Launchpad

## Quest 4: Explain the difference between Git fetch and Git pull
Git fetch is a command that downloads changes from a remote repository to the local repository but does not
integrate them into the working directory. It does not automatically merge any changes into your current
branch. It allows you to review the changes fetched before deciding to merge them manually; hence developers
typically use Git fetch when they want to see what changes exist in the remote repository without merging them
into their local branch immediately. Conversely, Git pull is a command that not only downloads new changes
from a remote repository but also integrates them into your current working directory. Developers use Git pull
when they want to update their local branch with the latest changes from a remote branch and immediately
incorporate those changes into their work. If there are conflicting changes between your local branch and the
remote branch, Git pull will attempt to merge them automatically. However, if there are conflicts that cannot
be resolved automatically, it will result in a merge conflict that needs manual intervention.

## Quest 5: Explain in simple terms, Git rebase and the command for it
Git rebase is a powerful command-line tool in Git for integrating changes from one branch into another. It
allows developers to apply the changes made in one branch onto another branch as if those changes were made
directly on the destination branch, and this usually results in a cleaner project history, as it eliminates
the need for merge commits and keeps the project history linear.
The command for Git rebase is:
$ git rebase <target_branch>

To use Git rebase, you first checkout the destination branch and then run Git rebase. For example, you would check out the experiment branch, and then rebase it onto the master branch as follows:
$ git checkout experiment
$ git rebase master

The command above tells Git to take the commits on the current branch (experiment) and place them on top of
the specified (master) branch.

## Quest 6: Explain in simple terms, Git cherry pick and the command for it
Git cherry-pick is a command in Git that allows developers to take a specific commit from one branch and apply
it to another branch. It’s like picking a commit from one place and placing it onto another branch, as if
you’re cherry-picking the commit you want.
The command for Git cherry-pick is:
$ git cherry-pick <commit_hash>

When you run this command, Git will take the changes made in the specified commit and apply them to your
current branch, allowing you to selectively choose and move commits between branches.