# GithubAllGreen

**GitHub Contribution Green-Out Script
**
This Python script automates the creation of daily commits to "green out" your GitHub contribution calendar. The tool is designed for fun and demonstration purposes, allowing you to fill in your contribution graph for a specified date range with automated commits.

Disclaimer: While this script can create the desired visual effect on your GitHub profile, please remember that genuine, meaningful contributions are what truly matter in the open-source community. This tool is not intended to be a substitute for real development work.

**Features
**Automated Daily Commits: Creates a new commit for each day in a user-defined date range.

Backdating: Uses the --date flag to ensure commits appear on the correct day, allowing you to fill in past dates.

Simple and Portable: A single Python script with no external dependencies beyond the standard library.

**Getting Started
**Prerequisites
Python: Ensure you have Python installed on your system.

Git: You must have Git installed and configured.

A GitHub Repository: You need a repository that you can clone locally. This is the repository where the commits will be pushed.

**Usage
**Clone the Repository:
First, clone the target repository to your local machine.

git clone [https://github.com/chipmoreno/GithubAllGreen](https://github.com/chipmoreno/GithubAllGreen)

**Navigate to the Script:
**Place the github_green.py script in a convenient location, or directly inside the cloned repository's folder.

**Modify the Script:
**Open the github_green.py file and edit the variables within the if __name__ == "__main__": block.

repo_directory = "/path/to/your/local/GithubAllGreen" # Replace with the actual path to your cloned repository
start_date = "2025-01-01" # The start date for your commits
end_date = "2025-09-13"   # The end date for your commits

**Run the Script:
**Execute the script from your terminal.

python github_green.py

**Push the Commits:
**After the script finishes, your local repository will contain all the new commits. The final step is to push them to GitHub.

git push origin <your_branch_name>

Replace <your_branch_name> with the name of your branch (e.g., main or master). Once the push is complete, your contribution graph will update on GitHub.

**How it Works
**The script iterates through each day in the specified date range. For every day, it performs the following steps:

Creates a new, empty text file with a unique name based on the date.

Adds the new file to the Git staging area.

Commits the change, using the --date flag to set the commit timestamp to the current day in the loop.

This process creates a historical record of commits, which is then reflected in your GitHub contribution history once you push the changes.
