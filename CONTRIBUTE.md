
A simple guide on contributing.
It's recommended to use a git interface for the ease of your workflow.
https://github.com/apps/desktop
https://gitextensions.github.io/
## Step 1: Fork the Repository

1. **Navigate to the Repository:**
    - Go to the original repository: [https://github.com/husseinmuhaisen/appliedOS](https://github.com/husseinmuhaisen/appliedOS)
2. **Fork the Repository:**
    - Click the **"Fork"** button in the top-right corner of the page.
    - This creates a copy of the repository under your GitHub account.

## Step 2: Clone Your Forked Repository

1. **Copy the Repository URL:**
    - On your forked repository page, click the **"Code"** button.
    - Copy the URL (use HTTPS unless you have SSH keys set up).
2. **Clone to Your Local Machine:**
    - Open your terminal or command prompt.
    - Run:
```
git clone https://github.com/your-username/appliedOS.git
```

Replace `your-username` with your GitHub username.

3. **Navigate to the Repository Folder:**
```
cd appliedOS
```

## Step 3: Set Up the Upstream Remote
Connecting to the original repository allows you to pull in updates.

1. **Add Upstream Remote:**
```
git remote add upstream https://github.com/husseinmuhaisen/appliedOS.git
```
2. **Verify Remotes:**
```
git remote -v
```
You should see `origin` (your fork) and `upstream` (original repository).

## Step 4: Sync Your Fork (Optional but Recommended)

Before making changes, ensure your fork is up-to-date with the original repository.
1. **Fetch Upstream Changes:**
```
git fetch upstream
```
2. **Merge Upstream Changes:**
```
git checkout main git merge upstream/main
```
## Step 5: Create a New Branch

It's good practice to create a new branch for your changes.
1. **Create and Switch to a New Branch:**
```
git checkout -b yourname-notes-day1
```
Name the branch with your name.

## Step 6: Add Your Notes

1. **Navigate to the Appropriate Folder:**
```
cd Day1
```

2. **Add Your Markdown File:**
- Place your `.md` file into the `Day1` folder.
- If you're already in `appliedOS/Day1`, you can copy or create your file here.

3. **Return to Repository Root:**
```
cd ..
```
## Step 7: Commit Your Changes

1. **Stage Your Changes:**
```
git add Day1/yourname-notes-file.md
```

2. **Commit with a Descriptive Message:**
```
git commit -m "Add Day 1 notes by [Your Name]"
```

## Step 8: Push Changes to Your Fork
1. **Push Your Branch to GitHub:**
```
git push origin yourname-notes-day1
```

## Step 9: Create a Pull Request
**Go to Your Fork on GitHub:**
- Navigate to `https://github.com/your-username/appliedOS`

1. **Open the Pull Request:**
- You may see a prompt to **"Compare & pull request"**. If not:
	- Click on the **"Pull requests"** tab.
	- Click **"New pull request"**.

2. **Select the Base and Compare Branches:**
- **Base Repository:** `husseinmuhaisen/appliedOS`
- **Base Branch:** `main`
- **Head Repository:** Your fork (`your-username/appliedOS`)
- **Compare Branch:** The branch you created (`yourname-notes-day1`)

3. **Review Your Changes:**
- Ensure that only the intended files are included.

4. **Write a Descriptive Title and Comment:**
- **Title:** `Add Day 1 notes by [Your Name]`
- **Description:** Add any additional information or context.

5. **Create the Pull Request:**
- Click **"Create pull request"**.

## Step 10: Pull in Updates from Upstream (Optional)

To keep your fork in sync:

1. **Fetch and Merge Upstream Changes:**
```
git fetch upstream 
git checkout main 
git merge upstream/main
```
2. **Push Updates to Your Fork:**
```
git push origin main
```
