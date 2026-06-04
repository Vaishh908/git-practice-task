# Git & GitLab Practical Assignment

Name: Vaishnavi Jagtap

Batch: 3 Nov

Course: MCA

## Task 1: Create a GitHub Repository
Objective

Create a public GitHub repository named git-practice-task.

Steps Performed
Logged in to GitHub.
Clicked New Repository.

Repository Name:

git-practice-task
Selected:
Public Repository
Initialize with README
Clicked Create Repository.
Result

Repository created successfully.

<img width="1920" height="1080" alt="Screenshot 2026-06-04 121307" src="https://github.com/user-attachments/assets/4905b3e5-f84e-4d50-a69d-4c3dcc320e7f" />

## Task 2: Clone the Repository
Objective

Clone repository to local machine.

Commands
git clone https://github.com/username/git-practice-task.git

Move into project directory:

cd git-practice-task

Verify repository:

git status
Result

Repository cloned successfully.

On branch main
nothing to commit, working tree clean

<img width="1920" height="1080" alt="Screenshot 2026-06-04 124141" src="https://github.com/user-attachments/assets/62372c3c-358d-431e-bf0b-24bf2fba1d83" />


## Task 3: Initial Development on Main Branch
Objective

Update README file.

Added Content

git add README.md

git commit -m "Updated README with assignment details"

git push origin main
Result

Changes pushed successfully to GitHub.

<img width="1920" height="1080" alt="Screenshot 2026-06-04 124807" src="https://github.com/user-attachments/assets/d5d602fe-e6d1-48fd-b425-635e5fadb5a1" />

## Task 4: Create Feature-A Branch
Objective

Create branch feature-A and add index.html.

Create Branch
git checkout -b feature-A
Create index.html
<!DOCTYPE html>
<html>
<head>
    <title>Feature A</title>
</head>
<body>
    <h1>Feature A Page</h1>
</body>
</html>
Commit Changes
git add index.html

git commit -m "Added index.html in feature-A"

git push origin feature-A
Result

Feature-A branch successfully created and pushed.


## Task 5: Create Pull Request
Objective

Create Pull Request:

feature-A → main
Steps
Open GitHub.
Go to Pull Requests.
Click New Pull Request.
Select:
Base: main
Compare: feature-A
Click Create Pull Request.
Result

Pull Request created successfully and left unmerged.

## Task 6: Create Feature-B Branch
Objective

Create another branch named feature-B.

Commands
git checkout main

git checkout -b feature-B

Modify same lines in index.html:

<!DOCTYPE html>
<html>
<head>
    <title>Feature B</title>
</head>
<body>
    <h1>Feature B Page</h1>
</body>
</html>

Commit:

git add index.html

git commit -m "Modified index.html in feature-B"

git push origin feature-B

Create Pull Request:

feature-B → main
Result

Feature-B branch and PR created successfully.

## Task 7: Merge Feature-A
Objective

Merge Feature-A into Main Branch.

Steps

Open Pull Request:

feature-A → main

Click:

Merge Pull Request
Confirm Merge

Update local repository:

git checkout main

git pull origin main
Verification
cat index.html

Output:

<h1>Feature A Page</h1>
Result

Feature-A merged successfully.

## Task 8: Handle Merge Conflict
Objective

Resolve merge conflict caused by Feature-B.

Attempt Merge

GitHub shows:

This branch has conflicts that must be resolved
Pull Latest Changes
git checkout feature-B

git pull origin main

Conflict Example

<<<<<<< HEAD
<h1>Feature B Page</h1>
=======
<h1>Feature A Page</h1>
>>>>>>> main

Resolve Conflict

<!DOCTYPE html>
<html>
<head>
    <title>Feature A & B</title>
</head>
<body>
    <h1>Feature A Page</h1>
    <h2>Feature B Page</h2>
</body>
</html>
Commit Resolution
git add index.html

git commit -m "Resolved merge conflict"

git push origin feature-B
Result

Merge conflict successfully resolved.

## Task 9: Complete Merge
Objective

Merge Feature-B Pull Request.

Steps

Open PR:

feature-B → main

Click:

Merge Pull Request
Verification
git checkout main

git pull origin main

Check file:

<h1>Feature A Page</h1>
<h2>Feature B Page</h2>
Result

Feature-B successfully merged.

## Task 10: Fork and Contribute
Objective

Fork any public GitHub repository.

Steps

Fork repository.

Clone:

git clone https://github.com/username/forked-repo.git

Modify README.

Commit:

git add README.md

git commit -m "Updated README"

git push origin main

Create Pull Request to fork repository.

Result

Fork updated successfully.

## Task 11: GitLab Repository Setup
Objective

Create private GitLab repository.

Clone Using SSH
git clone git@gitlab.com:username/project.git
Project Structure
project/
├── src/
│   └── app.py
├── docs/
│   └── guide.md
└── README.md
Create Structure
mkdir src docs

touch src/app.py
touch docs/guide.md
touch README.md
Commit and Push
git add .

git commit -m "Initial project structure"

git push origin main
Result

GitLab repository configured successfully.

## Task 12: Repository Mirroring
Objective

Mirror GitLab repository to GitHub.

Steps

GitLab:

Settings
→ Repository
→ Mirroring Repositories

Add:

GitHub Repository URL

Authentication:

GitHub Username
Personal Access Token

Enable:

Push Mirroring
Verification

Push a change:

git push origin main

Check GitHub repository.

Result

Changes automatically appeared in GitHub.

## Task 13: Branch Protection
Objective

Protect Main Branch.

GitHub Steps
Settings
→ Branches
→ Add Branch Rule

Rule:

Branch Name: main

Enable:

- Require Pull Request Reviews

- Restrict Direct Pushes

- Require Status Checks

Save Rule.

Verification

Attempt:

git push origin main

Output:

remote: Protected branch update failed
Result

Direct pushes blocked successfully.

## Task 14: Final Verification

Completed Items

- GitHub repository created

- Repository cloned locally

-  Feature branches created

- Pull Requests created

- Feature-A merged

- Merge conflict resolved

- Feature-B merged

- Fork created and updated

- GitLab repository configured

- Repository mirroring working

- Branch protection enabled

## Conclusion

Successfully completed all Git, GitHub, and GitLab practical tasks including repository creation, branching, commits, pushes, pull requests, merge requests, conflict resolution, and branch merging. The practical demonstrated collaborative software development workflows using version control systems.

