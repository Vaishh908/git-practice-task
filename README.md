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


<img width="1920" height="1080" alt="Screenshot 2026-06-04 125256" src="https://github.com/user-attachments/assets/da291b03-0892-42e5-8e34-ab288eb3e64a" />


## Task 5: Create Pull Request
Objective

Create Pull Request:

feature-A → main

Steps
Open GitHub.
Go to Pull Requests.

<img width="1920" height="1080" alt="Screenshot 2026-06-04 125416" src="https://github.com/user-attachments/assets/385f747c-b500-4972-96e6-651f6adc1576" />

Click New Pull Request.
Select:
Base: main
Compare: feature-A
Click Create Pull Request.

<img width="1517" height="765" alt="Screenshot 2026-06-04 125439" src="https://github.com/user-attachments/assets/8da79289-a059-47a5-b8c4-fd3b4ac69fe7" />


Result

Pull Request created successfully and left unmerged.

<img width="1498" height="765" alt="Screenshot 2026-06-04 125518" src="https://github.com/user-attachments/assets/d5021673-a8ac-4449-b6f1-7325d85e1e1c" />


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

<img width="1920" height="1080" alt="Screenshot 2026-06-04 125734" src="https://github.com/user-attachments/assets/f62ae2b8-a4b3-4cf2-93dc-9ec1e76fa1a6" />


Create Pull Request:

feature-B → main

<img width="1505" height="728" alt="Screenshot 2026-06-04 131102" src="https://github.com/user-attachments/assets/8b8a2aeb-9302-4a9c-9578-26e5131ff8a9" />

<img width="1480" height="783" alt="Screenshot 2026-06-04 131201" src="https://github.com/user-attachments/assets/b988f7d3-5c2e-41b3-8131-85905f695699" />

<img width="1521" height="728" alt="Screenshot 2026-06-04 131311" src="https://github.com/user-attachments/assets/05b10aa6-7f64-4685-80aa-d31d4f63c3f5" />


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

<img width="1477" height="760" alt="Screenshot 2026-06-04 130612" src="https://github.com/user-attachments/assets/c007299f-e64b-4cd2-b7ea-fba698a9e2e4" />

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

<img width="1495" height="776" alt="Screenshot 2026-06-04 131358" src="https://github.com/user-attachments/assets/6a5f8803-e308-4d73-b71f-592475770c10" />


<img width="1480" height="783" alt="Screenshot 2026-06-04 131201" src="https://github.com/user-attachments/assets/7c291db7-6042-47db-a82a-36734dc6f2b8" />


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

<img width="1920" height="1080" alt="Screenshot 2026-06-04 144851" src="https://github.com/user-attachments/assets/d85546d3-5178-4bb4-a3dd-ceb4ecc239fb" />


Clone:

git clone https://github.com/username/forked-repo.git

<img width="1920" height="1080" alt="Screenshot 2026-06-04 144914" src="https://github.com/user-attachments/assets/dca3e68d-bd10-464d-9aa2-0457d6af835a" />

Modify README.

Commit:

git add README.md

git commit -m "Updated README"

git push origin main

<img width="1920" height="1080" alt="Screenshot 2026-06-04 145735" src="https://github.com/user-attachments/assets/24f04969-4646-4aeb-a6d4-fe6aa1c94aeb" />


Create Pull Request to fork repository.

<img width="1507" height="742" alt="Screenshot 2026-06-04 150700" src="https://github.com/user-attachments/assets/7247df34-bf15-4290-9408-618c7a1bf1b0" />

<img width="1497" height="727" alt="Screenshot 2026-06-04 150716" src="https://github.com/user-attachments/assets/01781119-5700-4889-af7e-3640fc14f66b" />

<img width="1920" height="1080" alt="Screenshot 2026-06-04 150806" src="https://github.com/user-attachments/assets/b8b2cb92-d7ff-47c4-ab48-4b7e472ee72e" />

<img width="1517" height="677" alt="Screenshot 2026-06-04 151108" src="https://github.com/user-attachments/assets/c2f69bec-e0fc-4307-9459-46de44bbbc15" />

Result

Fork updated successfully.

## Task 11: GitLab Repository Setup
Objective

Create private GitLab repository.

<img width="1535" height="772" alt="Screenshot 2026-06-04 151339" src="https://github.com/user-attachments/assets/1cae2d2e-d0b5-4e2a-b914-434bde832f5a" />

Clone Using SSH
git clone git@gitlab.com:username/project.git

<img width="1523" height="732" alt="Screenshot 2026-06-04 151456" src="https://github.com/user-attachments/assets/1670aaef-3dac-4832-8e21-4b3d41e84772" />

<img width="1920" height="1080" alt="Screenshot 2026-06-04 153111" src="https://github.com/user-attachments/assets/0c810e9b-0925-4ef4-8520-2da491712f62" />

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

<img width="1920" height="1080" alt="Screenshot 2026-06-04 153121" src="https://github.com/user-attachments/assets/affd85ff-7f27-42ea-9471-97868672f05e" />

<img width="1520" height="761" alt="Screenshot 2026-06-04 154042" src="https://github.com/user-attachments/assets/22613b16-279a-485d-904b-9f7efa4dd972" />

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

<img width="1920" height="1080" alt="Screenshot 2026-06-05 124452" src="https://github.com/user-attachments/assets/48b6d772-f843-4955-aeb8-3b8e22a05a74" />


Authentication:

GitHub Username
Personal Access Token

Enable:

Push Mirroring
Verification


<img width="1920" height="1080" alt="Screenshot 2026-06-05 124546" src="https://github.com/user-attachments/assets/b664114f-ce8e-4fc8-9903-62073df1f2b5" />


<img width="1920" height="1080" alt="Screenshot 2026-06-05 124603" src="https://github.com/user-attachments/assets/470aef2a-7168-403e-9ca0-cc8150c40b16" />

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

<img width="1515" height="770" alt="Screenshot 2026-06-05 101430" src="https://github.com/user-attachments/assets/2be12f40-71fb-466f-96ab-3d934d33a540" />


<img width="1920" height="1080" alt="Screenshot 2026-06-05 101943" src="https://github.com/user-attachments/assets/6150c0cb-10c4-4c4a-a4b4-f80d8ce343ae" />


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

