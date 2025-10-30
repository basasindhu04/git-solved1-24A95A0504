#  My Git Mastery Challenge Journey


##  Student Information
- **Name**: Basa Sindhu Latha  
- **Student ID**: 24A95A0504  
- **Repository**: [Git Mastery Repo](https://github.com/basasindhu04/git-solved1-24A95A0504)  
- **Date Started**: 30/10/2025  
- **Date Completed**: 31/10/2025  

##  Task Summary
Cloned instructor's repository with pre-built conflicts and resolved all merge conflicts across multiple branches using proper Git workflows.

##  Commands Used

| Command        | Times Used | Purpose                                 |
|----------------|------------|-----------------------------------------|
| git clone      | 1          | Clone instructor's repository           |
| git checkout   | 20+        | Switch between branches                 |
| git branch     | 10+        | View and manage branches                |
| git merge      | 2          | Merge dev and conflict-simulator into main |
| git add        | 30+        | Stage resolved conflicts                |
| git commit     | 15+        | Commit resolved changes                 |
| git push       | 10+        | Push to my repository                   |
| git fetch      | 2          | Fetch updates from instructor           |
| git pull       | 1          | Pull updates                            |
| git stash      | 2          | Save temporary work                     |
| git cherry-pick| 1          | Copy specific commit                    |
| git rebase     | 1          | Rebase feature branch                   |
| git reset      | 3          | Undo commits (soft/mixed/hard)         |
| git revert     | 1          | Safe undo                               |
| git tag        | 2          | Create release tags                     |
| git status     | 50+        | Check repository state                  |
| git log        | 30+        | View history                            |
| git diff       | 20+        | Compare changes                         |

##  Conflicts Resolved

###  Merge 1: `main` + `dev` (6 files)

#### Conflict 1: `config/app-config.yaml`
- **Issue**: Production used port 8080, development used 3000  
- **Resolution**: Created unified config with environment-based settings  
- **Strategy**: Keep production as default, add dev as optional  
- **Difficulty**: Medium  
- **Time**: 15 minutes  

#### Conflict 2: `config/database-config.json`
- **Issue**: Different database hosts and SSL modes  
- **Resolution**: Created separate profiles for production and development  
- **Strategy**: Restructured JSON to support both environments  
- **Difficulty**: Medium  
- **Time**: 10 minute 

#### Conflict 3: `scripts/deploy.sh`
- **Issue**: Different deployment strategies (production vs docker-compose)  
- **Resolution**: Added conditional logic based on DEPLOY_ENV variable  
- **Strategy**: Made script handle both environments dynamically  
- **Difficulty**: Hard  
- **Time**: 20 minutes  

#### Conflict 4: `scripts/monitor.js`
- **Issue**: Different monitoring intervals and log formats  
- **Resolution**: Environment-based configuration object  
- **Strategy**: Used process.env.NODE_ENV to determine behavior  
- **Difficulty**: Medium  
- **Time**: 15 minutes  

#### Conflict 5: `docs/architecture.md`
- **Issue**: Different architectural descriptions  
- **Resolution**: Merged both descriptions into comprehensive document  
- **Strategy**: Created sections for each environment  
- **Difficulty**: Easy  
- **Time**: 10 minutes  

#### Conflict 6: `README.md`
- **Issue**: Different feature lists and version numbers  
- **Resolution**: Combined all features with clear environment labels  
- **Strategy**: Organized features by category  
- **Difficulty**: Easy  
- **Time**: 10 minutes  

### Merge 2: `main` + `conflict-simulator` (6 files)

#### Conflict 1: `src/auth.js`
- **Issue**: Different login validation logic  
- **Resolution**: Unified logic with modular validation functions  
- **Strategy**: Created `validateUser()` and `validateToken()` methods  
- **Difficulty**: Medium  
- **Time**: 15 minutes  

#### Conflict 2: `src/api.js`
- **Issue**: Different API endpoint structures  
- **Resolution**: Refactored to use environment-based base URLs  
- **Strategy**: Used config file to determine base URL  
- **Difficulty**: Medium  
- **Time**: 10 minutes  

#### Conflict 3: `src/logger.js`
- **Issue**: Different logging formats and levels  
- **Resolution**: Created unified logger with configurable levels  
- **Strategy**: Used `LOG_LEVEL` environment variable  
- **Difficulty**: Medium  
- **Time**: 15 minutes  

#### Conflict 4: `tests/test-auth.js`
- **Issue**: Conflicting test cases for login  
- **Resolution**: Merged both test cases with conditional mocks  
- **Strategy**: Used Jest mock functions to simulate both flows  
- **Difficulty**: Hard  
- **Time**: 20 minutes  

#### Conflict 5: `docs/conflict-resolution.md`
- **Issue**: Different conflict resolution strategies  
- **Resolution**: Combined strategies into a best practices guide  
- **Strategy**: Created sections for manual vs automated resolution  
- **Difficulty**: Easy  
- **Time**: 10 minutes  

#### Conflict 6: `README.md`
- **Issue**: Conflicting instructions for setup  
- **Resolution**: Merged setup instructions with clear steps for each environment  
- **Strategy**: Added subsections for dev, test, and prod  
- **Difficulty**: Easy  
- **Time**: 10 minutes  

## Most Challenging Parts
1. Understanding conflict markers (`<<<<<<<`, `=======`, `>>>>>>>`)  
2. Choosing between conflicting code  
3. Resolving complex logic conflicts (`deploy.sh`)  
4. Testing after resolution  

## Key Learnings

### Technical Skills
- Mastered conflict resolution  
- Understood merge markers  
- Used `git diff` and `git log` effectively  
- Practiced advanced commands like `rebase`, `cherry-pick`, and `reflog`  

### Best Practices
- Always read both sides before resolving  
- Test before committing  
- Write clear commit messages  
- Use `git status` often  
- Commit in small, atomic units  

### Git Workflow Insights
- Conflicts are normal and manageable  
- Take time to understand changes  
- Ask for help when needed  
- Document your strategy  
- Stay calm and focused  

## Reflection
This challenge transformed my view of Git. Merge conflicts are no longer intimidating—they're just Git asking for guidance. I now feel confident resolving conflicts in real-world projects. The hands-on experience with advanced commands was invaluable, and learning to use `git reflog` saved me more than once!