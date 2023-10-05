# Git Demo How to use git command 
Flow:
- Developer create feature branch from dev branch for develop feature code
- After develop from feature branch finish , Developer will merge feature branch to dev branch
- Source code in dev branch will deploy application by pipeline to dev environment for testing
- And when need to deploy application to sit environment, Deveoper will merger dev branch to main branch and tag version at main branch
- Source code that tag version will deploy application by pipeline to sit environment for testing

# Clone Initial code 
for start develop new application, clone source code from repository

```
git clone xxxx.git
```

# Create new branch (dev) if not exist
After clone source code, normally it will start from main or master branch. So first need to create dev branch before to not existing

```
git branch dev
```

# Checkout dev branch
Chenge working branch to dev  branch
```
git checkout dev
```

# Create branch feature from dev
Create feature base on dev branch for develop code 

```
git branch feature/test
```

# Check out feature branch
Change working branch to feature branch

```
git checkout feature/test
```

# Update code on feature branch after update finish
After devlope code finish in feature branch, push code back to feature branch on repository

```
git push
```

# Merge feature to dev
Update dev branch, merge feature branch to dev branch

```
git checkout dev 
git merge feature/test
git push
```

# Merge dev to main
If application on dev envrionment running ok and need to deploy to sit enviroment, merge dev branch to main branch

```
git checkout main
git merge dev
git push

```
