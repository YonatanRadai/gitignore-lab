this is a git ignore lab the task was: 

### Objective
In this lab, you will gain hands-on experience with `.gitignore` files to understand their purpose and learn how to effectively manage untracked files in your Git repositories.

### Overview
When working with Git, it’s important to prevent certain files from being tracked. These might include logs, temporary files, and files containing sensitive information. This lab will guide you through the process of setting up a project and configuring a `.gitignore` file to properly exclude these types of files.

### Scenario
You are tasked with setting up a new project that includes a variety of files, some of which should not be included in the repository due to their nature (logs, temporary files, local configurations).

### Tasks

#### Task 1: Set Up the Repository
1. Create a new directory called `ignore-lab`.
2. Navigate into `ignore-lab`.
3. Initialize a new Git repository.
4. Create the following files:
   - `index.html`
   - `app.js`
   - `style.css`
   - `config.json` (contains sensitive configuration details)
   - `debug.log` (a log file generated by the application)

#### Task 2: Observe Untracked Files
1. Run `git status` to view the untracked files in your repository.
2. Note that all files, including temporary or sensitive files, are listed.

#### Task 3: Create a .gitignore File
1. Create a `.gitignore` file in the repository.
2. Add rules to ignore:
   - All `.log` files using the pattern `*.log`.
   - The `config.json` file.
   - Any file in a directory named `temp`.

#### Task 4: Test .gitignore
1. Verify that `debug.log` and `config.json` no longer appear as untracked files when running `git status`.
2. Create a file `temp/notes.txt` and ensure it is ignored by Git.

#### Task 5: Modify .gitignore
1. Add a rule to ignore all `.css` files using the pattern `*.css`.
2. Realize that `style.css` should be tracked and modify `.gitignore` to explicitly include `style.css` by adding `!style.css`.

#### Task 6: Advanced .gitignore Scenarios
1. Create a directory called `build` with some files inside it.
2. Ignore the entire `build` directory using `build/*`.
3. Add an exception to track `build/README.md` while ignoring the rest of the files in the `build` directory.

#### Task 7: Commit .gitignore
1. Add the `.gitignore` file to the staging area.
2. Commit the `.gitignore` file with a message that describes the changes made (e.g., "Add initial .gitignore rules").

### Submission Requirements
- The `.gitignore` file containing all the rules.
- The final output of `git status` showing the tracked and ignored files.
- A snapshot of the repository structure illustrating which files are ignored and which are tracked.

