
The Gym@Kevin MINGW32 ~/Git-exercise (main|REBASE 1/2)
$ git rebase -i
fatal: It seems that there is already a rebase-merge directory, and
I wonder if you are in the middle of another rebase.  If that is the
case, please try
        git rebase (--continue | --abort | --skip)
If that is not the case, please
        rm -fr ".git/rebase-merge"
and run me again.  I am stopping in case you still have something    
valuable there.


The Gym@Kevin MINGW32 ~/Git-exercise (main|REBASE 1/2)
$ git reset --hard head~
HEAD is now at b03f09e chore: Create initial file

The Gym@Kevin MINGW32 ~/Git-exercise (main|REBASE 1/2)
$ git reset --hard head~2
HEAD is now at 3083f66 Update README

The Gym@Kevin MINGW32 ~/Git-exercise (main|REBASE 1/2)
$ git log
commit 3083f669516ea1396caaa74c8216de8cbe8236d3 (HEAD)
Author: Junior Hirwa <iamhirwejr@gmail.com>
Date:   Sat May 18 17:35:13 2024 +0200

    Update README

commit 826eba3e6add8872f92eb03855910bda3b8aadbf
Author: Junior Hirwa <iamhirwejr@gmail.com>
Date:   Sat May 18 17:32:23 2024 +0200

    Update README

commit 86ec50c18b51931cfc83c61a5490ebcb4447f306
Author: Junior Hirwa <iamhirwejr@gmail.com>
Date:   Sat May 18 15:47:09 2024 +0200

    refactor: update README

commit be0f35cda6dd4e00a34fa33bba3cd8d94d6d3feb
Author: Junior Hirwa <117777634+HIRWA13@users.noreply.github.com>    
Date:   Sat May 18 10:55:19 2024 +0200

    Update README.md

commit 6483bd64391b2c2b0682481853ea3a32aeea6816
Author: Junior Hirwa <117777634+HIRWA13@users.noreply.github.com>    
Date:   Sat May 18 10:14:00 2024 +0200

    Update README.md

commit 9dbca11b1765a872746f675cadccd09ab50f4fd5
Author: Algor Fernand <131036952+Algor-Fernand@users.noreply.github.com>
Date:   Fri May 17 18:27:50 2024 +0200

    Update README.md

commit 7cd7a2983997480b7ed637e4ceb53eaafebc1900
Merge: 6e0e33f bf8e72c
Author: Algor Fernand <131036952+Algor-Fernand@users.noreply.github.com>
Date:   Fri May 17 18:20:28 2024 +0200

    Merge pull request #1 from HIRWA13/chore/refine-exercises        

    refactor: Update Exercises

commit bf8e72c7f07cba3fb8c3b613bd4114adf28c467f
Author: Algor Fernand <131036952+Algor-Fernand@users.noreply.github.com>
Date:   Fri May 17 18:19:10 2024 +0200

    Update README.md

commit e632651b97aabf62c17a581cd84cbf5f11dd465c
Author: Junior Hirwa <iamhirwejr@gmail.com>
Date:   Fri May 17 16:20:03 2024 +0200

    refactor: clean and update exercise structure

commit aabb257cbf4b01b048df45dfe112e714b5275688
Author: Junior Hirwa <iamhirwejr@gmail.com>
Date:   Fri May 17 16:06:02 2024 +0200

    refactor: create branch from a commit

commit 4f71b9f5fa523c31abf31a188a09c17a0f71d179
Merge: 6448eeb 6e0e33f
Author: Junior Hirwa <iamhirwejr@gmail.com>
Date:   Fri May 17 15:59:56 2024 +0200

    refactor: update exercises


commit 23ea742821372b58d22749047000ad2e14ae52f9
Author: Junior Hirwa <iamhirwejr@gmail.com>

The Gym@Kevin MINGW32 ~/Git-exercise (main|REBASE 1/2)
$ git reset --hard head~
HEAD is now at 826eba3 Update README

