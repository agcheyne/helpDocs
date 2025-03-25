Forking a Repository on GitHub
Go to the Repository:

Navigate to the GitHub repository you want to fork (e.g., https://github.com/user/repo).
Click on "Fork":

On the top right of the repository page, click the "Fork" button.

GitHub will create a copy of the repository under your account.

Clone the Forked Repository (Optional):
```bash
git clone https://github.com/your-username/repo.git
```

## Keeping Your Fork Updated (Optional)
If you want to sync your fork with the original repository:

Add the original repository as an upstream remote:

```bash
git remote add upstream https://github.com/original-user/repo.git
```
Fetch updates from upstream:

```bash
git fetch upstream
```

Merge changes into your local main branch:

```bash
git checkout main
git merge upstream/main
```

Push the updated code to your fork:

```bash
git push origin main
```
