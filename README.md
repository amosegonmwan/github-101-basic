## GitHub-101 basics

1. **What is git?**  `Git` is a _Distributed Version control system_ used to:
    - _Tracks changes_ in code
    - Enables code _history management_
    - Supports _collaboration and multiple project versions_

    **Some Benefits of `Git`:**
    - **Code history management**: Easily revert to previous versions of the code.
    - **Collaboration**: Multiple developers can work on the same project without conflicts.
    - **Branching and merging**: Create branches for new features or experiments and merge them back seamlessly.
    - **Distributed system**: Each developer has a complete copy of the repository, enhancing redundancy and collaboration.
    - **Non-destructive Operations:**
        1. Actions in Git primarily add data to the database.
        2. Hard to perform irreversible actions; undoability is a core feature.
    - **Data Integrity:**
        1. Every piece of data is check-summed before storage.
        2. Impossible to change files or directories without detection.
    - **Local Operation Efficiency:**
        1. Most operations are local, minimizing network latency.
        2. Entire project history is stored locally, making operations nearly instantaneous.


2. **What is the purpose of git init?** The `git init` command is used to create a new Git repository. Essentially, the `git init` command is used perform the following:
    - **Create a New Git Repository:** Initializes a new Git repository in an existing directory by creating a `.git` subdirectory.
    - **Reinitialize an Existing Git Repository:** Reinitializes a repository if it already exists, useful if the `.git` directory was deleted or corrupted.
    - **Convert an Existing Project to a Git Repository:**_ Starts tracking an existing project with Git.


3. **How do we stage a file in git?** In order to stage a file in Git, the `git add` command is used. Staging a file means adding it to the staging area, also known as the index, which is a preparatory step before committing the changes to the repository. 
    - **Stage a Single File:** `git add filename`
    - **Stage Multiple Files:** `git add file1 file2 file3`
    - **Stage All Changes:** `git add .`
    - **Stage All Changes in a Specific Directory:** `git add path/to/directory`
    - **Stage Files Using a Pattern:** `git add *.txt`  stages all `.txt` files in the current directory.


4. **What does git log command do?** The `git log` command shows the commit history of a Git repository, detailing each commit's hash, author, date, and message.
    - `git log`: Shows commit history.
    - `git log -n <number>`: Limits commits shown.
    - `git log --oneline`: One-line format.
    - `git log --graph`: Graphical representation.
    - `git log -p`: Shows changes for each commit.
    - `git log <filename>`: File-specific history.
    - `git log --author="<author_name>"`: Author-specific commits.


5. **What is a git directory?** A Git directory is where Git stores all the information and history for a project. When a project directory is initialized as a Git repository, Git creates a `.git` directory in the root of the project.

    **Key Components of a Git Directory:**
    - `HEAD`: Points to the current commit.
    - `config`: Repository-specific settings.
    - `hooks/`: Scripts for automating tasks.
    - `objects/`: All the data (commits, files).
    - `refs/`: References to commits (branches, tags).


6. **What is git config?** `git config` is a command in Git that allows you to configure Git settings and preferences for your repository, user account, or system.

    **Levels of Configuration**
    - **System:** Applies to every user on the system and all their repositories.
        + `git config --system`
        + Stored in `/etc/gitconfig`.
    
    - **Global:**  Applies to all repositories for the current user.
        + `git config --system`
        + Stored in Stored in `~/.gitconfig` or `~/.config/git/config`
    
    - **Local:** Applies only to the specific repository.
        + `git config --local`
        + Stored in `.git/config` in the repository's directory.



7. **What are some options of the git config command?**
    - **Set User Name and Email:**
        + `git config --global user.name "Your Name"`
        + `git config --global user.email "your.email@example.com"`

    - **List All Configurations:** `git config --list`

    - **Get a Specific Configuration Value:** `git config user.name`

    - **Setting an Alias:** `git config --global alias.st status`
    
    - **Enable Colorized Output:** `git config --global color.ui auto`



### BASIC GIT WORKFLOW:
![Untitled](https://github.com/amosegonmwan/github-101-basic/assets/48167887/b051b032-c239-43a5-a34b-3e1335cecd5f)
