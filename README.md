
# Project_name





## Installation

Follow the steps below to correctly install and start this project:

1. Note that the main branch for development is the **dev-main** branch. This branch holds the latest code and it serves as the main reference when starting a new task.

2. Clone the repository: Repo_name

```bash
  git clone repo_origin
```

3. Ensure you are on the **dev-main** branch before installing the node modules.

```bash
  git checkout dev-main
```

4. Install the required packages using NPM.

```bash
  npm install --force
```

5. Start the project and explore the codebase.

```bash
  npm start
```
    
## Branches

#### "dev-main" Branch (Testing Environment)
- This is the main branch and it also serves as the official testing environment for the app.
- All completed tasks are merged to the **dev-main** branch after completion and approval.
- The **dev-main** branch is deployed to a certain link for testing.

#### "beta-version-1.1" Branch (Production Environment)
- This is the production branch 
- Only the **dev-main** branch can be merged to this branch
- Random pull requests should not be made to this branch

#### How to name a branch
- **feature/branchName** : To build a new feature
- **fix/fixName**: To quickly solve a bug
- **version/versionName**: To create a new parent branch

Note: Please do not delete general branches, you are only allowed to delete branches you create, if required.

## Starting a New Task

Follow the steps below to start a new task from scratch:

1. Move to the **dev-main** branch.

```bash
  git checkout dev-main
```

2. Pull the latest code from the **dev-main** branch.

```bash
  git pull origin dev-main
```

3. Create a new branch for your task. (Refer to the section above on how to correctly name a branch)
```bash
  git branch feature/taskName
```

4. Move into the created branch and start the task.
```bash
  git checkout feature/taskName

  npm start
```
## Continuing a Task

If you have an ongoing task and want to continue working on the branch, ensure you follow the steps below:

1. Stage the latest changes in your branch and commit the code.

```bash
  git add .
  
  git commit -m "commit message"
```

2. Move to the **dev-main** branch to pull the latest code.

```bash
  git checkout dev-main

  git pull origin dev-main
```

3. Move to your task branch and merge the **dev-main** code to it.

```bash
  git checkout feature/taskName

  git merge dev-main
```

4. Resolve all merge conflicts if any and don't hesitate to ask for help.
## Finishing a Task (Creating Pull Request)

When you have tested and completed an approved task, the next step is to create a pull request to a parent branch (mostly the **dev-main** branch) for testing. Follow the steps below to correctly create a PR:

1. Push your completed code the task branch

```bash
  git add .

  git commit -m "last commit message"

  git push origin feature/taskName
```

2. Ensure you have the latest dev-main code merged to your task branch. To confirm, move to the **dev-main** branch and pull the latest code.

```bash
  git checkout dev-main

  git pull origin dev-main
```

3. Move to back to the task branch to merge the **dev-main** code, if any.

```bash
  git checkout feature/taskName

  git merge dev-main
```

4. Resolve merge conflicts and push the merged code to the task branch.

5. On Github, create a **Pull Request (PR)** by pointing the task branch to the parent branch (e.g. **dev-main**).

6. Ensure the PR has no conflicts with the parent branch.

Note: If you don't the required clearance to merge, kindly notify someone that does or tag the person as a reviewer. 
## Tech Stack

**Languages & Frameworks:** JavaScript, React, TypeScript etc

**Styling:** CSS, Styled Components, Material UI

**API Management**: GraphQL, Axios


## Links

- [Website URL]
- [Production URL]
- [Testing URL]
- [Figma Board URL]
- [Teamwork Project Management Tool URL]

