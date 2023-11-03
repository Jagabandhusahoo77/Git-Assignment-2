
# Devops Git Assignment Project

Creating git braches 
# 1. Create a Git working directory with feature1.txt and feature2.txt in the master branch

# Create a new directory for the Git repository
mkdir my-git-repo

# Navigate to the directory
cd my-git-repo

# Initialize a new Git repository
git init

# Create two files, feature1.txt and feature2.txt, with some content
echo "Feature 1 content" > feature1.txt
echo "Feature 2 content" > feature2.txt

# Add the two files to the staging area
git add feature1.txt feature2.txt

# Commit the staged files to the local repository
git commit -m "Added feature1 and feature2 files"

# 2. Create 3 branches develop, feature1 and feature2

# Create a new branch called develop
git checkout -b develop

# Create a new branch called feature1
git checkout -b feature1

# Create a new branch called feature2
git checkout -b feature2

# 3. In develop branch create develop.txt, do not stage or commit it

# Create a new file called develop.txt with some content
echo "Develop content" > develop.txt

# 4. Stash this file and check out to feature1 branch

# Stash the current state of the working tree and index
git stash

# Check out to the feature1 branch
git checkout feature1

# 5. Create new.txt file in feature1 branch, stage and commit this file

# Create a new file called new.txt with some content
echo "New content" > new.txt

# Add the new file to the staging area
git add new.txt

# Commit the staged files to the local repository
git commit -m "Added new file"

# 6. Checkout to develop, unstash this file and commit

# Check out to the develop branch
git checkout develop

# Unstash the most recently stashed state to the working tree and index
git stash pop

# Commit the develop.txt file to the local repository
git commit -m "Unstashed and committed develop.txt"
Once you have completed these steps, you will have three branches in your Git repository:

master - The main branch, which contains the initial commit with the feature1.txt and feature2.txt files.
develop - A branch for development work, which contains the develop.txt file.
feature1 - A branch for feature1 development, which contains the new.txt file.
You can now continue to work on each branch independently, and merge them together when you are ready to release a new version of your software.# Git-Assignment-2
