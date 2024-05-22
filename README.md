
The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ touch test{1..4}.md

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ ls 
README.md  test1.md  test2.md  test3.md  test4.md

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git add test1.md 

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git commit -m "chore: Create initial file"
[main 0ad24d3] chore: Create initial file
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test1.md

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git add test2.md 

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git commit -m "chore: Create another file"
[main f3829b3] chore: Create another file
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test2.md

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git add test3.md 

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git commit -m "chore: Create third and fourth files"
[main 07851bd] chore: Create third and fourth files
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test3.md

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git log 
commit 07851bda6db6952fbdbcc9d0fa0d5f5b342293d9 (HEAD -> main)
Author: Kevin-gram <k.nyiringan@alustudent.com>
Date:   Tue May 21 11:35:42 2024 +0200

    chore: Create third and fourth files

commit f3829b3f448f687bd0353b4dcbb79830b0c107b5
Author: Kevin-gram <k.nyiringan@alustudent.com>
Date:   Tue May 21 11:34:37 2024 +0200

chore: this is the commit for the 4th test
    chore: Create another file

commit 0ad24d3173669e2f8c33b2c0a11940b8e0dfe1fd
Author: Kevin-gram <k.nyiringan@alustudent.com>
Date:   Tue May 21 11:33:35 2024 +0200

    chore: Create initial file

pick f3829b3 chore: Create second file
commit e4744a08b30e2268795804bd5e55d1335bf68c73 (origin/main, origin/HEAD) 
Author: Junior Hirwa <117777634+HIRWA13@users.noreply.github.com>
Date:   Sun May 19 11:20:17 2024 +0200

pick 0ad24d3 chore: Create initial file

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git add test4.md

pick 0ad24d3 chore: Create initial file
The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git commit commit --amend
error: pathspec 'commit' did not match any file(s) known to git

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git commit  --amend
[main 17e74b9] chore: this is the commit for the 4th test
 Date: Tue May 21 11:35:42 2024 +0200
 2 files changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test3.md
 create mode 100644 test4.md

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git rebase -i HEAD~2
Successfully rebased and updated refs/heads/main.

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git rebase -i
Successfully rebased and updated refs/heads/main.

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git rebase -i
[detached HEAD f430375] chore: Create initial file
 Date: Tue May 21 11:33:35 2024 +0200
 2 files changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test1.md
 create mode 100644 test2.md
Successfully rebased and updated refs/heads/main.

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git rebase -i
Successfully rebased and updated refs/heads/main.

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git log
commit 62f87587304ed25ee8010e7d39cbf2470ccb302d (HEAD -> main)
Author: Kevin-gram <k.nyiringan@alustudent.com>
Date:   Tue May 21 11:35:42 2024 +0200

    chore: this is the commit for the 4th test

commit f43037533a95f890c577ed63ac7ebc415e2486c5
Author: Kevin-gram <k.nyiringan@alustudent.com>
Date:   Tue May 21 11:33:35 2024 +0200

    chore: Create initial file

    chore: Create another file

commit e4744a08b30e2268795804bd5e55d1335bf68c73 (origin/main, origin/HEAD) 
Author: Junior Hirwa <117777634+HIRWA13@users.noreply.github.com>
Date:   Sun May 19 11:20:17 2024 +0200

    Update README.md

commit 3083f669516ea1396caaa74c8216de8cbe8236d3
Author: Junior Hirwa <iamhirwejr@gmail.com>

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git rebase -i HEAD~2
Successfully rebased and updated refs/heads/main.

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git rebase -i
Successfully rebased and updated refs/heads/main.

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git reset

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git rebase HEAD~4
Current branch main is up to date.

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git rebase -i
Successfully rebased and updated refs/heads/main.

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git log 
commit 62f87587304ed25ee8010e7d39cbf2470ccb302d (HEAD -> main)
Author: Kevin-gram <k.nyiringan@alustudent.com>
Date:   Tue May 21 11:35:42 2024 +0200

    chore: this is the commit for the 4th test

commit f43037533a95f890c577ed63ac7ebc415e2486c5
Author: Kevin-gram <k.nyiringan@alustudent.com>
Date:   Tue May 21 11:33:35 2024 +0200

    chore: Create initial file

    chore: Create another file

