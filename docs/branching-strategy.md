In this repo we work on a three branches they are master,dev,feature branches.

MAIN Branch(master)
1.The  master branch is the main branch were our code is fully Stable, production-ready code.
2.Only all merges fully tested from the other branches and reviewed features into Main.
3. All releases are tagged from this branch.

Development Branch (`dev`)
1.We can use this branch as Integration branch for ongoing development not distubing the main code.
2.All feature branches are merged here first.
3.Provides a staging area before merging into `main`.

**2. Branch Workflow**

1. Create a feature branch from `dev`:

git checkout dev
git checkout -b feature/add-readme

Work on the feature and commit changes:
git add README.md
git commit -m "Add project description to README"

Push feature branch to GitHub:
git push origin feature/add-readme

Open a Pull Request (PR) from feature/add-readme → dev:
Review changes.
Merge into dev after approval.

Merge dev into main for stable release:
git checkout main
git merge dev
git push origin main

From this Branching stratagies are the key to work for every individuals to work on specific tasks with out disturbing original content of the main branch.

