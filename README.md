## How to Contribute

Follow these steps:

1. **Clone the Repository**
   First, clone the repository to your local machine and navigate to the project folder using the following commands:

   ```bash
   git clone https://github.com/MehdiBouchachi/dantcare-web.git
   cd dantcare-web
   ```

2. **Create a New Branch**
   Always work on a separate branch for new features or bug fixes:

   ```bash
   git checkout -b feature/new-feature-name
   ```

3. **Make Your Changes**
   Implement your changes and make sure to test them locally.

4. **Commit Your Changes**
   Once you’re done, commit your changes with a meaningful message:

   ```bash
   git add .
   git commit -m "New feature added"
   ```

5. **Pull the Latest Changes**
   Pull the latest changes from the main branch to avoid conflicts:

   ```bash
   git checkout master
   git pull origin master
   git checkout feature/new-feature-name
   git rebase master
   ```

   Rebasing rewrites your branch history to incorporate the latest changes from main without creating merge commits. If there are conflicts, Git will pause the rebase and prompt you to resolve them.

   After resolving any conflicts, continue the rebase:

   ```bash
   git rebase --continue
   ```

6. **Push to Your Branch**
   Push your changes to your feature branch:

   ```bash
   git push origin feature/new-feature-name
   ```

7. **Create a Pull Request**
   In Github open a Pull Request (PR) from your branch to the main branch. Be sure to include a description of your changes and link any related issues.

8. **Wait for Review**
   After submitting the PR, your code will be reviewed. Address any feedback, if necessary, and push changes to the same branch.

9. **Merge After Approval**
   Once the PR is approved, merge it into main branche using Github or by these commandes:

   ```bash
   git checkout master
   git merge feature/new-feature-name
   ```

10. **Clean Up**
    After merging, delete the feature branch locally and remotely:

    ```bash
    git branch -d feature/new-feature-name
    git push origin --delete feature/new-feature-name
    ```