commit e4744a08b30e2268795804bd5e55d1335bf68c73 (origin/main, origin/HEAD) 
Author: Junior Hirwa <117777634+HIRWA13@users.noreply.github.com>
Date:   Sun May 19 11:20:17 2024 +0200

    Update README.md

commit 3083f669516ea1396caaa74c8216de8cbe8236d3
Author: Junior Hirwa <iamhirwejr@gmail.com>

The Gym@Kevin MINGW32 ~/Git-exercise (main)

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ touch test{1..4}.md

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ ls
README.md  test1.md  test2.md  test3.md  test4.md

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git add test1.md

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git commit -m "chore: Create initial file"
[main 0ad24d3] chore: Create initial file
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test1.md

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git add test2.md

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git commit -m "chore: Create another file"
[main f3829b3] chore: Create another file
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test2.md

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git add test3.md

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git commit -m "chore: Create third and fourth files"
[main 07851bd] chore: Create third and fourth files
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test3.md

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git log
commit 07851bda6db6952fbdbcc9d0fa0d5f5b342293d9 (HEAD -> main)
Author: Kevin-gram <k.nyiringan@alustudent.com>
Date:   Tue May 21 11:35:42 2024 +0200

    chore: Create third and fourth files

commit f3829b3f448f687bd0353b4dcbb79830b0c107b5
Author: Kevin-gram <k.nyiringan@alustudent.com>
Date:   Tue May 21 11:34:37 2024 +0200

chore: this is the commit for the 4th test
    chore: Create another file

commit 0ad24d3173669e2f8c33b2c0a11940b8e0dfe1fd
Author: Kevin-gram <k.nyiringan@alustudent.com>
Date:   Tue May 21 11:33:35 2024 +0200

    chore: Create initial file

pick f3829b3 chore: Create second file
commit e4744a08b30e2268795804bd5e55d1335bf68c73 (origin/main, origin/HEAD)
Author: Junior Hirwa <117777634+HIRWA13@users.noreply.github.com>
Date:   Sun May 19 11:20:17 2024 +0200

pick 0ad24d3 chore: Create initial file

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git add test4.md

pick 0ad24d3 chore: Create initial file
The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git commit commit --amend
error: pathspec 'commit' did not match any file(s) known to git

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git commit  --amend
[main 17e74b9] chore: this is the commit for the 4th test
 Date: Tue May 21 11:35:42 2024 +0200
 2 files changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test3.md
 create mode 100644 test4.md

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git rebase -i HEAD~2
Successfully rebased and updated refs/heads/main.

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git rebase -i
Successfully rebased and updated refs/heads/main.

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git rebase -i
[detached HEAD f430375] chore: Create initial file
 Date: Tue May 21 11:33:35 2024 +0200
 2 files changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test1.md
 create mode 100644 test2.md
Successfully rebased and updated refs/heads/main.

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git rebase -i
Successfully rebased and updated refs/heads/main.

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git log
commit 62f87587304ed25ee8010e7d39cbf2470ccb302d (HEAD -> main)
Author: Kevin-gram <k.nyiringan@alustudent.com>
Date:   Tue May 21 11:35:42 2024 +0200

    chore: this is the commit for the 4th test

commit f43037533a95f890c577ed63ac7ebc415e2486c5
Author: Kevin-gram <k.nyiringan@alustudent.com>
Date:   Tue May 21 11:33:35 2024 +0200

    chore: Create initial file

    chore: Create another file

commit e4744a08b30e2268795804bd5e55d1335bf68c73 (origin/main, origin/HEAD)
Author: Junior Hirwa <117777634+HIRWA13@users.noreply.github.com>
Date:   Sun May 19 11:20:17 2024 +0200

    Update README.md

commit 3083f669516ea1396caaa74c8216de8cbe8236d3
Author: Junior Hirwa <iamhirwejr@gmail.com>

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git rebase -i HEAD~2
Successfully rebased and updated refs/heads/main.

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git rebase -i
Successfully rebased and updated refs/heads/main.

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git reset

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git rebase HEAD~4
Current branch main is up to date.

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git rebase -i
Successfully rebased and updated refs/heads/main.

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git log
commit 62f87587304ed25ee8010e7d39cbf2470ccb302d (HEAD -> main)
Author: Kevin-gram <k.nyiringan@alustudent.com>
Date:   Tue May 21 11:35:42 2024 +0200

    chore: this is the commit for the 4th test

