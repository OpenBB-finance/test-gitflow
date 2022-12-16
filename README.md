# GitFlow Repository

GitFlow is a branching model for Git that makes it easier for teams to collaborate on projects using the Git version control system. This guide explains how to implement GitFlow for an open source project.

## Steps

1. Create a new branch called `feature/<feature-name>` from the `develop` branch for each new feature that you want to add to the project. This is where you will do your work on the feature.
~~~
git checkout -b feature/<feature-name> develop
~~~
2. When you are ready to merge your feature into the `develop` branch, create a pull request and have it reviewed by other members of the team. Once the pull request has been reviewed and approved, you can merge it into the `develop` branch.

3. Repeat this process for each new feature that you want to add to the project.

4. When you are ready to create a new release, create a new branch called `release/<version-number>` from the `develop` branch. This is where the final testing and preparations for the release with be done.
~~~
git checkout -b release/<version-number> develop
~~~
5. When the release is ready, merge it into the `main` branch and create a new tag with the version number. This will be your new release.

6. Finally, merge the `release` branch back into the `develop` branch and delete the `release` branch. This ensures that the `develop` branch always contains the latest code for the next release.

7. When you are ready to create a new hotfix, create a new branch called `hotfix/<issue-fixed>` from the `main` branch. This is where the hotfix will be developed.
~~~
git checkout -b hotfix/<issue-fixed> main
~~~
8. When the hotfix is ready, create a PR to merge it into the `main` branch and create a new tag with the version number. This will be the new release.

9. Finally, merge the `hotfix` branch back into the `develop` branch and delete the `hotfix` branch. This ensures that the `develop` branch always contains the latest code for the next release.