The Gym@Kevin MINGW32 ~/Git-exercise (main|REBASE 1/2)
$ [200~touch test{1..4}.md
bash: [200~touch: command not found

The Gym@Kevin MINGW32 ~/Git-exercise (main|REBASE 1/2)
$ git add test1.md && git commit -m "chore: Create initial file"
fatal: pathspec 'test1.md' did not match any files

The Gym@Kevin MINGW32 ~/Git-exercise (main|REBASE 1/2)
$ git add test2.md && git commit -m "chore: Create another file"
fatal: pathspec 'test2.md' did not match any files

The Gym@Kevin MINGW32 ~/Git-exercise (main|REBASE 1/2)
$ git add test3.md && git commit -m "chore: Create third and fourth files"~
fatal: pathspec 'test3.md' did not match any files

The Gym@Kevin MINGW32 ~/Git-exercise (main|REBASE 1/2)
$ touch test{1..4}.md

The Gym@Kevin MINGW32 ~/Git-exercise (main|REBASE 1/2)
$ ls 
README.md  test1.md  test2.md  test3.md  test4.md

The Gym@Kevin MINGW32 ~/Git-exercise (main|REBASE 1/2)
$ git add test1.md 

The Gym@Kevin MINGW32 ~/Git-exercise (main|REBASE 1/2)
$ git commit -m "chore: Create initial file"
[detached HEAD 782759c] chore: Create initial file
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test1.md

The Gym@Kevin MINGW32 ~/Git-exercise (main|REBASE 1/2)
$ git add test2.md

The Gym@Kevin MINGW32 ~/Git-exercise (main|REBASE 1/2)
$ git commit -m "chore: Create another file"
[detached HEAD 9e048c2] chore: Create another file
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test2.md

The Gym@Kevin MINGW32 ~/Git-exercise (main|REBASE 1/2)
$ git commit -m "chore: Create third and fourth files" 
interactive rebase in progress; onto b03f09e
Last command done (1 command done):
   edit a784e9a chore: Create another file
Next command to do (1 remaining command):
   pick ed1f8ee Create second file
  (use "git rebase --edit-todo" to view and edit)
You are currently editing a commit while rebasing branch 'main' on 'b03f09e'.
  (use "git commit --amend" to amend the current commit)
  (use "git rebase --continue" once you are satisfied with your changes)

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        test3.md
        test4.md

nothing added to commit but untracked files present (use "git add" to track)

The Gym@Kevin MINGW32 ~/Git-exercise (main|REBASE 1/2)
$ git add test3.md

The Gym@Kevin MINGW32 ~/Git-exercise (main|REBASE 1/2)
$ git commit -m "chore: Create third and fourth files"  
[detached HEAD 767f60e] chore: Create third and fourth files
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test3.md

The Gym@Kevin MINGW32 ~/Git-exercise (main|REBASE 1/2)
$ ls 
README.md  test1.md  test2.md  test3.md  test4.md

The Gym@Kevin MINGW32 ~/Git-exercise (main|REBASE 1/2)
$ git log 
commit 767f60eb0ab317b66d0fa6c5e6aa6303bfe4b180 (HEAD)
Author: Kevin-gram <k.nyiringan@alustudent.com>
Date:   Mon May 20 19:30:56 2024 +0200

    chore: Create third and fourth files

commit 9e048c23091cc35a17e23c35497dd07f4fda7266
Author: Kevin-gram <k.nyiringan@alustudent.com>
Date:   Mon May 20 19:25:44 2024 +0200

    chore: Create another file

commit 782759c9ba808118e9083c42148000b43f74d597
Author: Kevin-gram <k.nyiringan@alustudent.com>
Date:   Mon May 20 19:25:06 2024 +0200

    chore: Create initial file

commit 826eba3e6add8872f92eb03855910bda3b8aadbf
Author: Junior Hirwa <iamhirwejr@gmail.com>
Date:   Sat May 18 17:32:23 2024 +0200

    Update README

commit 86ec50c18b51931cfc83c61a5490ebcb4447f306
Author: Junior Hirwa <iamhirwejr@gmail.com>
Date:   Sat May 18 15:47:09 2024 +0200

    refactor: update README

commit be0f35cda6dd4e00a34fa33bba3cd8d94d6d3feb
Author: Junior Hirwa <117777634+HIRWA13@users.noreply.github.com>
Date:   Sat May 18 10:55:19 2024 +0200

    Update README.md

commit 6483bd64391b2c2b0682481853ea3a32aeea6816
Author: Junior Hirwa <117777634+HIRWA13@users.noreply.github.com>
Date:   Sat May 18 10:14:00 2024 +0200

    Update README.md

commit 9dbca11b1765a872746f675cadccd09ab50f4fd5
Author: Algor Fernand <131036952+Algor-Fernand@users.noreply.github.com>
Date:   Fri May 17 18:27:50 2024 +0200

    Update README.md

commit 7cd7a2983997480b7ed637e4ceb53eaafebc1900
Merge: 6e0e33f bf8e72c
Author: Algor Fernand <131036952+Algor-Fernand@users.noreply.github.com>
Date:   Fri May 17 18:20:28 2024 +0200

    Merge pull request #1 from HIRWA13/chore/refine-exercises

    refactor: Update Exercises

commit bf8e72c7f07cba3fb8c3b613bd4114adf28c467f
Author: Algor Fernand <131036952+Algor-Fernand@users.noreply.github.com>
Date:   Fri May 17 18:19:10 2024 +0200

    Update README.md

commit e632651b97aabf62c17a581cd84cbf5f11dd465c
Author: Junior Hirwa <iamhirwejr@gmail.com>
Date:   Fri May 17 16:20:03 2024 +0200

    refactor: clean and update exercise structure

commit aabb257cbf4b01b048df45dfe112e714b5275688
Author: Junior Hirwa <iamhirwejr@gmail.com>
Date:   Fri May 17 16:06:02 2024 +0200

    refactor: create branch from a commit

commit 4f71b9f5fa523c31abf31a188a09c17a0f71d179
Merge: 6448eeb 6e0e33f
Author: Junior Hirwa <iamhirwejr@gmail.com>
Date:   Fri May 17 15:59:56 2024 +0200

    refactor: update exercises

commit 6448eeb3e42566af9232efab3539e4c1f9347ebf
Author: Junior Hirwa <iamhirwejr@gmail.com>
Date:   Fri May 17 15:55:59 2024 +0200

    refactor: update readme file

commit 013976b22dd793cab99bbc6137bd4c84f017b46f
Author: Junior Hirwa <iamhirwejr@gmail.com>
Date:   Fri May 17 15:22:10 2024 +0200

    refactor: update exercises

commit 23ea742821372b58d22749047000ad2e14ae52f9
Author: Junior Hirwa <iamhirwejr@gmail.com>
Date:   Fri May 17 15:11:07 2024 +0200

    refactor: update and remove mistakes

commit 248fb71f4dfcd9e4b519f8e9f05c76b35303e2a5
Author: Junior Hirwa <iamhirwejr@gmail.com>
Date:   Fri May 17 12:58:14 2024 +0200

    refactor: Update Exercises

commit 6e0e33f7aab609f19a56361ca99affde732ce60d
Author: Junior Hirwa <117777634+HIRWA13@users.noreply.github.com>
Date:   Fri May 17 10:41:57 2024 +0200

    refactor: Update README.md
024 +0200

    refactor: update README

commit ea7834e239ce2a6d0f64dec2770679b8935f73e9
Author: Junior Hirwa <iamhirwejr@gmail.com>
Date:   Fri May 17 10:22:39 2024 +0200

chore: Create third and fourth file
    chore: add part one exercises

The Gym@Kevin MINGW32 ~/Git-exercise (main|REBASE 1/2)
$ git add test4.md

The Gym@Kevin MINGW32 ~/Git-exercise (main|REBASE 1/2)
$ git commit --amend
hint: Waiting for your editor to close the file...






[detached HEAD 67cfae2] chore: Create third and fourth files
 Date: Mon May 20 19:30:56 2024 +0200
 2 files changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test3.md
 create mode 100644 test4.md

The Gym@Kevin MINGW32 ~/Git-exercise (main|REBASE 1/2)
$ git commit --amend
[detached HEAD 4c52ab4] chore: Create third and fourth file
 Date: Mon May 20 19:30:56 2024 +0200
 2 files changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test3.md
 create mode 100644 test4.md

The Gym@Kevin MINGW32 ~/Git-exercise (main|REBASE 1/2)
$ git rebase -i HEAD~2
fatal: It seems that there is already a rebase-merge directory, and
I wonder if you are in the middle of another rebase.  If that is the
case, please try
        git rebase (--continue | --abort | --skip)
If that is not the case, please
        rm -fr ".git/rebase-merge"
and run me again.  I am stopping in case you still have something
valuable there.


The Gym@Kevin MINGW32 ~/Git-exercise (main|REBASE 1/2)
$ git rebase 
fatal: It seems that there is already a rebase-merge directory, and
I wonder if you are in the middle of another rebase.  If that is the       
case, please try
        git rebase (--continue | --abort | --skip)
If that is not the case, please
        rm -fr ".git/rebase-merge"
pick 782759c chore: Create initial file
and run me again.  I am stopping in case you still have something
valuable there.


The Gym@Kevin MINGW32 ~/Git-exercise (main|REBASE 1/2)
$ git rebase -i
fatal: It seems that there is already a rebase-merge directory, and        
I wonder if you are in the middle of another rebase.  If that is the       
case, please try
        git rebase (--continue | --abort | --skip)
If that is not the case, please
        rm -fr ".git/rebase-merge"
and run me again.  I am stopping in case you still have something
valuable there.


The Gym@Kevin MINGW32 ~/Git-exercise (main|REBASE 1/2)
$ git rebase --continue
Successfully rebased and updated refs/heads/main.

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git rebase -i
Successfully rebased and updated refs/heads/main.

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git rebase -i
Successfully rebased and updated refs/heads/main.

The Gym@Kevin MINGW32 ~/Git-exercise (main