commit f43037533a95f890c577ed63ac7ebc415e2486c5
Author: Kevin-gram <k.nyiringan@alustudent.com>
Date:   Tue May 21 11:33:35 2024 +0200

    chore: Create initial file

    chore: Create another file

commit e4744a08b30e2268795804bd5e55d1335bf68c73 (origin/main, origin/HEAD)
Author: Junior Hirwa <117777634+HIRWA13@users.noreply.github.com>
Date:   Sun May 19 11:20:17 2024 +0200

    Update README.md

commit 3083f669516ea1396caaa74c8216de8cbe8236d3
Author: Junior Hirwa <iamhirwejr@gmail.com>

The Gym@Kevin MINGW32 ~/Git-exercise (main)
pick f430375 chore: Create initial file
$ git add unwanted.txt

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git commit -m"unwanted "Unwanted commit"
pick 4303tial file
> git commit -m "Unwanted commit"
> git commit -m "unwanted commit "
pick 4303tial file
> ^C

The Gym@Kevin MINGW32 ~/Git-exercise (main)
pick 4303tial file
$ git commit -m"unwanted "Unwanted commit"
git commit -m "Unwanted commit"
pick 4303tial file
git commit -m "unwanted commit "
> ^C

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git commit -m "unwanted file "
[main 1e1fd8c] unwanted file
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 unwanted.txt

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git rebase -i
Successfully rebased and updated refs/heads/main.

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git rebase -i
hint: Waiting for your editor to close the file...       2 [sig] bash 1207! sigpacket::process: Suppressing signal 18 to win32 process (pid 5556)
                                                                       998407 [sig] bash 1207! sigpacket::process: Suppressing signal 18 to win32 process (pid 5556)
              2488889 [sig] bash 1207! sigpacket::process: Suppressing signal 18 to win32 process (pid 5556)
error: could not parse '4303tial'
error: invalid line 1: pick 4303tial file
You can fix this with 'git rebase --edit-todo' and then run 'git rebase --continue'.
Or you can abort the rebase with 'git rebase --abort'.

The Gym@Kevin MINGW32 ~/Git-exercise (main|REBASE)
$ git rebase -i
fatal: It seems that there is already a rebase-merge directory, and
I wonder if you are in the middle of another rebase.  If that is the
pick f430375 chore:  initial file
case, please try
        git rebase (--continue | --abort | --skip)
If that is not the case, please
        rm -fr ".git/rebase-merge"
and run me again.  I am stopping in case you still have something
valuable there.

pick  62f8758 chore: this is the commit for the 4th test

The Gym@Kevin MINGW32 ~/Git-exercise (main|REBASE)
$ git rebase -continue
error: did you mean `--continue` (with two dashes)?

The Gym@Kevin MINGW32 ~/Git-exercise (main|REBASE)
$ git rebase --continue
error: could not parse '4303tial'
error: invalid line 1: pick 4303tial file
error: please fix this using 'git rebase --edit-todo'.

The Gym@Kevin MINGW32 ~/Git-exercise (main|REBASE)
$ git rebase --edit-todo
error: could not parse '4303tial'
error: invalid line 1: pick 4303tial file

The Gym@Kevin MINGW32 ~/Git-exercise (main|REBASE)
$ git rebase --continue
Successfully rebased and updated refs/heads/main.

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git rebase -i
Successfully rebased and updated refs/heads/main.

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git checkout ft/branch
error: pathspec 'ft/branch' did not match any file(s) known to git

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git branch ft/branch

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git checkout ft/branch
Switched to branch 'ft/branch'

The Gym@Kevin MINGW32 ~/Git-exercise (ft/branch)
$ vi test5.md

The Gym@Kevin MINGW32 ~/Git-exercise (ft/branch)
$ git commit -m"Implemented test 5"
On branch ft/branch
nothing to commit, working tree clean

The Gym@Kevin MINGW32 ~/Git-exercise (ft/branch)
$ git log
commit 1537fe484aa7f1cd10137112844f0f2dbad618f8 (HEAD -> ft/branch, main)
Author: Kevin-gram <k.nyiringan@alustudent.com>
Date:   Tue May 21 11:33:35 2024 +0200

    chore: Create initial file

    chore: Create another file

