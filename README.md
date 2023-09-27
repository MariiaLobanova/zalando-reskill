
**Lab Exercise: Git Merge, Stash, and Revert**

**Objective:**
The objective of this lab exercise is to familiarize learners with common Git operations such as merging branches, stashing changes, and reverting commits.

**Prerequisites:**
1. Basic understanding of Git and GitHub.
2. Git installed on your local machine.
3. A GitHub account (for remote repository hosting, if needed).

**Instructions:**

**Step 1: Clone the Repository**

1. Open your terminal or command prompt.

2. Clone the Git repository for this exercise (you can use your own repository if you prefer):

   ```bash
   git clone <repository-url>
   ```

**Step 2: Create a Feature Branch**

1. Change to the cloned repository directory.

   ```bash
   cd <repository-directory>
   ```

2. Create a new branch for a feature you want to work on:

   ```bash
   git checkout -b feature-branch
   ```

**Step 3: Make Changes and Commit**

1. Make some changes to a file in the repository (e.g., edit a text file or add a new one).

2. Commit your changes:

   ```bash
   git add .
   git commit -m "Add feature changes"
   ```

**Step 4: Stash Changes**

1. Create a new file in your working directory (e.g., `new-feature.js`).

2. Realize you need to switch to another branch but don't want to commit your changes yet. Stash the changes:

   ```bash
   git stash save "Stash feature changes"
   ```

**Step 5: Create and Merge a New Branch**

1. Create a new branch called `bug-fix`:

   ```bash
   git checkout -b bug-fix
   ```

2. Make a change in the same file you modified earlier.

3. Commit your changes:

   ```bash
   git add .
   git commit -m "Fix a bug"
   ```

4. Merge the `bug-fix` branch into the `feature-branch`:

   ```bash
   git checkout feature-branch
   git merge bug-fix
   ```

**Step 6: Revert a Commit**

1. Realize that the last commit you made on `feature-branch` introduced a bug. Revert the commit:

   ```bash
   git log
   git revert <commit-hash>
   ```

   Replace `<commit-hash>` with the actual hash of the commit you want to revert. 

**Step 7: Apply Stash**

1. Apply the stash you created earlier:

   ```bash
   git stash apply
   ```

**Step 8: Push Changes**

1. Push your changes to the remote repository if you have one:

   ```bash
   git push origin feature-branch
   ```

**Step 9: Cleanup (Optional)**

1. If you're done with the branches and want to clean up, you can delete the `bug-fix` branch:

   ```bash
   git branch -d bug-fix
   ```




----------------------------------
Week 01 - Lesson 02 - Homework 1

```
Task: Write a program that calculates the total cost of a customer’s order at 
a coffee shop.

Requirements:

The program should prompt the user to enter the quantity of each item they 
want to order.The program should then calculate the total cost of the order 
based on the following prices:

Coffee: €2.50 per cup
Tea: €1.50 per cup
Pastry: €3.00 per item

The program should display the total cost of the order to the user.

Hints:
Use variables to store the quantity of each item ordered.
Use variables to store the price of each item.
Use arithmetic operators to calculate the total cost of the order.
Use Scanner class to read input from the user

```
