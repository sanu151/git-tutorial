# Git and GitHub

**Git:** Let's start with Git. Imagine it as a super-powered diary for our code. It keeps track of every change we make, allowing us to go back in time if something goes wrong. It's like having a time machine for our projects!

**GitHub:** Now, GitHub is like a digital library where we can store and share our Git-tracked projects. It's a platform for developers to collaborate, learn from each other, and showcase their work. Think of it as a social network for coders.

**My Experience:** I first encountered Git and GitHub when I started contributing to an open-source project. At first, it felt a bit overwhelming, but once I got the hang of it, I realized how valuable it was. It helped me:

* **Version Control:** Keep track of my changes and easily revert to previous versions if needed.
* **Collaboration:** Work with other developers on the same project without stepping on each other's toes.
* **Learning:** Explore other people's code and learn new techniques and best practices.

**Why We Should Use Them:** Whether we're a solo developer or part of a team, Git and GitHub can be incredibly beneficial. They help us:

* **Organize Our Work:** Keep our projects well-structured and easy to manage.
* **Collaborate Effectively:** Work with others seamlessly and efficiently.
* **Learn and Grow:** Explore open-source projects and contribute to the community.

### Visualization of Git : **[Visualizing Git](https://git-school.github.io/visualizing-git/)**

## Git vs. GitHub: A Comparison

| Feature | Git | GitHub |
|---|---|---|
| **Purpose** | A version control system for tracking changes in files. | A cloud-based hosting service for Git repositories. |
| **Functionality** | Creates, tracks, and manages versions of files. | Provides a platform to share, collaborate, and manage Git repositories. |
| **Nature** | Primarily a command-line tool. | A web-based platform. |
| **Storage** | Stores repositories locally on your computer. | Stores repositories remotely on cloud servers. |
| **Collaboration** | Supports collaboration through features like branches and merging. | Provides features like pull requests, issues, and forks for easier collaboration. |
| **Accessibility** | Requires installation on your computer. | Accessible through a web browser. |
| **Examples of Use** | Tracking changes in code, creating backups, and managing project history. | Sharing code with others, collaborating on open-source projects, and hosting private repositories. |

## Most Used Git and GitHub Commands

| Command | Definition | Example |
|---|---|---|
| **Git Commands** | | |
| `git init` | Initializes a new Git repository in the current directory. | `git init` |
| `git add <file>` | Adds a file to the staging area. | `git add README.md` |
| `git rm --cached <file>` | Unstage a file from staging area. | `git rm --cached README.md` |
| `git commit -m "message"` | Creates a new commit with the specified message. | `git commit -m "Initial commit"` |
| `git status` | Shows the current status of the repository. | `git status` |
| `git diff` | Shows the differences between the working directory and the staged or last committed version. | `git diff` |
| `git log` | Shows the commit history. | `git log` |
| `git show <commit_id>` | display detailed information about a specific commit. | `git show 913c106` |
| `git checkout <branch>` | Switches to the specified branch. | `git checkout feature_branch` |
| `git branch <branch_name>` | Creates a new branch. | `git branch new_feature` |
| `git merge <branch>` | Merges the specified branch into the current branch. | `git merge feature_branch` |
| `git pull` | Fetches changes from a remote repository and merges them into the current branch. | `git pull origin main` |
| `git push` | Pushes changes to a remote repository. | `git push origin main` |
| **GitHub Commands** | | |
| `git clone <url>` | Clones a remote repository to your local machine. | `git clone https://github.com/user/repo.git` |
| `git remote add origin <url>` | Adds a remote repository to your local repository. | `git remote add origin https://github.com/user/repo.git` |
| `git pull origin <branch>` | Fetches changes from a remote branch and merges them into your local branch. | `git pull origin main` |
| `git push origin <branch>` | Pushes changes from your local branch to a remote branch. | `git push origin main` |
| `git pull request` | Creates a pull request on GitHub to propose changes to a repository. | `git pull request` |
| `git issue` | Creates a new issue on GitHub. | `git issue` |



## Setting Up Git: A Quick Guide

