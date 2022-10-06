# Exercise 8 - Viewing changes before committing

1. Ensure your working directory is clean

2. Add text to any one of your files

3. Delete different text from another of your files

4. Look at `git status`

5. View all the changes you've made

        git diff

6. Does the following command return anything?

        git diff --staged

No.

7. Add one of your changed files to the index

        git commit add <changed file>

8. What do these commands show?

        git diff


diff --git a/appliances.txt b/appliances.txt
index 6e517e6..6a71e90 100644
--- a/appliances.txt
+++ b/appliances.txt
@@ -3,4 +3,4 @@ toaster
 microwave
 dryer
 sink
-oven
\ No newline at end of file
+vaccum
\ No newline at end of file

        git diff --staged


diff --git a/equipment.txt b/equipment.txt
index 5dadb08..83006eb 100644
--- a/equipment.txt
+++ b/equipment.txt
@@ -1,5 +1,4 @@
 axe
 saw
 drill
-shovel
-wrench
\ No newline at end of file
+shovel
\ No newline at end of file

9. Add the other changed file to the index

        git commit add <other changed file>

10. What do these commands show?

        git diff

        Nothing

        git diff --staged

diff --git a/appliances.txt b/appliances.txt
index 6e517e6..6a71e90 100644
--- a/appliances.txt
+++ b/appliances.txt
@@ -3,4 +3,4 @@ toaster
 microwave
 dryer
 sink
-oven
\ No newline at end of file
+vaccum
\ No newline at end of file
diff --git a/equipment.txt b/equipment.txt
index 5dadb08..83006eb 100644
--- a/equipment.txt
+++ b/equipment.txt
@@ -1,5 +1,4 @@
 axe
 saw
 drill
-shovel
-wrench
\ No newline at end of file
+shovel
\ No newline at end of file


11. Commit the changes

12. Check that your working directory is clean

13. Create a new file named `clothing.txt`

14. Does the new untracked file show up in git diff?

        git diff

It does not


15. Add and commit the new file
