## Getting Started

### Step 1: Clone the Dev Branch
Clone the development branch of the repository using the following command:
```sh
git clone --branch dev https://github.com/VeriTrust/veritrust-backend.git
git clone --branch dev https://github.com/VeriTrust/veritrust-frontend.git
```

### Step 2: Pull the Latest Changes
After cloning, ensure your local repository is up to date:
```sh
git pull origin dev
```

### Step 3: Make Changes
Modify the necessary files according to your requirements.

### Step 4: Check the Status
Run the following command to check the status of your changes:
```sh
git status
```
- If changes appear in **red**, they are unstaged.

### Step 5: Stage the Changes
```sh
git add .
```

### Step 6: Verify Staging
Check the status again to ensure changes are staged:
```sh
git status
```
- If changes appear in **green**, they are staged.

### Step 7: Commit the Changes
Commit your changes using the following syntax:
```sh
git commit -m "<type>: <description>"
```
> **Note:** `<type>` should be lowercase to follow conventional commit standards.

#### Commit Message Format:
- **feat** → Introduces a new feature
- **fix** → Fixes a bug
- **docs** → Changes in documentation only

#### Example:
**Single-line commit:**
```sh
git commit -m "feat: added profile section"
```

**Multi-line commit with description:**
```sh
git commit -m "feat: added profile section

- increased font size
- made footer bigger
- etc etc"
```
Read more: [Conventional Commits](https://cheatsheets.zip/conventional-commits)

### Step 8: Push Changes to the Dev Branch
Before pushing your changes, ensure you have the latest updates to avoid conflicts:
```sh
git pull origin dev --rebase
```
Then, push your changes:
```sh
git push origin dev
```

## Miscellaneous Git Commands

### 1. Handling Merge Conflicts
If someone else has made changes to the same files, use:
```sh
git pull --rebase --autostash
```

### 2. Unstaging Files
If you mistakenly staged files with `git add .`, unstage them using:
```sh
git reset .
```

### 3. Reverting to the Last Commit
If you made too many incorrect changes and want to discard them:
```sh
git restore .
```
