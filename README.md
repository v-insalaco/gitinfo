# Git Repository Info Sheet

This readme will help you push a repository to your online Github Repository.

### 1. Create & Activate Virtual Environment

Run `py -3.10 -m venv .[venvname]`; venvname being your choice of environment name, and here we're specifying the Python version to work with Azure.

If you've already files in your folder, make sure your `.gitignore` file is ignoring the .venvname for all the dependency files, and .env if you're using credentials.

Run `.[venvname]\Scripts\activate`, venvname being your choice of environment name.

### 2. Configure Git

run `git config --global user.name "My name"`

run `git config --global user.email "@gmail.com"`

### 3. Initiate and ready Git

run `git init` to start git on your terminal.

Make sure your `.gitignore` file is ignoring the .venvname for all the dependency files, and .env if you're using credentials.

run `git add .` to add your repository to the update queue.

### 4. Inital Commit and Remote URL adding

Run `git commit -m "Initial commit message"` to get your repository ready.

Create a Git repository on Github.com

run `git remote add origin YOUR_REPOSITORY_URL`, with YOUR_REPOSITORY_URL defined.

<details markdown="1">
  <summary>Changing the URL</summary>
  run `git remote set-url origin YOUR_REPOSITORY_URL` if you want to change the URL.
</details>

### 5. Push your Git Repository

For your first time, run `git push -u origin master`, where master is the channel name you're pushing to.

## Git Repository Updated!

<details markdown="1">
  <summary>Subsequent Submissions</summary>
  
If you've not restarted you virtual environment:

Run `python -m venv .[venvname]`; venvname being your choice of environment name.

Run `.[venvname]\Scripts\activate`, venvname being your choice of environment name to activate it.

With your virtual environment running:

run `git init`

run `git add .`

run `git commit -m "Message to document changes made"`

run `git push -u origin master` to push the first time of the session.

run `git push` subsequently.

Or run `git push origin master --force` if you want to overwrite the remote repository completely.
</details>