**1. Install Git:**
   - Download the installer from [https://git-scm.com/](https://git-scm.com/) for your operating system (Windows, macOS, or Linux) and follow the instructions.

**2. Verify Installation:**
   - Open your terminal or command prompt and type `git --version`. If it shows a version number, Git is installed.

**3. Configure Your Name and Email:**
   - These will be used to identify you in your commits.
   ```bash
   git config --global user.name "Your Name"
   git config --global user.email "your.email@example.com"
   ```
The `git config --list` command is used to display all of your Git configuration settings. It will show you the current values for various Git options, such as your name, email, editor, and other preferences. 

Here's an example of what the output might look like:

```
user.name=Your Name
user.email=your.email@example.com
core.editor=vim
color.ui=auto
...
```

In this example, the user's name is "Your Name", their email is "your.email@example.com", their preferred editor is "vim", and color output is enabled.

You can use this command to verify that your configuration settings are correct or to see the current values for specific options.

I'd be glad to assist you with creating a Git folder and adding a Git file. Here's a comprehensive guide that incorporates the best aspects of previous responses and addresses potential issues:

**1. Create a New Directory:**

- Open your terminal or command prompt and navigate to the desired location where you want to create the Git folder.
- Use the `mkdir` command to create a new directory named "git_folder":

   ```bash
   mkdir git_folder
   ```

**2. Change to the Git Folder:**

- Access the newly created directory using the `cd` command:

   ```bash
   cd git_folder
   ```

**3. Initialize Git Repository:**

- Convert the current directory into a Git repository using the `git init` command:

   ```bash
   git init
   ```

   This will create a hidden `.git` directory within the `git_folder`, which stores all the necessary Git metadata.

**4. Create a New File:**

- Use your preferred text editor to create a new file within the `git_folder`. For example, to create a file named `README.md`:

   ```bash
   touch README.md
   ```

   Open the `README.md` file in your text editor and add some content.

**5. Add the File to Git Staging Area:**

- Stage the newly created file for inclusion in the next commit using the `git add` command:

   ```bash
   git add README.md
   ```

   This adds the `README.md` file to the Git staging area, indicating that it's ready to be committed.

**6. Commit the Changes:**

- Create a new commit to capture the changes made to the `README.md` file using the `git commit` command. Provide a descriptive message for the commit:

   ```bash
   git commit -m "Initial commit of README.md"
   ```

   Replace `"Initial commit of README.md"` with a more meaningful message that describes the changes you've made.

**Additional Notes:**

- You can repeat steps 4-6 to add more files to the Git repository and create subsequent commits.
- To view the status of your Git repository, including any staged or unstaged changes, use the `git status` command.
- To undo the last commit, use the `git revert HEAD` command.
- To undo the last `git add` operation, use the `git reset HEAD <filename>` command.
- To push your changes to a remote Git repository (if you have one configured), use the `git push` command.

By following these steps, you'll have successfully created a Git folder, initialized a Git repository, and added a new file to it. This provides a solid foundation for using Git to track and manage your project's changes.

## Git Staging and Unstaging

**Staging** and **unstaging** in Git refer to the process of preparing files for inclusion or exclusion from the next commit. It provides a way to selectively choose which changes you want to include in a commit and which ones you want to postpone.

### Staging

* **Purpose:** Adds files to the staging area, indicating that they're ready to be committed.
* **Command:** `git add <filename>`
  - Replace `<filename>` with the name of the file you want to stage.
  - You can also stage multiple files at once: `git add <file1> <file2> ...`
  - To stage all changes in the current directory: `git add .`

### Unstaging

* **Purpose:** Removes files from the staging area, preventing them from being included in the next commit.
* **Command:** `git reset HEAD <filename>`
  - Replace `<filename>` with the name of the file you want to unstage.
  - To unstage all changes: `git reset HEAD --hard`

**Example:**

1. **Create a new file:**
   ```bash
   touch new_file.txt
   ```
2. **Stage the file:**
   ```bash
   git add new_file.txt
   ```
3. **Make changes to the file:**
   - Edit `new_file.txt` and add some content.
4. **Check the status:**
   ```bash
   git status
   ```
   You'll see that the file is staged for commit.
5. **Unstage the file:**
   ```bash
   git reset HEAD new_file.txt
   ```
6. **Check the status again:**
   ```bash
   git status
   ```
   Now, the file will be listed as modified but not staged.

**Key Points:**

* **Staging area:** A temporary storage area where files are prepared for inclusion in the next commit.
* **Commit:** A snapshot of the repository at a particular point in time.
* **Staging and unstaging:** Allow you to control which changes are included in each commit.
* **`git add` and `git reset`:** Commands used for staging and unstaging files.

By understanding staging and unstaging, you can effectively manage your Git workflow and create clean, focused commits.

**`git status`**

This command provides a snapshot of the current state of your Git repository, showing you which files have been modified, staged, or unstaged.

**Example:**

```bash
git status
```

**Output:**

```
On branch main

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        new_file.txt

nothing to commit, working tree clean
```

This output indicates that there is an untracked file named `new_file.txt` in the working directory. It also shows that there are no staged changes or uncommitted changes.

**`git diff`**

This command compares the current state of your working directory to the staged changes or to the last committed version. It shows you the specific differences between the files.

**Example:**

1. **Compare working directory to staged changes:**
   ```bash
   git diff
   ```
2. **Compare staged changes to last commit:**
   ```bash
   git diff --staged
   ```
3. **Compare working directory to last commit:**
   ```bash
   git diff HEAD
   ```

**Output:**

```
diff --git a/new_file.txt b/new_file.txt
index 8864750..e69de29 100644
--- a/new_file.txt
+++ b/new_file.txt
@@ -0,0 +1 +2 @@
+This is a new line.
```

This output shows the specific differences between the current version of `new_file.txt` and the last committed version. In this case, a new line has been added to the file.

**Additional Notes:**

- You can use the `--cached` option instead of `--staged` to get the same output.
- The `git diff` command can also be used with specific file paths to compare differences between specific files.
- To see a more detailed diff output, you can use the `--patch` option.

By effectively using `git status` and `git diff`, you can gain a better understanding of the changes in your Git repository and make informed decisions about your commits.

**Git Folder Staging**

* **Purpose:** Adds files within a specific folder to the staging area for inclusion in the next commit.
* **Command:** `git add <folder_name>`
  - Replace `<folder_name>` with the name of the folder you want to stage.
  - This command will stage all files and subfolders within the specified folder.

**Example:**

1. **Create a new folder:**
   ```bash
   mkdir new_folder
   ```
2. **Create files within the folder:**
   ```bash
   touch new_folder/file1.txt
   touch new_folder/file2.txt
   ```
3. **Stage the entire folder:**
   ```bash
   git add new_folder
   ```

**Git Diff for Folders**

* **Purpose:** Compares the changes in a specific folder to the staged changes or the last committed version.
* **Command:** `git diff <folder_name>`
  - Replace `<folder_name>` with the name of the folder you want to compare.

**Example:**

1. **Compare changes in the folder to staged changes:**
   ```bash
   git diff new_folder
   ```
2. **Compare changes in the folder to the last commit:**
   ```bash
   git diff HEAD new_folder
   ```

**Additional Notes:**

- You can use the `--cached` option instead of `--staged` to get the same output.
- The `git diff` command can be used with specific file paths within the folder to compare differences between specific files.
- To see a more detailed diff output, you can use the `--patch` option.
- If you want to stage only specific files within a folder, you can use the `git add <file_path>` command.

By effectively using these commands, you can efficiently manage changes within Git folders and gain a better understanding of the differences between the current state and previous versions.

## Git Commit and Reset Commit

### Git Commit
* **Purpose:** Creates a snapshot of the current state of your repository, saving your changes.
* **Command:** `git commit -m "<message>"`
  - Replace `<message>` with a descriptive message about the changes you made.
  - The message should be concise and informative.

**Example:**
```bash
git commit -m "Added new feature to calculate area of a circle"
```

### Git Reset
* **Purpose:** Reverts the repository to a previous state.
* **Command:** `git reset <commit_hash>`
  - Replace `<commit_hash>` with the SHA-1 hash of the commit you want to reset to.

**Types of Resets:**
* **Soft reset:** Unstages changes but keeps them in your working directory.
* **Mixed reset:** Unstages changes and discards them from your working directory.
* **Hard reset:** Unstages changes, discards them from your working directory, and removes them from the commit history.

**Example:**
```bash
# Soft reset to the previous commit:
git reset HEAD~1

# Mixed reset to the previous commit:
git reset --mixed HEAD~1

# Hard reset to the previous commit:
git reset --hard HEAD~1
```

**Additional Notes:**
* Use `git log` to view the commit history and get the SHA-1 hashes.
* Be cautious with hard resets, as they can permanently delete changes.
* Consider using `git revert` to create a new commit that undoes the changes of a previous commit instead of resetting.

**Example:**
```bash
# Revert the last commit:
git revert HEAD
```

By understanding `git commit` and `git reset`, you can effectively manage your Git repository and undo changes if necessary.

**Git Log**

The `git log` command is used to view the commit history of a Git repository. It provides information about each commit, including its author, date, and a short message describing the changes.

**Basic Usage:**

```bash
git log
```

This will display a list of commits, starting from the most recent to the oldest.

```bash
$ git log
commit 425a91ec7759aba8844fe1b47646795845f30665 (HEAD -> master)
Author: Supriyo Das <das.supriyo07@gmail.com>
Date:   Tue Sep 24 21:33:23 2024 +0530

    First Commit

```

**Options:**

You can customize the output of `git log` using various options:

* **`--oneline`:** Displays each commit on a single line.
* **`--pretty=format`:** Specifies the format of the output. For example, `--pretty=format:"%h %s"` will display the commit hash and subject.
* **`--author=<author_name>`:** Filters commits by author.
* **`--after=<date>`:** Shows commits after a specific date.
* **`--before=<date>`:** Shows commits before a specific date.
* **`--grep=<pattern>`:** Filters commits based on their commit message.
* **`--reverse`:** Reverses the order of commits (oldest to newest).

**Examples:**

* **Show the commit history in a one-line format:**
  ```bash
  git log --oneline
  ```
* **Show the commit hash, subject, and author:**
  ```bash
  git log --pretty=format:"%h %s (%an)"
  ```
* **Show commits made by a specific author:**
  ```bash
  git log --author="John Doe"
  ```
* **Show commits made after a specific date:**
  ```bash
  git log --after="2023-01-01"
  ```
* **Show commits with a specific keyword in the commit message:**
  ```bash
  git log --grep="feature"
  ```

By using these options, you can tailor the output of `git log` to your specific needs and easily find the commits you're looking for.

## Git Checkout, HEAD, and Related Commands

 ### git checkout

**Purpose:**

* Switches the current working directory to a specific commit in the repository's history.
* Allows you to inspect files, compare changes, or create a new branch from that commit.

**Syntax:**

```bash
git checkout <commit-id>
```

Replace `<commit-id>` with the SHA-1 hash of the commit you want to check out.

**Example:**

```bash
git checkout 9876543210abcdef1234567890
```

This command will switch your working directory to the commit with the ID `9876543210abcdef1234567890`, allowing you to explore the files and changes at that point in time.

**Key Points:**

* **Detached HEAD:** When you check out a specific commit, you enter a detached HEAD state. This means you're not on a branch, but rather a specific point in the history.
* **Creating a New Branch:** If you want to create a new branch from a specific commit, you can use the `-b` option with `git checkout`:
  ```bash
  git checkout -b <new-branch-name> <commit-id>
  ```
* **Returning to a Branch:** To return to a branch after checking out a commit, use:
  ```bash
  git checkout <branch-name>
  ```

**Additional Notes:**

* Be cautious when working in a detached HEAD state, as you might lose your changes if you don't create a new branch.
* Use `git log` to find the commit IDs you want to check out.

By understanding `git checkout` for commits, you can effectively explore your repository's history and create new branches from specific points in time.


### `git checkout HEAD`
* **Purpose:** Restores the working directory to the state of the last committed version.
* **Explanation:** This command essentially undoes any uncommitted changes you've made, bringing your working directory back in line with the latest commit.

### `git checkout <commit ID>`
* **Purpose:** Switches to a specific commit in the repository's history.
* **Explanation:** This command allows you to explore different points in time in your project's development. You can inspect files, compare changes, or even create a new branch from that commit.

### `git checkout master`
* **Purpose:** Switches to the `master` branch.
* **Explanation:** `master` is often the main development branch of a repository. This command brings you back to the main line of development.

### `git clean`
* **Purpose:** Removes untracked files from the working directory.
* **Explanation:** This command can be useful when you've created temporary files or clutter that you don't want to include in your commits.

**Usage:**
* `git clean -f`: Removes untracked files, but asks for confirmation before deleting each.
* `git clean -d`: Removes untracked directories as well.
* `git clean -x`: Removes ignored files.

### `git rm`
* **Purpose:** Removes files from the repository.
* **Explanation:** This command removes files from both the working directory and the staging area.

**Usage:**
* `git rm <filename>`: Removes a specific file.
* `git rm -r <directory>`: Removes a directory and its contents.

### `git revert`
* **Purpose:** Creates a new commit that undoes the changes of a previous commit.
* **Explanation:** This command is useful when you need to revert a mistake or change that was later found to be incorrect.

**Usage:**
* `git revert <commit_hash>`: Reverts the specified commit.

**Example:**

```bash
# Switch to the master branch
git checkout master

# Remove all untracked files:
git clean -f

# Revert the last commit:
git revert HEAD
```

By understanding these commands, you can effectively navigate and manage your Git repository, undoing changes and restoring previous states as needed.

## .gitignore: Ignoring Files in Git

The `.gitignore` file is a powerful tool in Git that allows you to specify files or patterns of files that should be excluded from version control. This is useful for ignoring files that are generated automatically, temporary files, or files that you don't want to track in your repository.

**Creating a `.gitignore` File:**

1. **Create a new file:** In your Git repository's root directory, create a file named `.gitignore`.
2. **Add patterns:** Inside the `.gitignore` file, list the files or patterns of files that you want to ignore.

**Basic Patterns:**

* **Specific files:**
  ```
  file1.txt
  file2.jpg
  ```
* **Wildcards:**
  ```
  *.swp  # Ignore all files ending with ".swp" (common for Vim temporary files)
  *~      # Ignore all files starting with a tilde (common for backup files)
  ```
* **Directories:**
  ```
  build/
  dist/
  ```
* **Negation:**
  ```
  !node_modules/package-lock.json
  ```
  This will ignore all files in the `node_modules` directory except for `package-lock.json`.

**Example `.gitignore` File:**

```
# Build artifacts
build/
dist/

# Temporary files
*.swp
*~

# IDE configuration files
*.suo
*.user
*.sln

# Logs
*.log
```

**Important Notes:**

* The `.gitignore` file is case-sensitive.
* Patterns are matched from the beginning of the file path.
* To ignore files that have already been added to the repository, you'll need to use `git rm --cached <filename>` to remove them from the staging area, and then add the pattern to `.gitignore`.

By using a `.gitignore` file, you can keep your Git repository clean and organized by excluding unnecessary files from version control.

## Creating a Repository and Committing Changes on GitHub

While GitHub doesn't offer direct file editing functionality on the webpage GUI, there are two main ways to create a repository, commit changes, and push them to GitHub:

**1. Using the Webpage GUI:**

* **Create a Repository:**
   1. Go to your GitHub account and click on the "New repository" button.
   2. Give your repository a name, add a description (optional), and choose whether you want it to be public or private.
   3. Click "Create repository."

* **Committing Changes:**
   You'll need to use a local Git client like Git Bash or GitHub Desktop to commit changes. Install a local Git client, clone the repository you just created, make changes to the files, commit those changes locally, and then push them to the remote repository on GitHub.

**2. Using the Command Line (CLI):**

* **Create a Repository:**
   1. Open a terminal window.
   2. Use `git init` to initialize a local Git repository in your project directory.
   3. Run `git remote add origin <repository_url>` where `<repository_url>` is the URL of your newly created repository on GitHub. You can find this URL on your repository page on GitHub.

* **Committing Changes:**
   1. Make changes to your project files.
   2. Use `git add <filename>` to stage the files you want to commit.
   3. Run `git commit -m "Your commit message"` to create a commit with a descriptive message.
   4. Push your changes to the remote repository on GitHub using `git push origin main`.

**Here's a breakdown of the steps for both approaches:**

**Approach 1: Webpage GUI (requires local Git client)**

1. Create a new repository on GitHub.com.
2. Clone the repository to your local machine using a Git client.
3. Make changes to your project files locally.
4. Use the Git client to stage and commit your changes with a message.
5. Push the committed changes to the remote repository on GitHub.com.

**Approach 2: Command Line (CLI)**

1. Initialize a local Git repository in your project directory.
2. Add a remote pointing to your GitHub repository.
3. Make changes to your project files.
4. Stage the files you want to commit.
5. Create a commit with a descriptive message.
6. Push your committed changes to the remote repository on GitHub.com.

**Important Note:** Remember to replace `<repository_url>` with the actual URL of your repository on GitHub.

By using either of these approaches, you can effectively manage your code on GitHub and collaborate with others.

## Comprehensive Markdown table :

* We can use HTML for markdown

| Markdown Element | Description | Example |
|---|---|---|
| **Headings** | Create different levels of headings for structure | `# This is a Level 1 Heading` <br> `## This is a Level 2 Heading` <br> `### This is a Level 3 Heading` |
| **Paragraphs** | Define blocks of text | One or more lines of text separated by blank lines. |
| **Bold** | Emphasize text | `**This is bold text**` |
| **Italic** | Less emphasis than bold | `_This is italic text_` |
| **Strikethrough** | Text that is no longer relevant | `~~This is strikethrough text~~` |
| **Inline Code** | Code displayed within text | ` This is a function:  `code()\`\` |
| **Code Block** | Dedicated block for formatted code | ` javascript function add(x, y) { return x + y; }  `<br> \`python print("Hello, world\!") \` |
| **Quote** | Text presented as a quotation | \`\> This is a quoted passage.\` |
| **Unordered List** | List items without a specific order | \`\* Item 1\` <br> \`\* Item 2\` <br> \`  \* Sub-item\` |
| **Ordered List** | List items with a specific order (numbered) | \`1. Item 1\` <br> \`2. Item 2\` <br> \`   3. Sub-item\` |
| **Link** | Create a hyperlink to another resource | \`[Link Text] (https://www.example.com)`\` |
| **Image** | Embed an image | \`![Image Alt Text] (image src)\` |
| **Horizontal Rule** | Create a thematic line separator | \`\*\*\*\` <br> \`---\` <br> \`\_\_\_\` |
| **Table** | Organize data in a tabular format |

```markdown
| Header 1 | Header 2 | Header 3 |
|---|---|---|
| Cell 1, Row 1 | Cell 2, Row 1 | Cell 3, Row 1 |
| Cell 1, Row 2 | Cell 2, Row 2 | Cell 3, Row 2 |
```
### A Comprehensive List of Markdown Emojis

Markdown supports a wide range of emojis that can be used to add expressiveness and personality to your text. Here's a comprehensive list of commonly used emojis, along with their corresponding syntax:

**Basic Emojis:**

| Emoji | Syntax |
|---|---|
| 😊 | `:)` or `:-)` |
| 😃 | `:)` or `:-)` |
| 😄 | `:)` or `:-)` |
| 😁 | `:)` or `:-)` |
| 😅 | `;)` or `;-)` |
| 😂 | `:)` or `:-)` |
| 🤣 | `:)` or `:-)` |
| 😭 | `:(` or `:-(`) |
| 😥 | `:(` or `:-(`) |
| 😓 | `:(` or `:-(`) |
| 😲 | `:(` or `:-(`) |
| 🤯 | `:(` or `:-(`) |
| 😇 | `:)` or `:-)` |
| 😈 | `:)` or `:-)` |
| 💩 | `:(` or `:-(`) |
| ❤️ | `<3` |
| 👍 | `:+1:` |
| 👎 | `:-1:` |

**Other Emojis:**

| Emoji | Syntax |
|---|---|
| 🎉 | `:tada:` |
| 🎁 | `:gift:` |
| 🎈 | `:balloon:` |
| 🎂 | `:cake:` |
| ☕ | `:coffee:` |
| 🍺 | `:beer:` |
| 🍷 | `:wine_glass:` |
| 🍕 | `:pizza:` |
| 🍔 | `:hamburger:` |
| 🍟 | `:fries:` |
| 🍦 | `:ice_cream:` |
| 🍿 | `:popcorn:` |
| 🎥 | `:film:` |
| 🎧 | `:headphones:` |
| 🎮 | `:video_game:` |
| ⚽️ | `:soccer:` |
| 🏀 | `:basketball:` |
| 🎾 | `:tennis:` |
| 🏈 | `:football:` |
| ⚾️ | `:baseball:` |
| 🚗 | `:car:` |
| ✈️ | `:airplane:` |
| 🏠 | `:house:` |
| 🌳 | `:tree:` |
| ☀️ | `:sun:` |
| 🌙 | `:moon:` |
| ☁️ | `:cloud:` |
| ☔️ | `:umbrella:` |
| ❄️ | `:snowflake:` |
| ⚡ | `:zap:` |
| 🔔 | `:bell:` |
| 📱 | `:mobile:` |
| 💻 | `:computer:` |
| 📚 | `:books:` |
| ✏️ | `:pencil:` |
| 📝 | `:notebook:` |
| 📎 | `:paperclip:` |
| 🔑 | `:key:` |
| 🔒 | `:lock:` |
| 🔓 | `:unlock:` |

**Note:** The specific syntax for emojis may vary slightly depending on the platform or application you're using. However, the syntax provided here is generally compatible with most Markdown renderers.

You can find more information about emojis and their syntax on websites like [https://github.com/github/gemoji](https://github.com/github/gemoji) and [https://emojipedia.org/](https://emojipedia.org/).

###### Examples
```
# Heading 1

## Heading 2

### Heading 3

#### Heading 4

##### Heading 5

###### Heading 6

<!-- Comment -->

This is normal text, One or more lines of text separated by blank lines or double_space.

**This is Bold Text**  
_This is italic Text_  
~~This is Strikethrough text~~

**Single line code**  
`printf("Hello World)`

**Multi line Code**

```C            .
#include<stdio.h>

int main(){
    printf("Hello World");
    return 0;
}
```        .

> This is a quoted passage

**Unorder List**

- List item 1
- List item 2
- List item 3

**Order List**

1. List item 1
2. List item 2
3. List item 3

**Tasks**

- [x] Complete feature X
- [-] Fix bug Y
- [ ] Write unit tests for Z
- [ ] Update documentation

**Link**  
[Git Tutorial](https://github.com/sanu151/git-tutorial)

**Image**
![alt text](image.png)

<!-- [Image Text](image Source) -->

**Horizontal Rule**

---

**Table**
| Heading 1 | Heading 2 | Heading 3 |
|---|---|---|
| Data 1 | Data 2 | Data 3 |
| Data 4 | Data 5 | Data 6 |

**Emoji**  
😊 <!--Copy and Pest is the best option-->
```


**Additional Notes:**

  * You can escape special characters in Markdown by using a backslash (`\`) before them.
  * Use `#` for comments within your Markdown file.
  * There are extensions for Markdown that provide additional features, such as footnotes, tables of contents, and syntax highlighting for specific programming languages.

By using these elements effectively, you can create well-structured, informative, and visually appealing README.md files for your projects.


## Connecting Your Local and Remote Git Repositories

**Understanding the Connection:**

* **Local Repository:** A Git repository stored on your local computer.
* **Remote Repository:** A Git repository hosted on a remote server, like GitHub, GitLab, or Bitbucket.

**Establishing the Connection:**

1. **Create a Local Repository:**
   - Navigate to your project directory in the terminal.
   - Initialize a Git repository:
     ```bash
     git init
     ```

2. **Add a Remote:**
   - Connect your local repository to the remote repository:
     ```bash
     git remote add origin <remote_repository_url>
     ```
   - Replace `<remote_repository_url>` with the actual URL of your remote repository.

**Pushing Changes to the Remote:**

* Once you have made changes and committed them locally, you can push them to the remote repository:
   ```bash
   git push -u origin main
   ```
   - This command pushes the changes from your local `main` branch to the `main` branch on the remote repository.

**Pulling Changes from the Remote:**

* To fetch and merge changes from the remote repository into your local repository:
   ```bash
   git pull origin main
   ```

**Additional Notes:**

* You can use other branch names instead of `main` if your remote repository uses different branch names.
* If you encounter any errors, make sure you have the correct remote URL and that you're authenticated with the remote repository.
* For more complex scenarios, you might need to use additional Git commands like `git fetch`, `git merge`, and `git rebase`.

**Example:**

If your remote repository is on GitHub and its URL is `https://github.com/yourusername/yourrepository.git`, you would use the following commands:

```bash
git init
git remote add origin https://github.com/yourusername/yourrepository.git
git push -u origin main
```

By following these steps, you can successfully connect your local and remote Git repositories, enabling you to collaborate with others and manage your projects effectively.

**Git Push:**

- **Purpose:** Sends local changes from your working directory to a remote repository.
- **Workflow:**
    1. **Make changes:** Modify files in your working directory.
    2. **Stage changes:** Add modified files to the staging area using `git add <filename>`.
    3. **Commit changes:** Create a new commit with the staged changes using `git commit -m "Commit message"`.
    4. **Push changes:** Send the commit to the remote repository using `git push <remote> <branch>`.
- **Example:**
    ```bash
    git push origin main
    ```
    This command pushes the current branch (likely `main`) to the remote repository named `origin`.

**Git Pull:**

- **Purpose:** Fetches changes from a remote repository and merges them into your local working directory.
- **Workflow:**
    1. **Fetch changes:** Download the latest changes from the remote repository using `git fetch <remote>`.
    2. **Merge changes:** Merge the fetched changes into your local branch using `git merge <remote>/<branch>`.
- **Example:**
    ```bash
    git pull origin main
    ```
    This command fetches changes from the `main` branch of the `origin` remote repository and merges them into your current local branch.

**Git Clone:**

- **Purpose:** Creates a local copy of a remote repository.
- **Workflow:**
    1. **Clone repository:** Create a local copy of the repository using `git clone <repository URL>`.
- **Example:**
    ```bash
    git clone https://github.com/user/repository.git
    ```
    This command clones the repository with the URL [https://github.com/user/repository.git](https://github.com/user/repository.git) into a new directory named `repository`.

**Key Points:**

- **Remote repository:** A central location where Git stores the history of your project.
- **Local repository:** A copy of the remote repository on your local machine.
- **Branch:** A parallel line of development within a repository.
- **Commit:** A snapshot of the repository's state at a particular point in time.
- **Working directory:** The directory where you edit your files.

By understanding these commands and their workflows, you can effectively manage your Git repositories and collaborate with others on your projects.

### Git Branch and Marge

**Git Branch:**

- **Purpose:** Creates a new branch in your Git repository.
- **Workflow:**
    1. **Create a new branch:** Use `git branch <branch-name>` to create a new branch.
    2. **Switch to the new branch:** Use `git checkout <branch-name>` to start working on the new branch.
- **Example:**
    ```bash
    git branch feature-new-feature
    git checkout feature-new-feature
    ```
    This creates a new branch named `feature-new-feature` and switches to it.

**Git Merge:**

- **Purpose:** Combines changes from one branch into another.
- **Workflow:**
    1. **Switch to the target branch:** Use `git checkout <target-branch>` to switch to the branch where you want to merge the changes.
    2. **Merge the source branch:** Use `git merge <source-branch>` to merge the changes from the source branch into the target branch.
- **Example:**
    ```bash
    git checkout main
    git merge feature-new-feature
    ```
    This merges the changes from the `feature-new-feature` branch into the `main` branch.

#### Delete a branch

To delete a branch in Git using the command line interface (CLI), you can use the `git branch` command with the `-d` or `-D` option.

Here's a breakdown of the options:

- **`-d`:** Deletes the branch only if it has been merged into the current branch.
- **`-D`:** Deletes the branch unconditionally, even if it has not been merged.

**Example:**

To delete a branch named "feature_branch":

```bash
git branch -d feature_branch
```

If you want to force delete the branch, regardless of whether it has been merged, use:

```bash
git branch -D feature_branch
```

**Important Notes:**

- **Deleting a branch permanently removes its history.** Make sure you have a backup or have merged the changes from the branch into another branch before deleting it.
- If you're unsure whether a branch has been merged, you can use `git branch --merged` to list branches that have been merged into the current branch.

**Key Points:**

- **Branch:** A parallel line of development within a repository.
- **Merge:** The process of combining changes from one branch into another.
- **Conflict:** A situation where Git cannot automatically merge changes due to overlapping modifications.
- **Fast-forward merge:** A simple merge where Git can directly update the target branch with the changes from the source branch.
- **Non-fast-forward merge:** A more complex merge where Git creates a new commit to combine the changes from both branches.

**Additional Considerations:**

- **Rebase:** An alternative to merging that rewrites the commit history of a branch onto another branch. This can result in a cleaner commit history but can also introduce conflicts.
- **Cherry-picking:** A way to select specific commits from one branch and apply them to another branch.
- **Squashing:** A way to combine multiple commits into a single commit.

By understanding these commands and their workflows, you can effectively manage your Git branches and merge changes between them to collaborate on your projects.

## GitHub Issues: Tracking Tasks and Bugs

**GitHub Issues** is a powerful tool within the GitHub platform that allows you to track, manage, and discuss tasks, bugs, and feature requests related to your projects. It provides a centralized location for teams to collaborate, prioritize work, and keep track of project progress.

**Creating an issue**  
Issues can be created in a variety of ways, so you can choose the most convenient method for your workflow.

Who can use this feature?  
* People with read access can create an issue in a repository where issues are enabled.

Repository administrators can disable issues for a repository. For more information, see "Disabling issues."

#### Creating an issue from a repository  
* On GitHub, navigate to the main page of the repository.

* Under your repository name, click  Issues.  
![image](https://github.com/user-attachments/assets/4885ccee-2de2-4d8a-b441-542f8f4a9e93)

* Click New issue.

* If your repository uses issue templates, next to the type of issue you'd like to open, click Get started.  

If the type of issue you'd like to open isn't included in the available options, click Open a blank issue.

![image](https://github.com/user-attachments/assets/4c99e773-9f9a-4abf-a802-e5db9d80a863)


* In the comment body field, type a description of your issue.

* If you're a project maintainer, you can `assign the issue to someone`, `add it to a project`, `associate it with a milestone`, or` apply a label`.

* When you're finished, click `Submit new` issue.

#### Creating an issue with GitHub CLI
GitHub CLI is an open source tool for using GitHub from your computer's command line. When you're working from the command line, you can use the GitHub CLI to save time and avoid switching context. To learn more about GitHub CLI, see "[About GitHub CLI](https://docs.github.com/en/github-cli/github-cli/about-github-cli)."

To create an issue, use the `gh issue create` subcommand. To skip the interactive prompts, include the `--body` and the `--title` flags.
```
gh issue create --title "My new issue" --body "Here are more details."
```
You can also specify assignees, labels, milestones, and projects.
```
gh issue create --title "My new issue" --body "Here are more details." --assignee @me,monalisa --label "bug,help wanted" --project onboarding --milestone "learning codebase"
```

#### Creating an issue from a comment  
You can open a new issue from a comment in an issue or pull request. When you open an issue from a comment, the issue contains a snippet showing where the comment was originally posted.

* Navigate to the comment that you would like to open an issue from.

* In that comment, click ...

![image](https://github.com/user-attachments/assets/41f90177-a183-4121-b6ac-0c191675b80b)

* Click **Reference in new issue**.

* Use the "Repository" dropdown menu, and select the repository you want to open the issue in.

* Type a descriptive title and body for the issue.

* Click Create issue.


**Key Features of GitHub Issues:**

* **Issue Creation:** You can create new issues to report bugs, propose features, or track tasks.
* **Issue Tracking:** Assign issues to team members, set due dates, and add labels to categorize and organize them.
* **Comments and Discussions:** Collaborate with your team by adding comments and discussions to issues.
* **Milestones:** Group related issues into milestones to track project progress.
* **Labels:** Use labels to categorize issues based on their type, priority, or other criteria.
* **Assignees:** Assign issues to specific team members to assign responsibility.
* **Project Boards:** Visualize your project's workflow using Kanban boards or other board styles.

**Using GitHub Issues Effectively:**

* **Clear Issue Descriptions:** Provide detailed descriptions of issues, including steps to reproduce bugs or desired features.
* **Utilize Labels:** Use labels to categorize issues and make them easier to find and manage.
* **Assign Issues:** Assign issues to the appropriate team members to ensure accountability.
* **Set Due Dates:** Set realistic due dates to track progress and prioritize tasks.
* **Hold Regular Reviews:** Review open and closed issues regularly to assess project progress and identify any bottlenecks.
* **Use Project Boards:** Visualize your project's workflow using Kanban boards or other board styles.

**Example:**

If you're working on a web application and encounter a bug, you could create a new issue with the following information:

* **Title:** "Error message appears when clicking on 'Submit' button"
* **Description:** "When I click on the 'Submit' button, an error message appears saying 'Invalid input.' This happens consistently on Chrome and Firefox."
* **Labels:** "bug", "high priority"
* **Assignee:** John Doe (the developer responsible for the 'Submit' button)

By using GitHub Issues effectively, you can improve collaboration, streamline your development process, and ensure that your projects are delivered on time and with high quality.

### **Fast-forward Merge in Git**

A fast-forward merge in Git is a type of merge that occurs when the branch you're merging into (the target branch) hasn't diverged from the branch you're merging from (the source branch) since the last commit on the source branch. 

**How it works:**  
* Instead of creating a new merge commit, Git simply moves the target branch's pointer forward to the tip of the source branch.  
* This effectively integrates the changes from the source branch into the target branch without creating any additional merge commit.  
* It maintains a linear history, making it easier to follow the evolution of the codebase.
  
**When does it happen:**  
* You're merging a feature branch back into the main branch, and no changes have been made to the main branch since the feature branch was created.  
* You're pulling changes from a remote repository, and your local branch is up-to-date with the remote branch.  

**Conditions for a Fast-Forward Merge:**

* The branch being merged must be a direct descendant of the current branch.
* There must be no commits on the current branch that are not also on the branch being merged.

**Steps to Perform a Fast-Forward Merge:**

1. **Switch to the branch you want to merge into:**
   ```bash
   git checkout main
   ```

2. **Merge the other branch:**
   ```bash
   git merge feature_branch
   ```

If the merge is a fast-forward, Git will display a message like:

```
Updating 9876543210abcdef1234567890...
Fast-forward
```
![Fast-Forword Marge](https://miro.medium.com/v2/resize:fit:1400/0*GhW5WSCRH1dneU6c.gif)


**Advantages of Fast-Forward Merges:**

* **Simple and Efficient:** Fast-forward merges are straightforward and don't create unnecessary merge commits.
* **Cleaner History:** They keep your commit history linear, making it easier to follow and understand.

**When to Use Fast-Forward Merges:**

* When you want to merge a branch that has only new commits and no conflicting changes.
* When you want to keep your commit history clean and linear.

**Disabling fast-forward merges:**
If you want to explicitly create a merge commit even when a fast-forward merge is possible, use the --no-ff flag:

```bash
git merge --no-ff feature-branch
```

**Note:** If there are conflicting changes between the two branches, a fast-forward merge will not be possible. In this case, Git will stop and require you to resolve the conflicts before completing the merge.

By understanding fast-forward merges, you can effectively merge branches in Git and maintain a clean commit history.

**3-Way Merge in Git**

A 3-way merge is a more complex type of merge that Git performs when there are conflicting changes between the two branches being merged. In this scenario, Git compares the changes in both branches to a common ancestor commit to determine how to resolve the conflicts.

**Steps Involved in a 3-Way Merge:**

1. **Identify Common Ancestor:** Git finds the common ancestor commit of the two branches being merged.
2. **Compare Changes:** Git compares the changes made in each branch relative to the common ancestor.
3. **Resolve Conflicts:** If there are conflicting changes, Git will stop and indicate the files that need to be resolved. You'll need to manually edit the files to resolve the conflicts and decide which changes to keep.
4. **Stage Resolved Changes:** Once you've resolved the conflicts, stage the changes using `git add`.
5. **Complete the Merge:** Use `git commit` to create a new commit that represents the merged changes.

**Example:**

```bash
git checkout main
git merge feature_branch
```

If there are conflicts, Git will display a message like:

```
Auto-merging conflicting file: path/to/file.txt
CONFLICT (content): Merge conflict in path/to/file.txt
Automatic merge failed; fix conflicts and then commit.
```

You'll need to edit `path/to/file.txt` to resolve the conflicts, then stage the changes and commit the merge.

![3-way marge](https://kodekloud.com/blog/content/images/2023/10/git-merge.gif)

**Advantages of 3-Way Merges:**

* **Handles Conflicts Effectively:** 3-way merges can help resolve conflicts more accurately by comparing changes to a common ancestor.
* **Preserves History:** They preserve the history of both branches, making it easier to understand the development process.

**When to Use 3-Way Merges:**

* When there are conflicting changes between the branches being merged.
* When you want to preserve a detailed history of your project.

By understanding 3-way merges, you can effectively handle conflicts in Git and maintain a clean and accurate project history.

## Resolving Merge Conflicts in Git

Merge conflicts occur when Git encounters conflicting changes between two branches that are being merged. This happens when both branches have modified the same file or portion of a file.

**Steps to Resolve Merge Conflicts:**

1. **Identify Conflicting Files:**
   - After attempting a merge, Git will indicate which files have conflicts. You can use the `git status` command to see which files are marked as "unmerged".

2. **Open Conflicting Files:**
   - Open the conflicting files in your text editor. Git will usually add markers like `<<<<<<< HEAD`, `=======`, and `>>>>>>>` to indicate the conflicting sections.

3. **Manually Resolve Conflicts:**
   - Carefully review the conflicting sections and decide which changes you want to keep.
   - Edit the file to resolve the conflicts, removing the conflict markers and making the necessary changes.

4. **Stage Resolved Files:**
   - Once you've resolved the conflicts, stage the modified files using `git add`:
     ```bash
     git add <filename>
     ```

5. **Commit the Merge:**
   - Create a new commit to merge the changes:
     ```bash
     git commit -m "Merged feature_branch with conflict resolution"
     ```

**Example:**

```
Auto-merging conflicting file: path/to/file.txt
CONFLICT (content): Merge conflict in path/to/file.txt
Automatic merge failed; fix conflicts and then commit.
```

In this example, `path/to/file.txt` has conflicting changes. You'll need to open the file, resolve the conflicts, and then stage and commit the changes.

**Tips for Resolving Conflicts:**

* **Review Changes Carefully:** Examine the conflicting sections carefully to understand the differences between the branches.
* **Consider Using a Merge Tool:** Some Git clients or external tools can help visualize and resolve conflicts more easily.
* **Create a Backup:** Before making changes, consider creating a backup of the conflicting file in case you need to revert.

By following these steps and carefully resolving conflicts, you can successfully merge branches in Git even when there are conflicting changes.

## Resolving Merge Conflicts on GitHub

**Understanding Merge Conflicts**

Merge conflicts occur when you attempt to merge two branches that have modified the same file or portion of a file. This can happen when different developers work on the same codebase simultaneously or when you rebase a branch onto another.

**Resolving Conflicts on GitHub:**

1. **Identify Conflicting Files:**
   - GitHub will usually notify you of merge conflicts when you push your changes to a remote repository. You can also check the "Pull Requests" tab to see if any merge conflicts are blocking your pull request.

2. **Fetch the Remote Changes:**
   - If you haven't already, fetch the latest changes from the remote repository:
     ```bash
     git fetch origin
     ```

3. **View Conflicting Files:**
   - GitHub provides a visual diff tool to compare the conflicting changes. You can review the conflicting sections and decide which changes to keep.

4. **Resolve Conflicts Locally:**
   - If the conflicts are complex or you prefer to work locally, you can checkout the branch with the conflicts:
     ```bash
     git checkout <branch_name>
     ```
   - Resolve the conflicts manually in your text editor.
   - Stage the resolved files:
     ```bash
     git add <filename>
     ```
   - Commit the changes:
     ```bash
     git commit -m "Resolved merge conflicts"
     ```

5. **Push the Resolved Changes:**
   - Push your changes back to the remote repository:
     ```bash
     git push origin <branch_name>
     ```

**Additional Tips:**

* **Use GitHub's Merge Conflict Viewer:** GitHub provides a visual diff tool that can help you understand and resolve conflicts more easily.
* **Create a Backup:** Before making changes, consider creating a backup of the conflicting file in case you need to revert.
* **Communicate with Teammates:** If you're working with a team, communicate with other developers to coordinate conflict resolution.

By following these steps and using GitHub's tools effectively, you can resolve merge conflicts efficiently and continue working on your project.


<body id="documentation">

  <div class="inner">
    <header>

  <a href="/"><img src="/images/logo@2x.png" width="110" height="46" alt="Git"></a>
  <span id="tagline">--fast-version-control</span>
  <script type="text/javascript">
    const taglines = [
      "fast-version-control",
      "everything-is-local",
      "distributed-even-if-your-workflow-isnt",
      "local-branching-on-the-cheap",
      "distributed-is-the-new-centralized"
    ];
    var tagline = taglines[Math.floor(Math.random() * taglines.length)];
    document.getElementById('tagline').innerHTML = '--' + tagline;
  </script>

  
  <form id="search" action="/search/results">
    <input id="search-text" name="search" placeholder="Type / to search entire site…" autocomplete="off" type="text">
  </form>
  <div id="search-results"></div>
  

</header>

  </div> 

  
    
    <div class="inner">
      <div id="content-wrapper">
        
<button class="sidebar-btn"></button>
<aside class="sidebar" id="sidebar">
  <nav>
    <ul>
      <li>
        <a href="/about">About</a>
        <ul>
          
        </ul>
      </li>
      <li>
        <a href="/doc" class="active">Documentation</a>
        <ul class="expanded">
          <li>
            <a href="/docs">Reference</a>
          </li>
          <li>
            <a href="/book" class="active">Book</a>
          </li>
          <li>
            <a href="/videos">Videos</a>
          </li>
          <li>
            <a href="/doc/ext">External Links</a>
          </li>
        </ul>
      </li>
      <li>
        <a href="/downloads">Downloads</a>
        <ul>
          <li>
            <a href="/downloads/guis">GUI Clients</a>
          </li>
          <li>
            <a href="/downloads/logos">Logos</a>
          </li>
        </ul>
      </li>
      <li>
        <a href="/community">Community</a>
      </li>
    </ul>
    
      <hr class="sidebar">
      <p>
This book is available in
  <a href="/book/en">English</a>.
</p>
<p>
  Full translation available in
  </p><table>
    <tbody><tr><td><a href="/book/az">azərbaycan dili</a>,</td></tr>
    <tr><td><a href="/book/bg">български език</a>,</td></tr>
    <tr><td><a href="/book/de">Deutsch</a>,</td></tr>
    <tr><td><a href="/book/es">Español</a>,</td></tr>
    <tr><td><a href="/book/fr">Français</a>,</td></tr>
    <tr><td><a href="/book/gr">Ελληνικά</a>,</td></tr>
    <tr><td><a href="/book/ja">日本語</a>,</td></tr>
    <tr><td><a href="/book/ko">한국어</a>,</td></tr>
    <tr><td><a href="/book/nl">Nederlands</a>,</td></tr>
    <tr><td><a href="/book/ru">Русский</a>,</td></tr>
    <tr><td><a href="/book/sl">Slovenščina</a>,</td></tr>
    <tr><td><a href="/book/tl">Tagalog</a>,</td></tr>
    <tr><td><a href="/book/uk">Українська</a></td></tr>
    <tr><td><a href="/book/zh">简体中文</a>,</td></tr>
  </tbody></table>
<p></p>
<p>
  Partial translations available in
  </p><table>
    <tbody><tr><td><a href="/book/cs">Čeština</a>,</td></tr>
    <tr><td><a href="/book/mk">Македонски</a>,</td></tr>
    <tr><td><a href="/book/pl">Polski</a>,</td></tr>
    <tr><td><a href="/book/sr">Српски</a>,</td></tr>
    <tr><td><a href="/book/uz">Ўзбекча</a>,</td></tr>
    <tr><td><a href="/book/zh-tw">繁體中文</a>,</td></tr>
  </tbody></table>
<p></p>
<p>
  Translations started for
  </p><table>
    <tbody><tr><td><a href="/book/be">Беларуская</a>,</td></tr>
    <tr><td><a href="/book/fa" dir="rtl">فارسی</a>,</td></tr>
    <tr><td><a href="/book/id">Indonesian</a>,</td></tr>
    <tr><td><a href="/book/it">Italiano</a>,</td></tr>
    <tr><td><a href="/book/ms">Bahasa Melayu</a>,</td></tr>
    <tr><td><a href="/book/pt-br">Português (Brasil)</a>,</td></tr>
    <tr><td><a href="/book/pt-pt">Português (Portugal)</a>,</td></tr>
    <tr><td><a href="/book/sv">Svenska</a>,</td></tr>
    <tr><td><a href="/book/tr">Türkçe</a>.</td></tr>
  </tbody></table>
<p></p>
<hr class="sidebar">
<p>
The source of this book is <a href="https://github.com/progit2-sv/progit2">hosted on GitHub.</a><br>
Patches, suggestions and comments are welcome.
</p>

    
  </nav>
</aside>

        <div id="content">
          
          <div id="book-chapters">
            <a class="dropdown-trigger" id="book-chapters-trigger" data-panel-id="chapters-dropdown" href="#">Chapters ▾</a>







<div class="dropdown-panel" id="chapters-dropdown">
  <div class="three-column">
    <div class="column-left">
      
      
      <ol class="book-toc">
  
  
  <li class="chapter">
  <h2>1. <a href="/book/sv/v2/Kom-ig%c3%a5ng-Om-versionshantering">Kom igång</a></h2>
    <ol>
      
        <li>
          1.1
          <a href="/book/sv/v2/Kom-ig%c3%a5ng-Om-versionshantering">Om versionshantering</a>
        </li>
      
        <li>
          1.2
          <a href="/book/sv/v2/Kom-ig%c3%a5ng-En-kort-historik-av-Git">En kort historik av Git</a>
        </li>
      
        <li>
          1.3
          <a href="/book/sv/v2/Kom-ig%c3%a5ng-Vad-%c3%a4r-Git%3F">Vad är Git?</a>
        </li>
      
        <li>
          1.4
          <a href="/book/sv/v2/Kom-ig%c3%a5ng-Kommandoraden">Kommandoraden</a>
        </li>
      
        <li>
          1.5
          <a href="/book/sv/v2/Kom-ig%c3%a5ng-Installera-Git">Installera Git</a>
        </li>
      
        <li>
          1.6
          <a href="/book/sv/v2/Kom-ig%c3%a5ng-Anv%c3%a4nda-Git-f%c3%b6r-f%c3%b6rsta-g%c3%a5ngen">Använda Git för första gången</a>
        </li>
      
        <li>
          1.7
          <a href="/book/sv/v2/Kom-ig%c3%a5ng-F%c3%a5-hj%c3%a4lp">Få hjälp</a>
        </li>
      
        <li>
          1.8
          <a href="/book/sv/v2/Kom-ig%c3%a5ng-Sammanfattning">Sammanfattning</a>
        </li>
      
    </ol>
  </li>
  
  
  
  <li class="chapter">
  <h2>2. <a href="/book/sv/v2/Grunder-i-Git-Skaffa-ett-Git-f%c3%b6rvar">Grunder i Git</a></h2>
    <ol>
      
        <li>
          2.1
          <a href="/book/sv/v2/Grunder-i-Git-Skaffa-ett-Git-f%c3%b6rvar">Skaffa ett Git-förvar</a>
        </li>
      
        <li>
          2.2
          <a href="/book/sv/v2/Grunder-i-Git-Spara-%c3%a4ndringar-till-f%c3%b6rvaret">Spara ändringar till förvaret</a>
        </li>
      
        <li>
          2.3
          <a href="/book/sv/v2/Grunder-i-Git-Visa-historiken">Visa historiken</a>
        </li>
      
        <li>
          2.4
          <a href="/book/sv/v2/Grunder-i-Git-%c3%85ngra-saker">Ångra saker</a>
        </li>
      
        <li>
          2.5
          <a href="/book/sv/v2/Grunder-i-Git-Jobba-med-fj%c3%a4rrf%c3%b6rvar">Jobba med fjärrförvar</a>
        </li>
      
        <li>
          2.6
          <a href="/book/sv/v2/Grunder-i-Git-Taggning">Taggning</a>
        </li>
      
        <li>
          2.7
          <a href="/book/sv/v2/Grunder-i-Git-Git-alias">Git alias</a>
        </li>
      
        <li>
          2.8
          <a href="/book/sv/v2/Grunder-i-Git-Sammanfattning">Sammanfattning</a>
        </li>
      
    </ol>
  </li>
  
  
  
  <li class="chapter">
  <h2>3. <a href="/book/sv/v2/Git-f%c3%b6rgreningar-Grenar-i-ett-n%c3%b6tskal">Git förgreningar</a></h2>
    <ol>
      
        <li>
          3.1
          <a href="/book/sv/v2/Git-f%c3%b6rgreningar-Grenar-i-ett-n%c3%b6tskal">Grenar i ett nötskal</a>
        </li>
      
        <li>
          3.2
          <a href="/book/sv/v2/Git-f%c3%b6rgreningar-Grundl%c3%a4ggande-f%c3%b6rgrening-och-sammanslagning">Grundläggande förgrening och sammanslagning</a>
        </li>
      
        <li>
          3.3
          <a href="/book/sv/v2/Git-f%c3%b6rgreningar-Hantera-grenar">Hantera grenar</a>
        </li>
      
        <li>
          3.4
          <a href="/book/sv/v2/Git-f%c3%b6rgreningar-Arbetsfl%c3%b6de-med-grenar">Arbetsflöde med grenar</a>
        </li>
      
        <li>
          3.5
          <a href="/book/sv/v2/Git-f%c3%b6rgreningar-Fj%c3%a4rrgrenar">Fjärrgrenar</a>
        </li>
      
        <li>
          3.6
          <a href="/book/sv/v2/Git-f%c3%b6rgreningar-Grenflytt">Grenflytt</a>
        </li>
      
        <li>
          3.7
          <a href="/book/sv/v2/Git-f%c3%b6rgreningar-Sammanfattning">Sammanfattning</a>
        </li>
      
    </ol>
  </li>
  
  
  
  <li class="chapter">
  <h2>4. <a href="/book/sv/v2/Git-p%c3%a5-servern-Protokollen">Git på servern</a></h2>
    <ol>
      
        <li>
          4.1
          <a href="/book/sv/v2/Git-p%c3%a5-servern-Protokollen">Protokollen</a>
        </li>
      
        <li>
          4.2
          <a href="/book/sv/v2/Git-p%c3%a5-servern-Skaffa-Git-p%c3%a5-en-server">Skaffa Git på en server</a>
        </li>
      
        <li>
          4.3
          <a href="/book/sv/v2/Git-p%c3%a5-servern-Generera-din-publika-SSH-nyckel">Generera din publika SSH-nyckel</a>
        </li>
      
        <li>
          4.4
          <a href="/book/sv/v2/Git-p%c3%a5-servern-Konvigurera-servern">Konvigurera servern</a>
        </li>
      
        <li>
          4.5
          <a href="/book/sv/v2/Git-p%c3%a5-servern-Git-Daemonen">Git Daemonen</a>
        </li>
      
        <li>
          4.6
          <a href="/book/sv/v2/Git-p%c3%a5-servern-Smart-HTTP">Smart HTTP</a>
        </li>
      
        <li>
          4.7
          <a href="/book/sv/v2/Git-p%c3%a5-servern-GitWeb">GitWeb</a>
        </li>
      
        <li>
          4.8
          <a href="/book/sv/v2/Git-p%c3%a5-servern-GitLab">GitLab</a>
        </li>
      
        <li>
          4.9
          <a href="/book/sv/v2/Git-p%c3%a5-servern-Alternativ-tillhandah%c3%a5llna-av-tredje-part">Alternativ tillhandahållna av tredje part</a>
        </li>
      
        <li>
          4.10
          <a href="/book/sv/v2/Git-p%c3%a5-servern-Sammanfattning">Sammanfattning</a>
        </li>
      
    </ol>
  </li>
  
  
  
  <li class="chapter">
  <h2>5. <a href="/book/sv/v2/Distribuerade-Git-Distribuerade-arbetsfl%c3%b6den">Distribuerade Git</a></h2>
    <ol>
      
        <li>
          5.1
          <a href="/book/sv/v2/Distribuerade-Git-Distribuerade-arbetsfl%c3%b6den">Distribuerade arbetsflöden</a>
        </li>
      
        <li>
          5.2
          <a href="/book/sv/v2/Distribuerade-Git-Medverka-i-ett-projekt">Medverka i ett projekt</a>
        </li>
      
        <li>
          5.3
          <a href="/book/sv/v2/Distribuerade-Git-Underh%c3%a5lla-ett-projekt">Underhålla ett projekt</a>
        </li>
      
        <li>
          5.4
          <a href="/book/sv/v2/Distribuerade-Git-Sammanfattning">Sammanfattning</a>
        </li>
      
    </ol>
  </li>
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
</ol>

    </div>
    <div class="column-middle">
      
      
      <ol class="book-toc">
  
  
  
  
  
  
  
  
  
  
  
  
  <li class="chapter">
  <h2>6. <a href="/book/sv/v2/GitHub-Account-Setup-and-Configuration">GitHub</a></h2>
    <ol>
      
        <li>
          6.1
          <a href="/book/sv/v2/GitHub-Account-Setup-and-Configuration">Account Setup and Configuration</a>
        </li>
      
        <li>
          6.2
          <a href="/book/sv/v2/GitHub-Contributing-to-a-Project" class="active">Contributing to a Project</a>
        </li>
      
        <li>
          6.3
          <a href="/book/sv/v2/GitHub-Maintaining-a-Project">Maintaining a Project</a>
        </li>
      
        <li>
          6.4
          <a href="/book/sv/v2/GitHub-Managing-an-organization">Managing an organization</a>
        </li>
      
        <li>
          6.5
          <a href="/book/sv/v2/GitHub-Scripting-GitHub">Scripting GitHub</a>
        </li>
      
        <li>
          6.6
          <a href="/book/sv/v2/GitHub-Summary">Summary</a>
        </li>
      
    </ol>
  </li>
  
  
  
  <li class="chapter">
  <h2>7. <a href="/book/sv/v2/Git-Tools-Revision-Selection">Git Tools</a></h2>
    <ol>
      
        <li>
          7.1
          <a href="/book/sv/v2/Git-Tools-Revision-Selection">Revision Selection</a>
        </li>
      
        <li>
          7.2
          <a href="/book/sv/v2/Git-Tools-Interactive-Staging">Interactive Staging</a>
        </li>
      
        <li>
          7.3
          <a href="/book/sv/v2/Git-Tools-Stashing-and-Cleaning">Stashing and Cleaning</a>
        </li>
      
        <li>
          7.4
          <a href="/book/sv/v2/Git-Tools-Signing-Your-Work">Signing Your Work</a>
        </li>
      
        <li>
          7.5
          <a href="/book/sv/v2/Git-Tools-Searching">Searching</a>
        </li>
      
        <li>
          7.6
          <a href="/book/sv/v2/Git-Tools-Rewriting-History">Rewriting History</a>
        </li>
      
        <li>
          7.7
          <a href="/book/sv/v2/Git-Tools-Reset-Demystified">Reset Demystified</a>
        </li>
      
        <li>
          7.8
          <a href="/book/sv/v2/Git-Tools-Advanced-Merging">Advanced Merging</a>
        </li>
      
        <li>
          7.9
          <a href="/book/sv/v2/Git-Tools-Rerere">Rerere</a>
        </li>
      
        <li>
          7.10
          <a href="/book/sv/v2/Git-Tools-Debugging-with-Git">Debugging with Git</a>
        </li>
      
        <li>
          7.11
          <a href="/book/sv/v2/Git-Tools-Submodules">Submodules</a>
        </li>
      
        <li>
          7.12
          <a href="/book/sv/v2/Git-Tools-Bundling">Bundling</a>
        </li>
      
        <li>
          7.13
          <a href="/book/sv/v2/Git-Tools-Replace">Replace</a>
        </li>
      
        <li>
          7.14
          <a href="/book/sv/v2/Git-Tools-Credential-Storage">Credential Storage</a>
        </li>
      
        <li>
          7.15
          <a href="/book/sv/v2/Git-Tools-Summary">Summary</a>
        </li>
      
    </ol>
  </li>
  
  
  
  <li class="chapter">
  <h2>8. <a href="/book/sv/v2/Customizing-Git-Git-Configuration">Customizing Git</a></h2>
    <ol>
      
        <li>
          8.1
          <a href="/book/sv/v2/Customizing-Git-Git-Configuration">Git Configuration</a>
        </li>
      
        <li>
          8.2
          <a href="/book/sv/v2/Customizing-Git-Git-Attributes">Git Attributes</a>
        </li>
      
        <li>
          8.3
          <a href="/book/sv/v2/Customizing-Git-Git-Hooks">Git Hooks</a>
        </li>
      
        <li>
          8.4
          <a href="/book/sv/v2/Customizing-Git-An-Example-Git-Enforced-Policy">An Example Git-Enforced Policy</a>
        </li>
      
        <li>
          8.5
          <a href="/book/sv/v2/Customizing-Git-Summary">Summary</a>
        </li>
      
    </ol>
  </li>
  
  
  
  <li class="chapter">
  <h2>9. <a href="/book/sv/v2/Git-and-Other-Systems-Git-as-a-Client">Git and Other Systems</a></h2>
    <ol>
      
        <li>
          9.1
          <a href="/book/sv/v2/Git-and-Other-Systems-Git-as-a-Client">Git as a Client</a>
        </li>
      
        <li>
          9.2
          <a href="/book/sv/v2/Git-and-Other-Systems-Migrating-to-Git">Migrating to Git</a>
        </li>
      
        <li>
          9.3
          <a href="/book/sv/v2/Git-and-Other-Systems-Summary">Summary</a>
        </li>
      
    </ol>
  </li>
  
  
  
  <li class="chapter">
  <h2>10. <a href="/book/sv/v2/Git-Internals-Plumbing-and-Porcelain">Git Internals</a></h2>
    <ol>
      
        <li>
          10.1
          <a href="/book/sv/v2/Git-Internals-Plumbing-and-Porcelain">Plumbing and Porcelain</a>
        </li>
      
        <li>
          10.2
          <a href="/book/sv/v2/Git-Internals-Git-Objects">Git Objects</a>
        </li>
      
        <li>
          10.3
          <a href="/book/sv/v2/Git-Internals-Git-References">Git References</a>
        </li>
      
        <li>
          10.4
          <a href="/book/sv/v2/Git-Internals-Packfiles">Packfiles</a>
        </li>
      
        <li>
          10.5
          <a href="/book/sv/v2/Git-Internals-The-Refspec">The Refspec</a>
        </li>
      
        <li>
          10.6
          <a href="/book/sv/v2/Git-Internals-Transfer-Protocols">Transfer Protocols</a>
        </li>
      
        <li>
          10.7
          <a href="/book/sv/v2/Git-Internals-Maintenance-and-Data-Recovery">Maintenance and Data Recovery</a>
        </li>
      
        <li>
          10.8
          <a href="/book/sv/v2/Git-Internals-Environment-Variables">Environment Variables</a>
        </li>
      
        <li>
          10.9
          <a href="/book/sv/v2/Git-Internals-Summary">Summary</a>
        </li>
      
    </ol>
  </li>
  
  
  
  
  
  
  
  
</ol>

    </div>
    <div class="column-right">
      
      
      <ol class="book-toc">
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  <li class="chapter">
  <h2>A1. <a href="/book/sv/v2/Bilaga-A:-Git-in-Other-Environments-Graphical-Interfaces">Bilaga A: Git in Other Environments</a></h2>
    <ol>
      
        <li>
          A1.1
          <a href="/book/sv/v2/Bilaga-A:-Git-in-Other-Environments-Graphical-Interfaces">Graphical Interfaces</a>
        </li>
      
        <li>
          A1.2
          <a href="/book/sv/v2/Bilaga-A:-Git-in-Other-Environments-Git-in-Visual-Studio">Git in Visual Studio</a>
        </li>
      
        <li>
          A1.3
          <a href="/book/sv/v2/Bilaga-A:-Git-in-Other-Environments-Git-in-Eclipse">Git in Eclipse</a>
        </li>
      
        <li>
          A1.4
          <a href="/book/sv/v2/Bilaga-A:-Git-in-Other-Environments-Git-in-Bash">Git in Bash</a>
        </li>
      
        <li>
          A1.5
          <a href="/book/sv/v2/Bilaga-A:-Git-in-Other-Environments-Git-in-Zsh">Git in Zsh</a>
        </li>
      
        <li>
          A1.6
          <a href="/book/sv/v2/Bilaga-A:-Git-in-Other-Environments-Git-in-PowerShell">Git in PowerShell</a>
        </li>
      
        <li>
          A1.7
          <a href="/book/sv/v2/Bilaga-A:-Git-in-Other-Environments-Summary">Summary</a>
        </li>
      
    </ol>
  </li>
  
  
  
  <li class="chapter">
  <h2>A2. <a href="/book/sv/v2/Bilaga-B:-Embedding-Git-in-your-Applications-Command-line-Git">Bilaga B: Embedding Git in your Applications</a></h2>
    <ol>
      
        <li>
          A2.1
          <a href="/book/sv/v2/Bilaga-B:-Embedding-Git-in-your-Applications-Command-line-Git">Command-line Git</a>
        </li>
      
        <li>
          A2.2
          <a href="/book/sv/v2/Bilaga-B:-Embedding-Git-in-your-Applications-Libgit2">Libgit2</a>
        </li>
      
        <li>
          A2.3
          <a href="/book/sv/v2/Bilaga-B:-Embedding-Git-in-your-Applications-JGit">JGit</a>
        </li>
      
        <li>
          A2.4
          <a href="/book/sv/v2/Bilaga-B:-Embedding-Git-in-your-Applications-go-git">go-git</a>
        </li>
      
        <li>
          A2.5
          <a href="/book/sv/v2/Bilaga-B:-Embedding-Git-in-your-Applications-Dulwich">Dulwich</a>
        </li>
      
    </ol>
  </li>
  
  
  
  <li class="chapter">
  <h2>A3. <a href="/book/sv/v2/Bilaga-C:-Git-Commands-Setup-and-Config">Bilaga C: Git Commands</a></h2>
    <ol>
      
        <li>
          A3.1
          <a href="/book/sv/v2/Bilaga-C:-Git-Commands-Setup-and-Config">Setup and Config</a>
        </li>
      
        <li>
          A3.2
          <a href="/book/sv/v2/Bilaga-C:-Git-Commands-Getting-and-Creating-Projects">Getting and Creating Projects</a>
        </li>
      
        <li>
          A3.3
          <a href="/book/sv/v2/Bilaga-C:-Git-Commands-Basic-Snapshotting">Basic Snapshotting</a>
        </li>
      
        <li>
          A3.4
          <a href="/book/sv/v2/Bilaga-C:-Git-Commands-Branching-and-Merging">Branching and Merging</a>
        </li>
      
        <li>
          A3.5
          <a href="/book/sv/v2/Bilaga-C:-Git-Commands-Sharing-and-Updating-Projects">Sharing and Updating Projects</a>
        </li>
      
        <li>
          A3.6
          <a href="/book/sv/v2/Bilaga-C:-Git-Commands-Inspection-and-Comparison">Inspection and Comparison</a>
        </li>
      
        <li>
          A3.7
          <a href="/book/sv/v2/Bilaga-C:-Git-Commands-Debugging">Debugging</a>
        </li>
      
        <li>
          A3.8
          <a href="/book/sv/v2/Bilaga-C:-Git-Commands-Patching">Patching</a>
        </li>
      
        <li>
          A3.9
          <a href="/book/sv/v2/Bilaga-C:-Git-Commands-Email">Email</a>
        </li>
      
        <li>
          A3.10
          <a href="/book/sv/v2/Bilaga-C:-Git-Commands-External-Systems">External Systems</a>
        </li>
      
        <li>
          A3.11
          <a href="/book/sv/v2/Bilaga-C:-Git-Commands-Administration">Administration</a>
        </li>
      
        <li>
          A3.12
          <a href="/book/sv/v2/Bilaga-C:-Git-Commands-Plumbing-Commands">Plumbing Commands</a>
        </li>
      
    </ol>
  </li>
  
  
</ol>

    </div>
  </div>
</div>


            <span class="light" id="edition">
              2nd Edition
            </span>
          </div>
          <div id="main" data-pagefind-filter="category:book" data-pagefind-meta="category:Book" data-pagefind-weight="0.05" data-pagefind-body="" class="book edition2">
            <h1>6.2 GitHub - Contributing to a Project</h1>
            <div>
              <h2 id="_contributing_to_a_project">Contributing to a Project</h2>
<div class="paragraph">
<p>Now that our account is set up, let’s walk through some details that could be useful in helping you contribute to an existing project.</p>
</div>
<div class="sect3">
<h3 id="_forking_projects">Forking Projects</h3>
<div class="paragraph">
<p>
If you want to contribute to an existing project to which you don’t have push access, you can “fork” the project.
When you “fork” a project, GitHub will make a copy of the project that is entirely yours; it lives in your namespace, and you can push to it.</p>
</div>
<div class="admonitionblock note">
<table>
<tbody><tr>
<td class="icon">
<div class="title">Notera</div>
</td>
<td class="content">
<div class="paragraph">
<p>Historically, the term “fork” has been somewhat negative in context, meaning that someone took an open source project in a different direction, sometimes creating a competing project and splitting the contributors.
In GitHub, a “fork” is simply the same project in your own namespace, allowing you to make changes to a project publicly as a way to contribute in a more open manner.</p>
</div>
</td>
</tr>
</tbody></table>
</div>
<div class="paragraph">
<p>This way, projects don’t have to worry about adding users as collaborators to give them push access.
People can fork a project, push to it, and contribute their changes back to the original repository by creating what’s called a Pull Request, which we’ll cover next.
This opens up a discussion thread with code review, and the owner and the contributor can then communicate about the change until the owner is happy with it, at which point the owner can merge it in.</p>
</div>
<div class="paragraph">
<p>To fork a project, visit the project page and click the “Fork” button at the top-right of the page.</p>
</div>
<div class="imageblock">
<div class="content">
<img src="/book/sv/v2/images/forkbutton.png" alt="The ``Fork'' button.">
</div>
<div class="title">Figur 89. The “Fork” button.</div>
</div>
<div class="paragraph">
<p>After a few seconds, you’ll be taken to your new project page, with your own writeable copy of the code.</p>
</div>
</div>
<div class="sect3">
<h3 id="ch06-github_flow">The GitHub Flow</h3>
<div class="paragraph">
<p>
GitHub is designed around a particular collaboration workflow, centered on Pull Requests.
This flow works whether you’re collaborating with a tightly-knit team in a single shared repository, or a globally-distributed company or network of strangers contributing to a project through dozens of forks.
It is centered on the <a href="/book/sv/v2/ch00/_topic_branch">Ämnesgrenar</a> workflow covered in <a href="/book/sv/v2/ch00/ch03-git-branching">Git förgreningar</a>.</p>
</div>
<div class="paragraph">
<p>Here’s how it generally works:</p>
</div>
<div class="olist arabic">
<ol class="arabic">
<li>
<p>Fork the project</p>
</li>
<li>
<p>Create a topic branch from <code>master</code>.</p>
</li>
<li>
<p>Make some commits to improve the project.</p>
</li>
<li>
<p>Push this branch to your GitHub project.</p>
</li>
<li>
<p>Open a Pull Request on GitHub.</p>
</li>
<li>
<p>Discuss, and optionally continue committing.</p>
</li>
<li>
<p>The project owner merges or closes the Pull Request.</p>
</li>
</ol>
</div>
<div class="paragraph">
<p>This is basically the Integration Manager workflow covered in <a href="/book/sv/v2/ch00/_integration_manager">Integrationsstyrd arbetsprocess</a>, but instead of using email to communicate and review changes, teams use GitHub’s web based tools.</p>
</div>
<div class="paragraph">
<p>Let’s walk through an example of proposing a change to an open source project hosted on GitHub using this flow.</p>
</div>
<div class="sect4">
<h4 id="_creating_a_pull_request">Creating a Pull Request</h4>
<div class="paragraph">
<p>Tony is looking for code to run on his Arduino programmable microcontroller and has found a great program file on GitHub at <a href="https://github.com/schacon/blink" class="bare">https://github.com/schacon/blink</a>.</p>
</div>
<div class="imageblock">
<div class="content">
<img src="/book/sv/v2/images/blink-01-start.png" alt="The project we want to contribute to.">
</div>
<div class="title">Figur 90. The project we want to contribute to.</div>
</div>
<div class="paragraph">
<p>The only problem is that the blinking rate is too fast. We think it’s much nicer to wait 3 seconds instead of 1 in between each state change.
So let’s improve the program and submit it back to the project as a proposed change.</p>
</div>
<div class="paragraph">
<p>First, we click the <em>Fork</em> button as mentioned earlier to get our own copy of the project.
Our user name here is “tonychacon” so our copy of this project is at <code>https://github.com/tonychacon/blink</code> and that’s where we can edit it.
We will clone it locally, create a topic branch, make the code change and finally push that change back up to GitHub.</p>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlight"><code class="language-console" data-lang="console">$ git clone https://github.com/tonychacon/blink <b class="conum">(1)</b>
Cloning into 'blink'...

$ cd blink
$ git checkout -b slow-blink <b class="conum">(2)</b>
Switched to a new branch 'slow-blink'

$ sed -i '' 's/1000/3000/' blink.ino (macOS) <b class="conum">(3)</b>
# If you're on a Linux system, do this instead:
# $ sed -i 's/1000/3000/' blink.ino <b class="conum">(3)</b>

$ git diff --word-diff <b class="conum">(4)</b>
diff --git a/blink.ino b/blink.ino
index 15b9911..a6cc5a5 100644
--- a/blink.ino
+++ b/blink.ino
@@ -18,7 +18,7 @@ void setup() {
// the loop routine runs over and over again forever:
void loop() {
  digitalWrite(led, HIGH);   // turn the LED on (HIGH is the voltage level)
  [-delay(1000);-]{+delay(3000);+}               // wait for a second
  digitalWrite(led, LOW);    // turn the LED off by making the voltage LOW
  [-delay(1000);-]{+delay(3000);+}               // wait for a second
}

$ git commit -a -m 'three seconds is better' <b class="conum">(5)</b>
[slow-blink 5ca509d] three seconds is better
 1 file changed, 2 insertions(+), 2 deletions(-)

$ git push origin slow-blink <b class="conum">(6)</b>
Username for 'https://github.com': tonychacon
Password for 'https://tonychacon@github.com':
Counting objects: 5, done.
Delta compression using up to 8 threads.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 340 bytes | 0 bytes/s, done.
Total 3 (delta 1), reused 0 (delta 0)
To https://github.com/tonychacon/blink
 * [new branch]      slow-blink -&gt; slow-blink</code></pre>
</div>
</div>
<div class="colist arabic">
<ol>
<li>
<p>Clone our fork of the project locally</p>
</li>
<li>
<p>Create a descriptive topic branch</p>
</li>
<li>
<p>Make our change to the code</p>
</li>
<li>
<p>Check that the change is good</p>
</li>
<li>
<p>Commit our change to the topic branch</p>
</li>
<li>
<p>Push our new topic branch back up to our GitHub fork</p>
</li>
</ol>
</div>
<div class="paragraph">
<p>Now if we go back to our fork on GitHub, we can see that GitHub noticed that we pushed a new topic branch up and presents us with a big green button to check out our changes and open a Pull Request to the original project.</p>
</div>
<div class="paragraph">
<p>You can alternatively go to the “Branches” page at <code>https://github.com/&lt;user&gt;/&lt;project&gt;/branches</code> to locate your branch and open a new Pull Request from there.</p>
</div>
<div class="imageblock">
<div class="content">
<img src="/book/sv/v2/images/blink-02-pr.png" alt="Pull Request button">
</div>
<div class="title">Figur 91. Pull Request button</div>
</div>
<div class="paragraph">
<p>
If we click that green button, we’ll see a screen that asks us to give our Pull Request a title and description.
It is almost always worthwhile to put some effort into this, since a good description helps the owner of the original project determine what you were trying to do, whether your proposed changes are correct, and whether accepting the changes would improve the original project.</p>
</div>
<div class="paragraph">
<p>We also see a list of the commits in our topic branch that are “ahead” of the <code>master</code> branch (in this case, just the one) and a unified diff of all the changes that will be made should this branch get merged by the project owner.</p>
</div>
<div class="imageblock">
<div class="content">
<img src="/book/sv/v2/images/blink-03-pull-request-open.png" alt="Pull Request creation">
</div>
<div class="title">Figur 92. Pull Request creation page</div>
</div>
<div class="paragraph">
<p>When you hit the <em>Create pull request</em> button on this screen, the owner of the project you forked will get a notification that someone is suggesting a change and will link to a page that has all of this information on it.</p>
</div>
<div class="admonitionblock note">
<table>
<tbody><tr>
<td class="icon">
<div class="title">Notera</div>
</td>
<td class="content">
<div class="paragraph">
<p>Though Pull Requests are used commonly for public projects like this when the contributor has a complete change ready to be made, it’s also often used in internal projects <em>at the beginning</em> of the development cycle. Since you can keep pushing to the topic branch even <strong>after</strong> the Pull Request is opened, it’s often opened early and used as a way to iterate on work as a team within a context, rather than opened at the very end of the process.</p>
</div>
</td>
</tr>
</tbody></table>
</div>
</div>
<div class="sect4">
<h4 id="_iterating_on_a_pull_request">Iterating on a Pull Request</h4>
<div class="paragraph">
<p>At this point, the project owner can look at the suggested change and merge it, reject it or comment on it. Let’s say that he likes the idea, but would prefer a slightly longer time for the light to be off than on.</p>
</div>
<div class="paragraph">
<p>Where this conversation may take place over email in the workflows presented in <a href="/book/sv/v2/ch00/ch05-distributed-git">Distribuerade Git</a>, on GitHub this happens online. The project owner can review the unified diff and leave a comment by clicking on any of the lines.</p>
</div>
<div class="imageblock">
<div class="content">
<img src="/book/sv/v2/images/blink-04-pr-comment.png" alt="PR line comment">
</div>
<div class="title">Figur 93. Comment on a specific line of code in a Pull Request</div>
</div>
<div class="paragraph">
<p>Once the maintainer makes this comment, the person who opened the Pull Request (and indeed, anyone else watching the repository) will get a notification. We’ll go over customizing this later, but if he had email notifications turned on, Tony would get an email like this:</p>
</div>
<div id="_email_notification" class="imageblock">
<div class="content">
<img src="/book/sv/v2/images/blink-04-email.png" alt="Email notification">
</div>
<div class="title">Figur 94. Comments sent as email notifications</div>
</div>
<div class="paragraph">
<p>Anyone can also leave general comments on the Pull Request. In <a href="/book/sv/v2/ch00/_pr_discussion">Pull Request discussion page</a> we can see an example of the project owner both commenting on a line of code and then leaving a general comment in the discussion section. You can see that the code comments are brought into the conversation as well.</p>
</div>
<div id="_pr_discussion" class="imageblock">
<div class="content">
<img src="/book/sv/v2/images/blink-05-general-comment.png" alt="PR discussion page">
</div>
<div class="title">Figur 95. Pull Request discussion page</div>
</div>
<div class="paragraph">
<p>Now the contributor can see what they need to do in order to get their change accepted.
Luckily this is very straightforward.
Where over email you may have to re-roll your series and resubmit it to the mailing list, with GitHub you simply commit to the topic branch again and push, which will automatically update the Pull Request.
In <a href="/book/sv/v2/ch00/_pr_final">Pull Request final</a> you can also see that the old code comment has been collapsed in the updated Pull Request, since it was made on a line that has since been changed.</p>
</div>
<div class="paragraph">
<p>Adding commits to an existing Pull Request doesn’t trigger a notification, so once Tony has pushed his corrections he decides to leave a comment to inform the project owner that he made the requested change.</p>
</div>
<div id="_pr_final" class="imageblock">
<div class="content">
<img src="/book/sv/v2/images/blink-06-final.png" alt="PR final">
</div>
<div class="title">Figur 96. Pull Request final</div>
</div>
<div class="paragraph">
<p>An interesting thing to notice is that if you click on the “Files Changed” tab on this Pull Request, you’ll get the “unified” diff — that is, the total aggregate difference that would be introduced to your main branch if this topic branch was merged in. In <code>git diff</code> terms, it basically automatically shows you <code>git diff master...&lt;branch&gt;</code> for the branch this Pull Request is based on. See <a href="/book/sv/v2/ch00/_what_is_introduced">Avgöra vad som ska integreras</a> for more about this type of diff.</p>
</div>
<div class="paragraph">
<p>The other thing you’ll notice is that GitHub checks to see if the Pull Request merges cleanly and provides a button to do the merge for you on the server. This button only shows up if you have write access to the repository and a trivial merge is possible. If you click it GitHub will perform a “non-fast-forward” merge, meaning that even if the merge <strong>could</strong> be a fast-forward, it will still create a merge commit.</p>
</div>
<div class="paragraph">
<p>If you would prefer, you can simply pull the branch down and merge it locally. If you merge this branch into the <code>master</code> branch and push it to GitHub, the Pull Request will automatically be closed.</p>
</div>
<div class="paragraph">
<p>This is the basic workflow that most GitHub projects use. Topic branches are created, Pull Requests are opened on them, a discussion ensues, possibly more work is done on the branch and eventually the request is either closed or merged.</p>
</div>
<div class="admonitionblock note">
<table>
<tbody><tr>
<td class="icon">
<div class="title">Notera</div>
</td>
<td class="content">
<div class="title">Not Only Forks</div>
<div class="paragraph">
<p>It’s important to note that you can also open a Pull Request between two branches in the same repository. If you’re working on a feature with someone and you both have write access to the project, you can push a topic branch to the repository and open a Pull Request on it to the <code>master</code> branch of that same project to initiate the code review and discussion process. No forking necessary.</p>
</div>
</td>
</tr>
</tbody></table>
</div>
</div>
</div>
<div class="sect3">
<h3 id="_advanced_pull_requests">Advanced Pull Requests</h3>
<div class="paragraph">
<p>Now that we’ve covered the basics of contributing to a project on GitHub, let’s cover a few interesting tips and tricks about Pull Requests so you can be more effective in using them.</p>
</div>
<div class="sect4">
<h4 id="_pull_requests_as_patches">Pull Requests as Patches</h4>
<div class="paragraph">
<p>It’s important to understand that many projects don’t really think of Pull Requests as queues of perfect patches that should apply cleanly in order, as most mailing list-based projects think of patch series contributions. Most GitHub projects think about Pull Request branches as iterative conversations around a proposed change, culminating in a unified diff that is applied by merging.</p>
</div>
<div class="paragraph">
<p>This is an important distinction, because generally the change is suggested before the code is thought to be perfect, which is far more rare with mailing list based patch series contributions. This enables an earlier conversation with the maintainers so that arriving at the proper solution is more of a community effort. When code is proposed with a Pull Request and the maintainers or community suggest a change, the patch series is generally not re-rolled, but instead the difference is pushed as a new commit to the branch, moving the conversation forward with the context of the previous work intact.</p>
</div>
<div class="paragraph">
<p>For instance, if you go back and look again at <a href="/book/sv/v2/ch00/_pr_final">Pull Request final</a>, you’ll notice that the contributor did not rebase his commit and send another Pull Request. Instead they added new commits and pushed them to the existing branch. This way if you go back and look at this Pull Request in the future, you can easily find all of the context of why decisions were made. Pushing the “Merge” button on the site purposefully creates a merge commit that references the Pull Request so that it’s easy to go back and research the original conversation if necessary.</p>
</div>
</div>
<div class="sect4">
<h4 id="_keeping_up_with_upstream">Keeping up with Upstream</h4>
<div class="paragraph">
<p>If your Pull Request becomes out of date or otherwise doesn’t merge cleanly, you will want to fix it so the maintainer can easily merge it. GitHub will test this for you and let you know at the bottom of every Pull Request if the merge is trivial or not.</p>
</div>
<div id="_pr_fail" class="imageblock">
<div class="content">
<img src="/book/sv/v2/images/pr-01-fail.png" alt="PR merge failure">
</div>
<div class="title">Figur 97. Pull Request does not merge cleanly</div>
</div>
<div class="paragraph">
<p>If you see something like <a href="/book/sv/v2/ch00/_pr_fail">Pull Request does not merge cleanly</a>, you’ll want to fix your branch so that it turns green and the maintainer doesn’t have to do extra work.</p>
</div>
<div class="paragraph">
<p>You have two main options in order to do this. You can either rebase your branch on top of whatever the target branch is (normally the <code>master</code> branch of the repository you forked), or you can merge the target branch into your branch.</p>
</div>
<div class="paragraph">
<p>Most developers on GitHub will choose to do the latter, for the same reasons we just went over in the previous section. What matters is the history and the final merge, so rebasing isn’t getting you much other than a slightly cleaner history and in return is <strong>far</strong> more difficult and error prone.</p>
</div>
<div class="paragraph">
<p>If you want to merge in the target branch to make your Pull Request mergeable, you would add the original repository as a new remote, fetch from it, merge the main branch of that repository into your topic branch, fix any issues and finally push it back up to the same branch you opened the Pull Request on.</p>
</div>
<div class="paragraph">
<p>For example, let’s say that in the “tonychacon” example we were using before, the original author made a change that would create a conflict in the Pull Request. Let’s go through those steps.</p>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlight"><code class="language-console" data-lang="console">$ git remote add upstream https://github.com/schacon/blink <b class="conum">(1)</b>

$ git fetch upstream <b class="conum">(2)</b>
remote: Counting objects: 3, done.
remote: Compressing objects: 100% (3/3), done.
Unpacking objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0)
From https://github.com/schacon/blink
 * [new branch]      master     -&gt; upstream/master

$ git merge upstream/master <b class="conum">(3)</b>
Auto-merging blink.ino
CONFLICT (content): Merge conflict in blink.ino
Automatic merge failed; fix conflicts and then commit the result.

$ vim blink.ino <b class="conum">(4)</b>
$ git add blink.ino
$ git commit
[slow-blink 3c8d735] Merge remote-tracking branch 'upstream/master' \
    into slower-blink

$ git push origin slow-blink <b class="conum">(5)</b>
Counting objects: 6, done.
Delta compression using up to 8 threads.
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 682 bytes | 0 bytes/s, done.
Total 6 (delta 2), reused 0 (delta 0)
To https://github.com/tonychacon/blink
   ef4725c..3c8d735  slower-blink -&gt; slow-blink</code></pre>
</div>
</div>
<div class="colist arabic">
<ol>
<li>
<p>Add the original repository as a remote named “upstream”</p>
</li>
<li>
<p>Fetch the newest work from that remote</p>
</li>
<li>
<p>Merge the main branch of that repository into your topic branch</p>
</li>
<li>
<p>Fix the conflict that occurred</p>
</li>
<li>
<p>Push back up to the same topic branch</p>
</li>
</ol>
</div>
<div class="paragraph">
<p>Once you do that, the Pull Request will be automatically updated and re-checked to see if it merges cleanly.</p>
</div>
<div id="_pr_merge_fix" class="imageblock">
<div class="content">
<img src="/book/sv/v2/images/pr-02-merge-fix.png" alt="PR fixed">
</div>
<div class="title">Figur 98. Pull Request now merges cleanly</div>
</div>
<div class="paragraph">
<p>One of the great things about Git is that you can do that continuously. If you have a very long-running project, you can easily merge from the target branch over and over again and only have to deal with conflicts that have arisen since the last time that you merged, making the process very manageable.</p>
</div>
<div class="paragraph">
<p>If you absolutely wish to rebase the branch to clean it up, you can certainly do so, but it is highly encouraged to not force push over the branch that the Pull Request is already opened on. If other people have pulled it down and done more work on it, you run into all of the issues outlined in <a href="/book/sv/v2/ch00/_rebase_peril">Farorna med grenflyttar</a>. Instead, push the rebased branch to a new branch on GitHub and open a brand new Pull Request referencing the old one, then close the original.</p>
</div>
</div>
<div class="sect4">
<h4 id="_references">References</h4>
<div class="paragraph">
<p>Your next question may be “How do I reference the old Pull Request?”. It turns out there are many, many ways to reference other things almost anywhere you can write in GitHub.</p>
</div>
<div class="paragraph">
<p>Let’s start with how to cross-reference another Pull Request or an Issue. All Pull Requests and Issues are assigned numbers and they are unique within the project. For example, you can’t have Pull Request #3 <em>and</em> Issue #3. If you want to reference any Pull Request or Issue from any other one, you can simply put <code>#&lt;num&gt;</code> in any comment or description. You can also be more specific if the Issue or Pull request lives somewhere else; write <code>username#&lt;num&gt;</code> if you’re referring to an Issue or Pull Request in a fork of the repository you’re in, or <code>username/repo#&lt;num&gt;</code> to reference something in another repository.</p>
</div>
<div class="paragraph">
<p>Let’s look at an example. Say we rebased the branch in the previous example, created a new pull request for it, and now we want to reference the old pull request from the new one. We also want to reference an issue in the fork of the repository and an issue in a completely different project. We can fill out the description just like <a href="/book/sv/v2/ch00/_pr_references">Cross references in a Pull Request.</a>.</p>
</div>
<div id="_pr_references" class="imageblock">
<div class="content">
<img src="/book/sv/v2/images/mentions-01-syntax.png" alt="PR references">
</div>
<div class="title">Figur 99. Cross references in a Pull Request.</div>
</div>
<div class="paragraph">
<p>When we submit this pull request, we’ll see all of that rendered like <a href="/book/sv/v2/ch00/_pr_references_render">Cross references rendered in a Pull Request.</a>.</p>
</div>
<div id="_pr_references_render" class="imageblock">
<div class="content">
<img src="/book/sv/v2/images/mentions-02-render.png" alt="PR references rendered">
</div>
<div class="title">Figur 100. Cross references rendered in a Pull Request.</div>
</div>
<div class="paragraph">
<p>Notice that the full GitHub URL we put in there was shortened to just the information needed.</p>
</div>
<div class="paragraph">
<p>Now if Tony goes back and closes out the original Pull Request, we can see that by mentioning it in the new one, GitHub has automatically created a trackback event in the Pull Request timeline. This means that anyone who visits this Pull Request and sees that it is closed can easily link back to the one that superseded it. The link will look something like <a href="/book/sv/v2/ch00/_pr_closed">Link back to the new Pull Request in the closed Pull Request timeline.</a>.</p>
</div>
<div id="_pr_closed" class="imageblock">
<div class="content">
<img src="/book/sv/v2/images/mentions-03-closed.png" alt="PR closed">
</div>
<div class="title">Figur 101. Link back to the new Pull Request in the closed Pull Request timeline.</div>
</div>
<div class="paragraph">
<p>In addition to issue numbers, you can also reference a specific commit by SHA-1. You have to specify a full 40 character SHA-1, but if GitHub sees that in a comment, it will link directly to the commit. Again, you can reference commits in forks or other repositories in the same way you did with issues.</p>
</div>
</div>
</div>
<div class="sect3">
<h3 id="_github_flavored_markdown">GitHub Flavored Markdown</h3>
<div class="paragraph">
<p>Linking to other Issues is just the beginning of interesting things you can do with almost any text box on GitHub. In  Issue and Pull Request descriptions, comments, code comments and more, you can use what is called “GitHub Flavored Markdown”. Markdown is like writing in plain text but which is rendered richly.</p>
</div>
<div class="paragraph">
<p>See <a href="/book/sv/v2/ch00/_example_markdown">An example of GitHub Flavored Markdown as written and as rendered.</a> for an example of how comments or text can be written and then rendered using Markdown.</p>
</div>
<div id="_example_markdown" class="imageblock">
<div class="content">
<img src="/book/sv/v2/images/markdown-01-example.png" alt="Example Markdown">
</div>
<div class="title">Figur 102. An example of GitHub Flavored Markdown as written and as rendered.</div>
</div>
<div class="paragraph">
<p>The GitHub flavor of Markdown adds more things you can do beyond the basic Markdown syntax. These can all be really useful when creating useful Pull Request or Issue comments or descriptions.</p>
</div>
<div class="sect4">
<h4 id="_task_lists">Task Lists</h4>
<div class="paragraph">
<p>The first really useful GitHub specific Markdown feature, especially for use in Pull Requests, is the Task List. A task list is a list of checkboxes of things you want to get done. Putting them into an Issue or Pull Request normally indicates things that you want to get done before you consider the item complete.</p>
</div>
<div class="paragraph">
<p>You can create a task list like this:</p>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlight"><code class="language-text" data-lang="text">- [X] Write the code
- [ ] Write all the tests
- [ ] Document the code</code></pre>
</div>
</div>
<div class="paragraph">
<p>If we include this in the description of our Pull Request or Issue, we’ll see it rendered like <a href="/book/sv/v2/ch00/_eg_task_lists">Task lists rendered in a Markdown comment.</a></p>
</div>
<div id="_eg_task_lists" class="imageblock">
<div class="content">
<img src="/book/sv/v2/images/markdown-02-tasks.png" alt="Example Task List">
</div>
<div class="title">Figur 103. Task lists rendered in a Markdown comment.</div>
</div>
<div class="paragraph">
<p>This is often used in Pull Requests to indicate what all you would like to get done on the branch before the Pull Request will be ready to merge. The really cool part is that you can simply click the checkboxes to update the comment — you don’t have to edit the Markdown directly to check tasks off.</p>
</div>
<div class="paragraph">
<p>What’s more, GitHub will look for task lists in your Issues and Pull Requests and show them as metadata on the pages that list them out. For example, if you have a Pull Request with tasks and you look at the overview page of all Pull Requests, you can see how far done it is. This helps people break down Pull Requests into subtasks and helps other people track the progress of the branch. You can see an example of this in <a href="/book/sv/v2/ch00/_task_list_progress">Task list summary in the Pull Request list.</a>.</p>
</div>
<div id="_task_list_progress" class="imageblock">
<div class="content">
<img src="/book/sv/v2/images/markdown-03-task-summary.png" alt="Example Task List">
</div>
<div class="title">Figur 104. Task list summary in the Pull Request list.</div>
</div>
<div class="paragraph">
<p>These are incredibly useful when you open a Pull Request early and use it to track your progress through the implementation of the feature.</p>
</div>
</div>
<div class="sect4">
<h4 id="_code_snippets">Code Snippets</h4>
<div class="paragraph">
<p>You can also add code snippets to comments. This is especially useful if you want to present something that you <em>could</em> try to do before actually implementing it as a commit on your branch. This is also often used to add example code of what is not working or what this Pull Request could implement.</p>
</div>
<div class="paragraph">
<p>To add a snippet of code you have to “fence” it in backticks.</p>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlight"><code class="language-text" data-lang="text">```java
for(int i=0 ; i &lt; 5 ; i++)
{
   System.out.println("i is : " + i);
}
```</code></pre>
</div>
</div>
<div class="paragraph">
<p>If you add a language name like we did there with <em>java</em>, GitHub will also try to syntax highlight the snippet. In the case of the above example, it would end up rendering like <a href="/book/sv/v2/ch00/_md_code">Rendered fenced code example.</a>.</p>
</div>
<div id="_md_code" class="imageblock">
<div class="content">
<img src="/book/sv/v2/images/markdown-04-fenced-code.png" alt="Rendered fenced code">
</div>
<div class="title">Figur 105. Rendered fenced code example.</div>
</div>
</div>
<div class="sect4">
<h4 id="_quoting">Quoting</h4>
<div class="paragraph">
<p>If you’re responding to a small part of a long comment, you can selectively quote out of the other comment by preceding the lines with the <code>&gt;</code> character. In fact, this is so common and so useful that there is a keyboard shortcut for it. If you highlight text in a comment that you want to directly reply to and hit the <code>r</code> key, it will quote that text in the comment box for you.</p>
</div>
<div class="paragraph">
<p>The quotes look something like this:</p>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlight"><code class="language-text" data-lang="text">&gt; Whether 'tis Nobler in the mind to suffer
&gt; The Slings and Arrows of outrageous Fortune,

How big are these slings and in particular, these arrows?</code></pre>
</div>
</div>
<div class="paragraph">
<p>Once rendered, the comment will look like <a href="/book/sv/v2/ch00/_md_quote">Rendered quoting example.</a>.</p>
</div>
<div id="_md_quote" class="imageblock">
<div class="content">
<img src="/book/sv/v2/images/markdown-05-quote.png" alt="Rendered quoting">
</div>
<div class="title">Figur 106. Rendered quoting example.</div>
</div>
</div>
<div class="sect4">
<h4 id="_emoji">Emoji</h4>
<div class="paragraph">
<p>Finally, you can also use emoji in your comments. This is actually used quite extensively in comments you see on many GitHub Issues and Pull Requests. There is even an emoji helper in GitHub. If you are typing a comment and you start with a <code>:</code> character, an autocompleter will help you find what you’re looking for.</p>
</div>
<div id="_md_emoji_auto" class="imageblock">
<div class="content">
<img src="/book/sv/v2/images/markdown-06-emoji-complete.png" alt="Emoji autocompleter">
</div>
<div class="title">Figur 107. Emoji autocompleter in action.</div>
</div>
<div class="paragraph">
<p>Emojis take the form of <code>:&lt;name&gt;:</code> anywhere in the comment. For instance, you could write something like this:</p>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlight"><code class="language-text" data-lang="text">I :eyes: that :bug: and I :cold_sweat:.

:trophy: for :microscope: it.

:+1: and :sparkles: on this :ship:, it's :fire::poop:!

:clap::tada::panda_face:</code></pre>
</div>
</div>
<div class="paragraph">
<p>When rendered, it would look something like <a href="/book/sv/v2/ch00/_md_emoji">Heavy emoji commenting.</a>.</p>
</div>
<div id="_md_emoji" class="imageblock">
<div class="content">
<img src="/book/sv/v2/images/markdown-07-emoji.png" alt="Emoji">
</div>
<div class="title">Figur 108. Heavy emoji commenting.</div>
</div>
<div class="paragraph">
<p>Not that this is incredibly useful, but it does add an element of fun and emotion to a medium that is otherwise hard to convey emotion in.</p>
</div>
<div class="admonitionblock note">
<table>
<tbody><tr>
<td class="icon">
<div class="title">Notera</div>
</td>
<td class="content">
<div class="paragraph">
<p>There are actually quite a number of web services that make use of emoji characters these days. A great cheat sheet to reference to find emoji that expresses what you want to say can be found at:</p>
</div>
<div class="paragraph">
<p><a href="http://www.emoji-cheat-sheet.com" class="bare">http://www.emoji-cheat-sheet.com</a></p>
</div>
</td>
</tr>
</tbody></table>
</div>
</div>
<div class="sect4">
<h4 id="_images">Images</h4>
<div class="paragraph">
<p>This isn’t technically GitHub Flavored Markdown, but it is incredibly useful. In addition to adding Markdown image links to comments, which can be difficult to find and embed URLs for, GitHub allows you to drag and drop images into text areas to embed them.</p>
</div>
<div id="_md_drag" class="imageblock">
<div class="content">
<img src="/book/sv/v2/images/markdown-08-drag-drop.png" alt="Drag and drop images">
</div>
<div class="title">Figur 109. Drag and drop images to upload them and auto-embed them.</div>
</div>
<div class="paragraph">
<p>If you look at <a href="/book/sv/v2/ch00/_md_drag">Drag and drop images to upload them and auto-embed them.</a>, you can see a small “Parsed as Markdown” hint above the text area. Clicking on that will give you a full cheat sheet of everything you can do with Markdown on GitHub.</p>
</div>
</div>
</div>
<div id="nav"><a href="/book/sv/v2/GitHub-Account-Setup-and-Configuration">prev</a> | <a href="/book/sv/v2/GitHub-Maintaining-a-Project">next</a></div>
            </div>
          </div>
          
        </div>
      </div>
      <footer>
  <div class="site-source">
    <a href="/site">About this site</a><br>
    Patches, suggestions, and comments are welcome.
  </div>
  <div class="sfc-member">
    Git is a member of <a href="/sfc">Software Freedom Conservancy</a>
  </div>
</footer>
<a href="#top" class="scrollToTop" id="scrollToTop" data-label="Scroll to top" style="display: inline;">
  <img src="/images/icons/chevron-up@2x.png" width="20" height="20" alt="scroll-to-top">
</a>

<script src="/js/jquery-1.7.1.min.js"></script>
<script src="/js/jquery-ui-1.8.18.custom.min.js"></script>
<script src="/js/jquery.defaultvalue.js"></script>
<script src="/js/session.min.js"></script>


<script src="/js/application.min.js"></script>

    </div>
  




</body>
