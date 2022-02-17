# Git-Tutorial

## **A Brief Overview**
#### Git is essesntially a timeline management utility for projects.

<details open>
<summary>Important Terminology</summary>
<h4>Repositories</h4>
In Git, Repositories are a sort of data structure which store files and directories along with metadata about the changes that those files have undergone. Repositories track all changes made to files in your project, building a history over time. 
<h4>Branches</h4>
In Git, branching is when you diverge from the main branch of a repository. When you start working on a repository to add a new feature or fix a bug, you essentially make a new branch.

![Git Branch](git-branch.png)

 <h4>Add</h4>
 Git add takes a modified file in your working directory and places the modified version in a staging area.
<h4>Commit</h4>
Git commit takes everything from the staging area and makes a permanent snapshot of the current state of your repository that is associated with a unique identifier.

![Git Add and Commit](git-add-commit.png)


<h4>Stashes</h4>
When you want to switch branches but your work is not complete in the current branch you are in, you might not want to commit half done work. Stashing on git allows you to save your work and switch branches without commiting the current branch. To return to the stashed branched, the command git stash pop is used.
<h4>Merging</h4>
Merging in Git is when you combine a working branch back into your main branch. The changes you made in your working branch are implemented into the main branch when you merge if there are no conflicting code.

![Git Merge](git-merge.png)
</details>


---

## **Creating a Git Project**

### Step 1:
### Initialize a new Repository
The first step is to open up terminal and type in the following command:

`git init TestRepo`

Once you have done this, your terminal will say:

`Initialized empty Git repository in /Your Directory/TestRepo/.git/`

Right now your Repository is empty. If you type `git log` it will say `fatal: your current branch 'main' does not have any commits yet`. We will now add a text file to our repository.

Create a new file called `test-file.txt` in the TestRepo folder. From the terminal, this can be done with the command `touch test-file.txt`