commit dd69f7a887c7e19d3f06ac55bb0a2b64566b3a75
Author: Kevin-gram <k.nyiringan@alustudent.com>
Date:   Tue May 21 11:35:42 2024 +0200

    chore: this is the commit for the 4th test

commit e4744a08b30e2268795804bd5e55d1335bf68c73 (origin/main, origin/HEAD)
Author: Junior Hirwa <117777634+HIRWA13@users.noreply.github.com>
Date:   Sun May 19 11:20:17 2024 +0200

    Update README.md

commit 3083f669516ea1396caaa74c8216de8cbe8236d3
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
commit 1537fe484aa7f1cd10137112844f0f2dbad618f8 (HEAD -> ft/branch, main)
Author: Kevin-gram <k.nyiringan@alustudent.com>
Date:   Tue May 21 11:33:35 2024 +0200

    chore: Create initial file
commit 1537fe484aa7f1cd10137112844f0f2dbad618f8 (HEAD -> ft/branch, main)
Author: Kevin-gram <k.nyiringan@alustudent.com>
Date:   Tue May 21 11:33:35 2024 +0200

    chore: Create initial file

    chore: Create another file

commit dd69f7a887c7e19d3f06ac55bb0a2b64566b3a75
Author: Kevin-gram <k.nyiringan@alustudent.com>
Date:   Tue May 21 11:35:42 2024 +0200

    chore: this is the commit for the 4th test

commit e4744a08b30e2268795804bd5e55d1335bf68c73 (origin/main, origin/HEAD)
Author: Junior Hirwa <117777634+HIRWA13@users.noreply.github.com>
Date:   Sun May 19 11:20:17 2024 +0200

    Update README.md

commit 3083f669516ea1396caaa74c8216de8cbe8236d3
Author: Junior Hirwa <iamhirwejr@gmail.com>

The Gym@Kevin MINGW32 ~/Git-exercise (ft/branch)
$ git commit -m"Implemented test 5"
On branch ft/branch
nothing to commit, working tree clean

The Gym@Kevin MINGW32 ~/Git-exercise (ft/branch)
$ git log
commit 1537fe484aa7f1cd10137112844f0f2dbad618f8 (HEAD -> ft/branch, main)
Author: Kevin-gram <k.nyiringan@alustudent.com>
Date:   Tue May 21 11:33:35 2024 +0200

    chore: Create initial file

    chore: Create another file

commit dd69f7a887c7e19d3f06ac55bb0a2b64566b3a75
Author: Kevin-gram <k.nyiringan@alustudent.com>
Date:   Tue May 21 11:35:42 2024 +0200

    chore: this is the commit for the 4th test

commit e4744a08b30e2268795804bd5e55d1335bf68c73 (origin/main, origin/HEAD)
Author: Junior Hirwa <117777634+HIRWA13@users.noreply.github.com>
Date:   Sun May 19 11:20:17 2024 +0200
iiii

    Update README.md

commit 3083f669516ea1396caaa74c8216de8cbe8236d3
Author: Junior Hirwa <iamhirwejr@gmail.com>

The Gym@Kevin MINGW32 ~/Git-exercise (ft/branch)
$ git checkout main
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 2 commits.
  (use "git push" to publish your local commits)

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git checkout ft/branch
Switched to branch 'ft/branch'

The Gym@Kevin MINGW32 ~/Git-exercise (ft/branch)
$ ls
README.md  test1.md  test2.md  test3.md  test4.md

The Gym@Kevin MINGW32 ~/Git-exercise (ft/branch)
$ vi test5.md

The Gym@Kevin MINGW32 ~/Git-exercise (ft/branch)
$ git commit -m"Implemented test 5"
On branch ft/branch
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        test5.md

nothing added to commit but untracked files present (use "git add" to track)

The Gym@Kevin MINGW32 ~/Git-exercise (ft/branch)
$ git add .
warning: in the working copy of 'test5.md', LF will be replaced by CRLF the next time Git touches it

The Gym@Kevin MINGW32 ~/Git-exercise (ft/branch)
$ git commit -m"Implemented test 5"
[ft/branch 1895d69] Implemented test 5
 1 file changed, 1 insertion(+)
 create mode 100644 test5.md

