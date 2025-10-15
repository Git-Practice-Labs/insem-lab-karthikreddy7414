<img width="3200" height="1886" alt="image" src="https://github.com/user-attachments/assets/37017f14-7678-47dc-9d84-63d2293cbf59" /># Lab 01: Set up a Git repository with separate branches for frontend and backend, then merge them into the main branch.

## Objective
set up repository

## Tools / Technologies
List the tools and technologies required (e.g., Git, GitHub, Docker, Jenkins).

## Prerequisites
Describe any prerequisites (installed software, configured accounts, etc.).

## Steps / Commands
1. Step one — command(s) and explanation.
2. Step two — command(s) and explanation.
3. Continue with numbered steps to complete the lab.

## Expected Output / Result
Describe expected outputs, screenshots to capture, or verification steps.

## Deliverables (what to push)
- `Labs/Lab01_<ShortTitle>.md` (this file, completed)
- Any additional scripts, Dockerfiles, manifests, or screenshots placed in a folder named `Lab01_files/`

## Notes / Tips
- Add any helpful hints or troubleshooting tips here.
- Keep commands and outputs clear for grading.
- 
- solution: 
mkdir fullstack-project
cd fullstack-project
git init
echo "# Fullstack Project" > README.md
git add README.md
git commit -m "Initial commit"
git branch frontend
git branch backend
git checkout frontend
echo "<h1>Frontend</h1>" > index.html
git add .
git commit -m "Added frontend code"
git checkout backend
echo "print('Backend API running')" > app.py
git add .
git commit -m "Added backend code"
git checkout main
git merge frontend
git merge backend

