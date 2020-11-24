# Sandbox

Play with the Git or Rust over here :D

# Installation

Refer this [wiki](https://github.com/TPCSS-mbedTLS-Project-2020-22/sandbox/wiki/Tools-Required)

# Getting Started

1. Create a directory on your local machine `tpcss-project`
2. Navigate to `tpcss-project`

### Clone this repository

```
git clone https://github.com/TPCSS-mbedTLS-Project-2020-22/sandbox.git
```

## Exercises to try

### 1. Create a new branch

```
git branch <new-branch> <base-branch>
```

You can specify the name of the new branch and the base branch should be `main` For e.g.

```
git branch ashishk/test-branch main
```

After creating the new branch switch to that branch

```
git checkout ashishk/test-branch
```

### 2. Making changes

Open the `tpcss-project/sandbox` folder in VS Code. Try adding new files or editing the exisitng ones.

### 3. Publishing changes

Stage the changes

```
git add <File_name>
```

or to add all the changed files you can also do

```
git add .
```

Commit the changes by specifying the commit message

```
git commit -m "Put your message here"
```

Now, the code is only commited locally, to make it available at the remote repository, we will have to push it. If we push directly, it will throw error
since we have created the new branch locally, first we will need to create its remote upstream to which it will be pushed

```
git push --set-upstream origin <new-branch>
```

If you want to push to the exisitng branch you can directly do

```
git push
```

### 4. Create a pull request

- After you push the code successfully, you will see the yellow banner with button "Compare & Pull Request" on the repository page.
- In some edge cases, if you are unable to see the banner. Navigate to the `Pull Requests` tab.
- Click on "New Pull Request" button, add the base branch in which you want to merge your code (in most cases it will be the default branch "main" or "master").
- Select the newly created branch from the "compare" button dropdown and click on "Create Pull Request".
- Add the title and description to the pull request, so that the intention of the code change is pretty clear. You can also add screenshots.
- Add atleast 2 reviewers and labels and click on "Create pull request".
- If you are still working on some changes you can create a draft pull request.
- Don't directly merge the pull request, let the reviewers approve it, they might suggest changes, after everything is resolved, then it can be merged.
- The typical practice is to keep this option of merging disabled to avoid breaking of code in case someone pushes the code accidently. We will also follow the same practice for our `source` repository.