The Gym@Kevin MINGW32 ~/Git-exercise (ft/branch)
$ git checkout main
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 2 commits.
  (use "git push" to publish your local commits)

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git checkout ft/branch
Switched to branch 'ft/branch'

The Gym@Kevin MINGW32 ~/Git-exercise (ft/branch)
$ git log
commit 1895d691557bda1fa5b4be3689f4a86a4630de97 (HEAD -> ft/branch)
Author: Kevin-gram <k.nyiringan@alustudent.com>
Date:   Tue May 21 15:26:42 2024 +0200

    Implemented test 5

commit 1537fe484aa7f1cd10137112844f0f2dbad618f8 (main)
Author: Kevin-gram <k.nyiringan@alustudent.com>
Date:   Tue May 21 11:33:35 2024 +0200

    chore: Create initial file

    chore: Create another file

commit dd69f7a887c7e19d3f06ac55bb0a2b64566b3a75
Author: Kevin-gram <k.nyiringan@alustudent.com>
Date:   Tue May 21 11:35:42 2024 +0200

    chore: this is the commit for the 4th test

commit e4744a08b30e2268795804bd5e55d1335bf68c73 (origin/main, origin/HEAD)
Author: Junior Hirwa <117777634+HIRWA13@users.noreply.github.com>

The Gym@Kevin MINGW32 ~/Git-exercise (ft/branch)
$ git checkout main
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 2 commits.
  (use "git push" to publish your local commits)

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git cherry-pick 1895d691557bda1fa5b4be3689f4a86a4630de97
[main ea30c35] Implemented test 5
 Date: Tue May 21 15:26:42 2024 +0200
 1 file changed, 1 insertion(+)
 create mode 100644 test5.md

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git log --graph
* commit ea30c35f8d0bc68872c83694ecd488d3d4e697bf (HEAD -> main)
| Author: Kevin-gram <k.nyiringan@alustudent.com>
| Date:   Tue May 21 15:26:42 2024 +0200
|
|     Implemented test 5
|
* commit 1537fe484aa7f1cd10137112844f0f2dbad618f8
| Author: Kevin-gram <k.nyiringan@alustudent.com>
| Date:   Tue May 21 11:33:35 2024 +0200
|
|     chore: Create initial file
|
|     chore: Create another file
|
* commit dd69f7a887c7e19d3f06ac55bb0a2b64566b3a75
| Author: Kevin-gram <k.nyiringan@alustudent.com>
| Date:   Tue May 21 11:35:42 2024 +0200
|
|     chore: this is the commit for the 4th test
|
* commit e4744a08b30e2268795804bd5e55d1335bf68c73 (origin/main, origin/HEAD)
:$implemented functionality for new feature

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git checkout ft/new-feature
error: pathspec 'ft/new-feature' did not match any file(s) known to git    

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git branch ft/new-feature

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git branch ft/new-feature
fatal: a branch named 'ft/new-feature' already exists

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git checkout ft/new-feature
Switched to branch 'ft/new-feature'

The Gym@Kevin MINGW32 ~/Git-exercise (ft/new-feature)
 with some introductory content. Commit these changes with a message like "$ vi feature.txt

The Gym@Kevin MINGW32 ~/Git-exercise (ft/new-feature)
$ git add .
warning: in the working copy of 'feature.txt', LF will be replaced by CRLF the next time Git touches it

The Gym@Kevin MINGW32 ~/Git-exercise (ft/new-feature)
$ git commit -m "Implemented core functionality for new feature"
[ft/new-feature dba2a4d] Implemented core functionality for new feature    
 2 files changed, 2 insertions(+)
 create mode 100644 feature.txt
 create mode 100644 unwanted.txt

The Gym@Kevin MINGW32 ~/Git-exercise (ft/new-feature)
$ git checkout main
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 3 commits.
  (use "git push" to publish your local commits)

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ vi readme.txt

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git add readme.txt 
warning: in the working copy of 'readme.txt', LF will be replaced by CRLF the next time Git touches it

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git commit -m "Updated project readme"
[main dfb8f86] Updated project readme
 1 file changed, 1 insertion(+)
 create mode 100644 readme.txt

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ ls 
README.md  readme.txt  test1.md  test2.md  test3.md  test4.md  test5.md

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git checkout -d ft/new-feature  
HEAD is now at dba2a4d Implemented core functionality for new feature

