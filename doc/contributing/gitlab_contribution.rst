.. _gitlab_contribution:

Contributing on GitLab
======================

Reporting Issues or Ideas
-------------------------

If you encounter any bugs while using or contributing to this framework or have ideas for improvements and new features, create an issue on GitLab.

1. **Create a New Issue**

   - Provide a clear and descriptive title.
   - Include a detailed description of the current behavior and the expected behavior. If you have any implementation suggestions or screenshots, include them.
   - Use labels to categorize the issue (e.g., bug, feature, difficulty).
   - Assign the issue to yourself and/or relevant members.

Participating in Code Reviews
-----------------------------

Code reviews are essential for maintaining code quality, spotting any bugs early, and building a community. Here's how you can participate effectively:

**Review Code Changes**

   - Review open merge requests (MRs) regularly.
   - Provide constructive feedback on code quality, logic, and adherence to standards.
   - Address unresolved threads by sharing insights or seeking clarification.

Working on Issues
-----------------

When assigned or choosing to work on an issue, follow these steps to ensure smooth collaboration:

If there is an existing branch for the issue you want to work on already, skip the first step. 

1. **Create a New Branch**

   - Use GitLab's UI to create a new branch from the development branch. This ensures the automatic and consistent naming of branches. The name is related to the title of the corresponding issue. Hence, a clear title is important.
   - Ensure your branch name reflects the issue or feature you are addressing.


2. **Set Up Locally**

   - Clone the repository if you have not already: ``git clone <repository_url>``.
   - If your branch is not yet visible, run: ``git fetch``.
   - Your branch should now be visible, and you can switch to it using ``git checkout <branch-name>``, or you can use your IDE's UI.

   You are now ready to start implementing.

3. **Commit Changes**

   - Make your changes locally.
   - Stage changes for commit: ``git add <file or folder name>``.
   - Commit changes with a descriptive message: ``git commit -m "Your Description"``.

   Make sure to make small atomic commits so that it is easy to understand the commit history.

4. **Create a Merge Request**

   Once you have committed all your changes and your code is ready for review, you can create a merge request:

   - Push your branch to GitLab: ``git push origin <branch-name>`` or just ``git push origin`` if you are on the branch to be pushed already. 
   - Go to GitLab and navigate to the repository.
   - Create a new merge request targeting the **development** branch.
   - Provide a clear title and description summarizing your changes.
   - Assign relevant reviewers and add labels if necessary.


5. **Respond to Feedback**

   - Address feedback from reviewers promptly.
   - Revise your code, update documentation, or make necessary adjustments.
   - Engage in discussions to resolve any concerns or questions.

   Once all open threads have been resolved and the reviewer gives the approval, your changes will be merged.


By following these guidelines, you contribute effectively to the project, ensuring constructive communication, high-quality code, and collaborative teamwork.

