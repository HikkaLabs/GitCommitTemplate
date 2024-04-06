# Write Better Commit Messages in Git Using Commit Templates
![Git Logo](https://upload.wikimedia.org/wikipedia/commons/thumb/e/e0/Git-logo.svg/1280px-Git-logo.svg.png)
This repository provides a Git commit template to help standardize commit messages across projects. Clear and consistent commit messages are essential for understanding the history of a project and facilitating collaboration among team members. By following this template, you can ensure that your commit messages are informative and follow best practices.

Want to Appreciate our work 😁... Give our repo,  a Star⭐

## Requirements
- Git installed locally
- Basic Git Knowledge
- Fork the project (optional)

## Getting Started
First clone the project and place the git-commit-template.txt file in a preferred location.

Ex: `C:\Git\Shared\git-commit-template.txt`

### Rename the template (optional)
You can name your Git commit template file anything you like, but it's a good idea to choose a name that reflects its purpose. For example, you might name it something like `commit_template.txt` or `commit_template`.md.

The file extension for a Git commit template is not strictly defined, as Git itself does not enforce any specific file extension for commit templates. However, it's common to use .txt or .md (Markdown) extensions for readability and clarity.

## Configuring Git to Use the Commit Message Template
Once you have created your commit message template, you need to configure Git to use it by default. 

Follow these steps:

1. Open your terminal or command prompt.

2. Navigate to your Git repository using the cd command. ( Optional if setting up globally )

3. Run the following command to set the path to your commit message template.
    
    - To setup `local` project: 
    ```
    git config --local commit.template /path/to/git-commit-template.txt
    ``` 
    This setup the template to access only within the current project
    

    - To setup `globally`: 
    ```
    git config --global commit.template /path/to/git-commit-template.txt
    ```
    This setup the template to access globally which means by default this will be the default commit template with in your system.

    Above steps sets the commit.template configuration to the path of your git-commit-template file.

### Verifying the Configuration

Run following command to verify that the `commit.template` configuration has been set correctly

```
git config --local --get-all commit.template
```

You should see the path to your commit template file printed in the output.

Ex: `C:\Git\Shared\git-commit-template.txt`

### Writing Commit Messages Using the Template
Run the following command to create a new commit.

```
git commit
```

Git will automatically open your commit message template in your default text editor with the predefined structure.

`FYI` : 
- Lines stared with `#` will automatically ignored when you are saving the commit message.
- for the command `git commit -m "message"` the template is not useful at all. 


## Usage

### Fill in the Details:
Replace `[Type]` and `{Summary}` with appropriate values for your commit. Use the provided types (`Feat`, `Fix`, `Docs`, `Style`, `Refactor`, `Test`, `Chore`) to categorize your commit. Write a concise summary of your changes.

Add `Description` (Optional): Write a more detailed description of your changes below the summary, explaining what and why the changes were made. Follow the guidelines provided in the template for formatting and wrapping text.

Once you've filled in the template, commit your changes as usual.


## Commit Message Guidelines
- Separate Subject and Body: Begin your commit message with a clear and concise subject line, followed by a blank line before the description.
- Limit Subject Line Length: Keep the subject line under 50 characters to ensure readability.
- Use Imperative Mood: Write the subject line in the imperative mood (e.g., "Fix typo" rather than "Fixed typo").
- Wrap Body Text: Wrap the body of your commit message at 72 characters for better readability.
- Explain What and Why: Use the body of the commit message to explain what changes were made and why they were made, rather than how they were made.

### Types of Commits
- `Feat`: Introduce a new feature or functionality.
- `Fix`: Address a bug or issue.
- `Docs`: Make changes to documentation.
- `Style`: Update code style or formatting.
- `Refactor`: Refactor existing code without changing its external behavior.
- `Test`: Add or update tests.

## conclusion

In conclusion, using this Git commit template can make your commit messages clearer and more consistent. Clear commit messages help you and your team understand changes easily and maintain a clean codebase. Feel free to use this template in your projects, and if you have any questions or suggestions, we're here to help!

Designed & Developed by [HikkaLabs](HikkaLabs.com)

Happy Coding... ❤️😁

# About Hikka Labs
Hikka Labs is dedicated to providing innovative solutions to enhance development workflows and streamline project management. Our mission is to empower developers and teams to achieve their goals efficiently and effectively.

### Happy Coding ... ❤️🧑‍💻😁 