The Gym@Kevin MINGW32 ~/Git-exercise ((dba2a4d...))
$ git branch  -d ft/new-feature
Deleted branch ft/new-feature (was dba2a4d).

The Gym@Kevin MINGW32 ~/Git-exercise ((dba2a4d...))
$ git checkout main
Warning: you are leaving 1 commit behind, not connected to
any of your branches:

  dba2a4d Implemented core functionality for new feature

If you want to keep it by creating a new branch, this may be a good time   
to do so with:

 git branch <new-branch-name> dba2a4d

Switched to branch 'main'
Your branch is ahead of 'origin/main' by 4 commits.
  (use "git push" to publish your local commits)

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git log 
commit dfb8f861b4a4111ea463f981b7051cfcdff02b01 (HEAD -> main)
Author: Kevin-gram <k.nyiringan@alustudent.com>
Date:   Tue May 21 16:03:01 2024 +0200

    Updated project readme

commit ea30c35f8d0bc68872c83694ecd488d3d4e697bf
Author: Kevin-gram <k.nyiringan@alustudent.com>
Date:   Tue May 21 15:26:42 2024 +0200

    Implemented test 5

commit 1537fe484aa7f1cd10137112844f0f2dbad618f8
Author: Kevin-gram <k.nyiringan@alustudent.com>
Date:   Tue May 21 11:33:35 2024 +0200

    chore: Create initial file

    chore: Create another file

commit dd69f7a887c7e19d3f06ac55bb0a2b64566b3a75
Author: Kevin-gram <k.nyiringan@alustudent.com>
Date:   Tue May 21 11:35:42 2024 +0200

    chore: this is the commit for the 4th test

commit e4744a08b30e2268795804bd5e55d1335bf68c73 (origin/main, origin/HEAD) 
Author: Junior Hirwa <117777634+HIRWA13@users.noreply.github.com>

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git checkout -b ft/new-branch-from-commit 1895d691557bda1fa5b4be3689f4a86
a4630de97
Switched to a new branch 'ft/new-branch-from-commit'

The Gym@Kevin MINGW32 ~/Git-exercise (ft/new-branch-from-commit)
The Gym@Kevin MINGW32 ~/Git-exercise (ft/new-branch-from-commit)
$ git checkout main
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 4 commits.
  (use "git push" to publish your local commits)

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git merge ft/new-branch-from-commit
Merge made by the 'ort' strategy.

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git rebase ft/new-branch-from-commit
dropping ea30c35f8d0bc68872c83694ecd488d3d4e697bf Implemented test 5 -- patch contents already upstream
Successfully rebased and updated refs/heads/main.

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git branch -m ft/new-branch-from-commit ft/improved-branch-name

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git log 
commit 6d815e2bb4fb6e5294b3949172592b0eca20006c (HEAD -> main)
Author: Kevin-gram <k.nyiringan@alustudent.com>
Date:   Tue May 21 16:03:01 2024 +0200

    Updated project readme

commit 1895d691557bda1fa5b4be3689f4a86a4630de97 (ft/improved-branch-name, ft/branch)
Author: Kevin-gram <k.nyiringan@alustudent.com>
Date:   Tue May 21 15:26:42 2024 +0200

    Implemented test 5

commit 1537fe484aa7f1cd10137112844f0f2dbad618f8
Author: Kevin-gram <k.nyiringan@alustudent.com>
Date:   Tue May 21 11:33:35 2024 +0200

    chore: Create initial file

    chore: Create another file

commit dd69f7a887c7e19d3f06ac55bb0a2b64566b3a75

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git checkout 1537fe484aa7f1cd10137112844f0f2dbad618f8
Note: switching to '1537fe484aa7f1cd10137112844f0f2dbad618f8'.

You are in 'detached HEAD' state. You can look around, make experimental   
changes and commit them, and you can discard any commits you make in this  
state without impacting any branches by switching back to a branch.        

If you want to create a new branch to retain commits you create, you may   
do so (now or later) by using -c with the switch command. Example:

  git switch -c <new-branch-name>

Or undo this operation with:

  git switch -

Turn off this advice by setting config variable advice.detachedHead to false

HEAD is now at 1537fe4 chore: Create initial file

