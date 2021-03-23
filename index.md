---

# Developer 101 Series

## Part 1: Getting Started with Git/GitHub

### Terminologies

### Repository

### Remote

### Local

### Staging area

### Commit

### Push

---

### Install Git

[Git for Windows](https://git-scm.com/download/win)

Depending on your system architecture (32-bit vs. 64-bit), you will be prompted to download the correct version of the installer.

[Git for MacOS](https://git-scm.com/download/mac)

Under Binary Installer click installer.

[Git for Linux](https://git-scm.com/download/linux)

- Run the commands listed for your operating system
- Git icon after installation and how the icon/Git Bash can be accessed… add a visual for this!
- have everyone install git and create a github account before the meeting (see videos/youtube tutorial to set up than create a document)


### Create a GitHub account
Go to [GitHub](https://github.com/join?ref_cta=Sign+up&ref_loc=header+logged+out&ref_page=%2F&source=header-home) and use your my.unt.edu email address (student developer benefits!)

---

### Create a git repository in your local machine

Method 1:
```
Desktop> mkdir git101
Desktop> cd git101
```

Syntax: git init

```
Desktop\git101> git init
Initialized empty Git repository in /Users/xxx/Desktop/myproject/.git/
```

Method 2:
```
Desktop> git init git101
Initialized empty Git repository in /Users/xxx/Desktop/myproject/.git/
```


### Add a new file to the local repository

```
create a new file named test.txt
Desktop\git101> echo "this is a test file" > test.txt
```

Syntax: git status

```
git status
```

Syntax: git add <relative_path_of_the_filename_to_be_added>

```
git add ./test.txt
```

Commit

Syntax: git commit -m "<brief_description of_your_commit>"

```
git commit -m "This is my first commit!"
```

### Create a repository on GitHub

Syntax: git remote add <an_alias_for_remote_repository> <complete_url_of_remote_repository>

```
git remote add origin https://github.com/<yourname>/test.git
```

Syntax: git branch -M main

```
git branch -M main
```

### Push changes to GitHub

Syntax: git push <remote_repo_alias> <remote_repo_branch_name>

```
git push origin main
```

---

In the next part, we will explore:

- Creating a branch
- Pushing code from local branch to remote branch
- Creating a pull request
- Merging a PR
- Getting changes from GitHub to local machine
