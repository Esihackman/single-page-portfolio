Git Commands Used
Below are the Git commands I used during the development of this single-page portfolio. I worked on separate feature branches for each section of the project. After finishing working on each  branch, I merged them into the main branch and then deleted the feature branches to keep the repository clean.

# Initialize the Git repository
# This command initializes a new Git repository in the project directory
git init

# Add initial project files
# Adds all files in the project to the staging area (preparing them for commit)
git add .

# Commit the changes
# Commits the added files with a message describing the initial structure of the project
git commit -m "created the project structure"

# ===== Header Section =====
# Create a new branch for the header section
# This allows us to work on the header feature separately from other parts of the project
git checkout -b header-section

# After working on the header section, add the changes
# Stage the changes so they are ready to be committed
git add .

# Commit the changes for the header section
# This saves the progress made in the header section with a descriptive commit message
git commit -m "created and styled the header-section"

# ===== About Me Section =====
# Create a new branch for the About Me section
git checkout -b about-me

# After working on the About Me section, add the changes
git add .

# Commit the changes for the About Me section
git commit -m "structured and styled the about me and my work section"

# ===== Contact Section =====
# Create a new branch for the contact section
git checkout -b contact-section

# After working on the contact section, add the changes
git add .

# Commit the changes for the contact section
git commit -m "Created the call to action container  "

# ===== Merging Finished Branches =====
# Switch to the main branch before merging the feature branches
git checkout main

# Merge the header-section branch into the main branch
git merge header-section

# Merge the about-me branch into the main branch
git merge about-me

# Merge the contact-section branch into the main branch
git merge contact-section

# ===== Deleting Merged Branches =====
# After successfully merging, delete the feature branches locally to keep the repository clean
git branch -d header-section
git branch -d about-me
git branch -d contact-section

# ===== Connect to GitHub and Push =====
# Add the remote repository URL (replace with your own GitHub repository)
git remote add origin https://github.com/Esihackman/portfolio-project.git

# Push the changes to the main branch on GitHub
git push -u origin main
 