The Gym@Kevin MINGW32 ~/Git-exercise ((1537fe4...))
$ $ git stash
No local changes to save

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ vi test1.md

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git stash
warning: in the working copy of 'test1.md', LF will be replaced by CRLF the next time Git touches it
Saved working directory and index state WIP on main: ab36c59 un needed changes

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git log 
commit ab36c593f7403ab583a24cac3daab6c1d156e365 (HEAD -> main)
Author: Kevin-gram <k.nyiringan@alustudent.com>
Date:   Wed May 22 15:58:47 2024 +0200

    un needed changes

commit 6d815e2bb4fb6e5294b3949172592b0eca20006c
Author: Kevin-gram <k.nyiringan@alustudent.com>
Date:   Tue May 21 16:03:01 2024 +0200

    Updated project readme

commit 1895d691557bda1fa5b4be3689f4a86a4630de97 (ft/improved-branch-name, ft/branch)
Author: Kevin-gram <k.nyiringan@alustudent.com>
Date:   Tue May 21 15:26:42 2024 +0200

    Implemented test 5

commit 1537fe484aa7f1cd10137112844f0f2dbad618f8
Author: Kevin-gram <k.nyiringan@alustudent.com>
Date:   Tue May 21 11:33:35 2024 +0200

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git stash pop
On branch main
Your branch is ahead of 'origin/main' by 5 commits.
  (use "git push" to publish your local commits)

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)    
        modified:   test1.md

no changes added to commit (use "git add" and/or "git commit -a")
Dropped refs/stash@{0} (50a3a19f4aa86692f00f10dff32071cd773ab718)

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git checkout ft/new-branch-from-commit
error: pathspec 'ft/new-branch-from-commit' did not match any file(s) known to git

kevin here!
The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git checkout ft/improved-branch-name
error: Your local changes to the following files would be overwritten by checkout:
        test1.md
Please commit your changes or stash them before you switch branches.       
Aborting

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git add .

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git commit -m "un needed changes"
[main 60cdc22] un needed changes
 1 file changed, 1 insertion(+), 1 deletion(-)

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git checkout ft/improved-branch-name
Switched to branch 'ft/improved-branch-name'

The Gym@Kevin MINGW32 ~/Git-exercise (ft/improved-branch-name)
$ vi test1.md

The Gym@Kevin MINGW32 ~/Git-exercise (ft/improved-branch-name)
$ git add .
kevin here!
warning: in the working copy of 'test1.md', LF will be replaced by CRLF the next time Git touches it

The Gym@Kevin MINGW32 ~/Git-exercise (ft/improved-branch-name)
$ git commit -m "Improved changes in the inner branche"
[ft/improved-branch-name 1657bd9] Improved changes in the inner branche    
 1 file changed, 1 insertion(+)

The Gym@Kevin MINGW32 ~/Git-exercise (ft/improved-branch-name)
$ git checkout main
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 6 commits.
  (use "git push" to publish your local commits)

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git merge ft/improved-branch-name
Auto-merging test1.md
CONFLICT (content): Merge conflict in test1.md
Automatic merge failed; fix conflicts and then commit the result.

The Gym@Kevin MINGW32 ~/Git-exercise (main|MERGING)
$ vi test1.md

/tmp
The Gym@Kevin MINGW32 ~/Git-exercise (main|MERGING)
$ git add .

The Gym@Kevin MINGW32 ~/Git-exercise (main|MERGING)
$ git commit -m "merging the conflicts"
[main 7f587af] merging the conflicts

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git checkout ft/improved-branch-name
Switched to branch 'ft/improved-branch-name'

The Gym@Kevin MINGW32 ~/Git-exercise (ft/improved-branch-name)
$ git checkout main
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 8 commits.
  (use "git push" to publish your local commits)

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ vi gitignore

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ vi gitignore

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git tag v1.0

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git tag
v1.0

The Gym@Kevin MINGW32 ~/Git-exercise (main)
$ git tag -d v1.0 
 Deleted tag 'v1.0' (was 7f587af)\$ $ git pull
remote: Enumerating objects: 5, done.
remote: Counting objects: 100% (5/5), done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), 967 bytes | 29.00 KiB/s, done.
From https://github.com/Kevin-gram/Git-advanced
   bbab6c0..07b3690  main       -> origin/main
error: Your local changes to the following files would be overwritten by merge:
        README.md
Please commit your changes or stash them before you merge.
Aborting
Updating bbab6c0..07b3690

