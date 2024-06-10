#### 1. **Create and Push `collab-dev` Branch**

Create a new branch named `collab-dev` from the `main` branch and push it to your fork (origin):

`git checkout -b collab-dev git push origin collab-dev`
#### 2. **Create Feature Branches from `collab-dev`**

For each feature or task, create a new branch from `collab-dev`:

`git checkout collab-dev git checkout -b feature-branch`
#### 3. **Make Changes and Commit**

Make changes in your feature branch, then stage and commit them:

`git add . git commit -m "Describe your changes"`

#### 4. **Push Feature Branch to Your Fork**

Push your feature branch to your fork (origin):

`git push origin feature-branch`

#### 5. **Create a Pull Request (PR) to `collab-dev` in Your Fork**

On GitHub:

- Navigate to your fork.
- Click the "Compare & pull request" button.
- Set the base branch to `collab-dev` and the compare branch to your feature branch.
- Create the pull request.

#### 6. **Request Feedback from Mentor**

Share the link to your pull request with your mentor to request a review and feedback.
#### 7. **Review and Merge PR**

After the PR is reviewed and approved, merge it into the `collab-dev` branch in your fork.

#### 8. **Sync Your Fork with Upstream**

Periodically, sync your fork with the upstream repository to keep it up to date:

`git fetch upstream git checkout main git merge upstream/main git push origin main`

#### 9. **Merge `main` into `collab-dev`**

Update `collab-dev` with the latest changes from `main`:

`git checkout collab-dev git merge main git push origin collab-dev`

#### 10. **Create a PR from Your `collab-dev` to Upstream's `main`**

Once your `collab-dev` branch in your fork is ready for integration into the upstream repository:

- Create a pull request from your fork's `collab-dev` branch to the `main` branch in the upstream repository.
- On GitHub, navigate to the upstream repository and click the "Compare & pull request" button.
- Set the base branch to `upstream/main` and the compare branch to `origin/collab-dev`.
- Create the pull request.