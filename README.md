<img width="1183" height="712" alt="Screenshot 2025-09-26 140056" src="https://github.com/user-attachments/assets/92598726-e5f9-49a5-9d60-f6f88b9ac2df" />


<img width="1313" height="588" alt="Screenshot 2025-09-26 140135" src="https://github.com/user-attachments/assets/fc628dac-bc4c-4c53-b75f-5570e6195738" />


This project explains how to manage a DevOps project using **Git best practices**, including:

- Version control for code and documentation
- Branching strategies (`main`, `dev`, `feature/*`)
- Pull request workflow
- Proper documentation

1.First create a local git repository in a EC2 machine.Then create directory to add  neccessary files includes that directory.
And "Add" those files using git command  "git add ." to add all files in the local repo.
And Commit the changes using git command "git commit -m " some content added message ". Here "m" is a 

2.Branching Strategy
main → Production-ready code
dev → Development and integration branch
feature/* → Individual features or tasks

3.Push to GitHub
Add remote repository using:
git remote add origin https://github.com/<username>/devops-git-project.git

And then Push branches using git commands:
git push -u origin main
git push origin dev
git push origin feature/add-readme

4.Pull Request Workflow from github:
Open a Pull Request (PR) from feature/* → dev
Review and merge the PR
Merge dev branch into main branch for stable release
