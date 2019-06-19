## TAVISCA SOLUTIONS PVT. LTD. PRE-JOINING ASSIGNMENT-1

### INIT
C:\Users\saqlain>git config --global user.name "Saqlain Kadiri
C:\Users\saqlain>git config --global user.email "skadiri@tavisca.in
C:\Users\saqlain>git config --global core.autocrlf true
C:\Users\saqlain>git config --global core.safecrlf true
C:\Users\saqlain>cd training
C:\Users\saqlain\training>cd work
C:\Users\saqlain\training\work>mkdir hello
C:\Users\saqlain\training\work>cd hello

C:\Users\saqlain\training\work\hello>git init
Initialized empty Git repository in C:/Users/saqlain/training/work/hello/.git/

C:\Users\saqlain\training\work\hello>git add hello.txt

C:\Users\saqlain\training\work\hello>git commit -m "First commit lab3"
[master (root-commit) 4b0a874] First commit lab3
 1 file changed, 1 insertion(+)
 create mode 100644 hello.txt

C:\Users\saqlain\training\work\hello>git status
On branch master
nothing to commit, working tree clean

C:\Users\saqlain\training\work\hello>ruby -v
'ruby' is not recognized as an internal or external command,
operable program or batch file.

### STAGING
C:\Users\saqlain\training\work\hello>git status
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)
        modified:   hello.txt

no changes added to commit (use "git add" and/or "git commit -a")

C:\Users\saqlain\training\work\hello>git add hello.txt

C:\Users\saqlain\training\work\hello>git status
On branch master
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)
        modified:   hello.txt

C:\Users\saqlain\training\work\hello>git status
On branch master
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)
        modified:   hello.txt

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        a.txt
        b.txt
        c.txt

C:\Users\saqlain\training\work\hello>git add a.txt

C:\Users\saqlain\training\work\hello>git add b.txt

### COMMITTING
C:\Users\saqlain\training\work\hello>git commit -m "Changes for a and b"
[master 95f9cae] Changes for a and b
 3 files changed, 3 insertions(+), 1 deletion(-)
 create mode 100644 a.txt
 create mode 100644 b.txt

C:\Users\saqlain\training\work\hello>git status
On branch master
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        c.txt

nothing added to commit but untracked files present (use "git add" to track)

C:\Users\saqlain\training\work\hello>git add c.txt

C:\Users\saqlain\training\work\hello>git commit -m "Changes for c"
[master 29d7d03] Changes for c
 1 file changed, 1 insertion(+)
 create mode 100644 c.txt

C:\Users\saqlain\training\work\hello>git commit
On branch master
nothing to commit, working tree clean

C:\Users\saqlain\training\work\hello>git add .

C:\Users\saqlain\training\work\hello>git status
On branch master
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)
        modified:   c.txt

C:\Users\saqlain\training\work\hello>git commit
[master edaa2aa] USING ARGV
 1 file changed, 1 insertion(+), 1 deletion(-)

C:\Users\saqlain\training\work\hello>git status
On branch master
nothing to commit, working tree clean

C:\Users\saqlain\training\work\hello>git add .

C:\Users\saqlain\training\work\hello>git status
On branch master
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)
        modified:   c.txt

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)
        modified:   c.txt

C:\Users\saqlain\training\work\hello>git commit -m "Added a default value"
[master df24d44] Added a default value
 1 file changed, 2 insertions(+), 1 deletion(-)

C:\Users\saqlain\training\work\hello>git status
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)
        modified:   c.txt

no changes added to commit (use "git add" and/or "git commit -a")

C:\Users\saqlain\training\work\hello>git add .

C:\Users\saqlain\training\work\hello>git status
On branch master
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)
        modified:   c.txt

C:\Users\saqlain\training\work\hello>git commit -m "Added the last line in another commit"
[master 4c4dde9] Added the last line in another commit
 1 file changed, 2 insertions(+), 1 deletion(-)

### HISTORY
C:\Users\saqlain\training\work\hello>git log --pretty=oneline
4c4dde94b04b02679598634a78ec3303769d469e (HEAD -> master) Added the last line in another commit
df24d44e803f0922602b437ae0ac5053a4acf0e2 Added a default value
edaa2aaa06ea4c73c79017f739bf7861aefeeb36 USING ARGV
29d7d039a9830e3f59317d23e97bb7e0f210d322 Changes for c
95f9caeb58cf786a33d74787fb3a2acc89d92d95 Changes for a and b
4b0a8745a25819224109b0bc352336d698ac52fe First commit lab3

C:\Users\saqlain\training\work\hello>git log --pretty=oneline --all
4c4dde94b04b02679598634a78ec3303769d469e (HEAD -> master) Added the last line in another commit
df24d44e803f0922602b437ae0ac5053a4acf0e2 Added a default value
edaa2aaa06ea4c73c79017f739bf7861aefeeb36 USING ARGV
29d7d039a9830e3f59317d23e97bb7e0f210d322 Changes for c
95f9caeb58cf786a33d74787fb3a2acc89d92d95 Changes for a and b
4b0a8745a25819224109b0bc352336d698ac52fe First commit lab3

C:\Users\saqlain\training\work\hello>

### ALIASES
C:\Users\saqlain\training\work\hello>git hist
4c4dde94b04b02679598634a78ec3303769d469e (HEAD -> master) Added the last line in another commit
df24d44e803f0922602b437ae0ac5053a4acf0e2 Added a default value
edaa2aaa06ea4c73c79017f739bf7861aefeeb36 USING ARGV
29d7d039a9830e3f59317d23e97bb7e0f210d322 Changes for c
95f9caeb58cf786a33d74787fb3a2acc89d92d95 Changes for a and b
4b0a8745a25819224109b0bc352336d698ac52fe First commit lab3

### OLD VERSIONS
C:\Users\saqlain\training\work\hello>git checkout 4b0a8745a25819224109b0bc352336d698ac52fe
Note: checking out '4b0a8745a25819224109b0bc352336d698ac52fe'.

You are in 'detached HEAD' state. You can look around, make experimental
changes and commit them, and you can discard any commits you make in this
state without impacting any branches by performing another checkout.

If you want to create a new branch to retain commits you create, you may
do so (now or later) by using -b with the checkout command again. Example:
 git checkout -b <new-branch-name>

HEAD is now at 4b0a874 First commit lab3

C:\Users\saqlain\training\work\hello>git checkout master
Previous HEAD position was 4b0a874 First commit lab3
Switched to branch 'master'

C:\Users\saqlain\training\work\hello>git hist
4c4dde94b04b02679598634a78ec3303769d469e (HEAD -> master) Added the last line in another commit
df24d44e803f0922602b437ae0ac5053a4acf0e2 Added a default value
edaa2aaa06ea4c73c79017f739bf7861aefeeb36 USING ARGV
29d7d039a9830e3f59317d23e97bb7e0f210d322 Changes for c
95f9caeb58cf786a33d74787fb3a2acc89d92d95 Changes for a and b
4b0a8745a25819224109b0bc352336d698ac52fe First commit lab3

### TAGGING
C:\Users\saqlain\training\work\hello>git tag v1

C:\Users\saqlain\training\work\hello>git checkout v1~1
Note: checking out 'v1~1'.

You are in 'detached HEAD' state. You can look around, make experimental
changes and commit them, and you can discard any commits you make in this
state without impacting any branches by performing another checkout.

If you want to create a new branch to retain commits you create, you may
do so (now or later) by using -b with the checkout command again. Example:
  git checkout -b <new-branch-name>

HEAD is now at df24d44 Added a default value

C:\Users\saqlain\training\work\hello>git hist
4c4dde94b04b02679598634a78ec3303769d469e (tag: v1, master) Added the last line in another commit
df24d44e803f0922602b437ae0ac5053a4acf0e2 (HEAD) Added a default value
edaa2aaa06ea4c73c79017f739bf7861aefeeb36 USING ARGV
29d7d039a9830e3f59317d23e97bb7e0f210d322 Changes for c
95f9caeb58cf786a33d74787fb3a2acc89d92d95 Changes for a and b
4b0a8745a25819224109b0bc352336d698ac52fe First commit lab3

C:\Users\saqlain\training\work\hello>git tag v1-beta

C:\Users\saqlain\training\work\hello>git checkout v1
Previous HEAD position was df24d44 Added a default value
HEAD is now at 4c4dde9 Added the last line in another commit

C:\Users\saqlain\training\work\hello>git checkout v1-beta
Previous HEAD position was 4c4dde9 Added the last line in another commit
HEAD is now at df24d44 Added a default value

C:\Users\saqlain\training\work\hello>git hist
4c4dde94b04b02679598634a78ec3303769d469e (tag: v1, master) Added the last line in another commit
df24d44e803f0922602b437ae0ac5053a4acf0e2 (HEAD, tag: v1-beta) Added a default value
edaa2aaa06ea4c73c79017f739bf7861aefeeb36 USING ARGV
29d7d039a9830e3f59317d23e97bb7e0f210d322 Changes for c
95f9caeb58cf786a33d74787fb3a2acc89d92d95 Changes for a and b
4b0a8745a25819224109b0bc352336d698ac52fe First commit lab3

C:\Users\saqlain\training\work\hello>git tag
v1
v1-beta

### UNDOING CHANGES IN STAGING AREA
C:\Users\saqlain\training\work\hello>git checkout master
Previous HEAD position was df24d44 Added a default value
Switched to branch 'master'

C:\Users\saqlain\training\work\hello>git status
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)
        modified:   hello.txt

no changes added to commit (use "git add" and/or "git commit -a")

C:\Users\saqlain\training\work\hello>git checkout hello.txt
Updated 1 path from the index

C:\Users\saqlain\training\work\hello>git status
On branch master
nothing to commit, working tree clean

### RESETTING COMMITS

C:\Users\saqlain\training\work\hello>git add hello.txt

C:\Users\saqlain\training\work\hello>git status
On branch master
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)
        modified:   hello.txt

C:\Users\saqlain\training\work\hello>git reset HEAD hello.txt
Unstaged changes after reset:
M       hello.txt

C:\Users\saqlain\training\work\hello>git checkout hello.txt
Updated 1 path from the index

C:\Users\saqlain\training\work\hello>git status
On branch master
nothing to commit, working tree clean

C:\Users\saqlain\training\work\hello>git add hello.txt

C:\Users\saqlain\training\work\hello>git commit -m "Commit by mistake"
On branch master
nothing to commit, working tree clean

C:\Users\saqlain\training\work\hello>git hist
4c4dde94b04b02679598634a78ec3303769d469e (HEAD -> master, tag: v1) Added the last line in another commit
df24d44e803f0922602b437ae0ac5053a4acf0e2 (tag: v1-beta) Added a default value
edaa2aaa06ea4c73c79017f739bf7861aefeeb36 USING ARGV
29d7d039a9830e3f59317d23e97bb7e0f210d322 Changes for c
95f9caeb58cf786a33d74787fb3a2acc89d92d95 Changes for a and b
4b0a8745a25819224109b0bc352336d698ac52fe First commit lab3

C:\Users\saqlain\training\work\hello>git add .

C:\Users\saqlain\training\work\hello>git commit -m "Commit by mistake"
[master 6bc6879] Commit by mistake
 1 file changed, 2 insertions(+), 1 deletion(-)

C:\Users\saqlain\training\work\hello>git revert HEAD
[master de339a5] Revert "Commit by mistake"
 1 file changed, 1 insertion(+), 2 deletions(-)

C:\Users\saqlain\training\work\hello>git hist
de339a513e91448a600a7b8cd4570bf4d57baad4 (HEAD -> master) Revert "Commit by mistake"
6bc6879f20b60109884e4001fd3551be7c80ecb6 Commit by mistake
4c4dde94b04b02679598634a78ec3303769d469e (tag: v1) Added the last line in another commit
df24d44e803f0922602b437ae0ac5053a4acf0e2 (tag: v1-beta) Added a default value
edaa2aaa06ea4c73c79017f739bf7861aefeeb36 USING ARGV
29d7d039a9830e3f59317d23e97bb7e0f210d322 Changes for c
95f9caeb58cf786a33d74787fb3a2acc89d92d95 Changes for a and b
4b0a8745a25819224109b0bc352336d698ac52fe First commit lab3

C:\Users\saqlain\training\work\hello>git tag oops

### HARD RESETTING COMMITS
C:\Users\saqlain\training\work\hello>git reset --hard v1
HEAD is now at 4c4dde9 Added the last line in another commit

C:\Users\saqlain\training\work\hello>git tag -d oops
Deleted tag 'oops' (was de339a5)

C:\Users\saqlain\training\work\hello>git hist --all
4c4dde94b04b02679598634a78ec3303769d469e (HEAD -> master, tag: v1) Added the last line in another commit
df24d44e803f0922602b437ae0ac5053a4acf0e2 (tag: v1-beta) Added a default value
edaa2aaa06ea4c73c79017f739bf7861aefeeb36 USING ARGV
29d7d039a9830e3f59317d23e97bb7e0f210d322 Changes for c
95f9caeb58cf786a33d74787fb3a2acc89d92d95 Changes for a and b
4b0a8745a25819224109b0bc352336d698ac52fe First commit lab3

### AMENDING
C:\Users\saqlain\training\work\hello>git add .

C:\Users\saqlain\training\work\hello>git commit -m "Add your name"
[master 6f3b9e4] Add your name
 1 file changed, 2 insertions(+), 1 deletion(-)

C:\Users\saqlain\training\work\hello>git add .

C:\Users\saqlain\training\work\hello>git status
On branch master
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)
        modified:   hello.txt

C:\Users\saqlain\training\work\hello>git commit --amend -m "Add your name/email"
[master 88a9eb7] Add your name/email
 Date: Tue Jun 18 16:46:45 2019 +0530
 1 file changed, 2 insertions(+), 1 deletion(-)

C:\Users\saqlain\training\work\hello>git hist
88a9eb767dbf518129b1fe156219ed9bd47d2a65 (HEAD -> master) Add your name/email
4c4dde94b04b02679598634a78ec3303769d469e (tag: v1) Added the last line in another commit
df24d44e803f0922602b437ae0ac5053a4acf0e2 (tag: v1-beta) Added a default value
edaa2aaa06ea4c73c79017f739bf7861aefeeb36 USING ARGV
29d7d039a9830e3f59317d23e97bb7e0f210d322 Changes for c
95f9caeb58cf786a33d74787fb3a2acc89d92d95 Changes for a and b
4b0a8745a25819224109b0bc352336d698ac52fe First commit lab3

### MOVING FILES
C:\Users\saqlain\training\work\hello>mkdir lib

C:\Users\saqlain\training\work\hello>git mv hello.txt lib

C:\Users\saqlain\training\work\hello>git status
On branch master
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)
        renamed:    hello.txt -> lib/hello.txt

C:\Users\saqlain\training\work\hello>git commit -m "Moved hello.txt to lib"
[master 62f92ae] Moved hello.txt to lib
 1 file changed, 0 insertions(+), 0 deletions(-)
 rename hello.txt => lib/hello.txt (100%)

C:\Users\saqlain\training\work\hello>git hist
62f92aed88ad45a74816caa580543a9bdc149dc4 (HEAD -> master) Moved hello.txt to lib
88a9eb767dbf518129b1fe156219ed9bd47d2a65 Add your name/email
4c4dde94b04b02679598634a78ec3303769d469e (tag: v1) Added the last line in another commit
df24d44e803f0922602b437ae0ac5053a4acf0e2 (tag: v1-beta) Added a default value
edaa2aaa06ea4c73c79017f739bf7861aefeeb36 USING ARGV
29d7d039a9830e3f59317d23e97bb7e0f210d322 Changes for c
95f9caeb58cf786a33d74787fb3a2acc89d92d95 Changes for a and b
4b0a8745a25819224109b0bc352336d698ac52fe First commit lab3

### OBJECTS
C:\Users\saqlain\training\work\hello>git cat-file -p 88a9eb767dbf518129b1fe156219ed9bd47d2a65
tree 1f539ee85f9bc74f891633af7ee3ed68e659f70a
parent 4c4dde94b04b02679598634a78ec3303769d469e
author Saqlain Kadiri <skadiri@tavisca.in> 1560856605 +0530
committer Saqlain Kadiri <skadiri@tavisca.in> 1560856767 +0530

Add your name/email

### BRANCHING
C:\Users\saqlain\training\work\hello>git add lib/rakefile.txt

C:\Users\saqlain\training\work\hello>git status
On branch greet
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)
        new file:   lib/rakefile.txt

C:\Users\saqlain\training\work\hello>git hist
* 428c614694b10ee19f2c0dda856d0263845af520 (HEAD -> greet) Hello updated after greet
* 57aff6c20f384d7fe3cc2698b47ee120d45b4d47 Added greet.txt
* 62f92aed88ad45a74816caa580543a9bdc149dc4 (master) Moved hello.txt to lib
* 88a9eb767dbf518129b1fe156219ed9bd47d2a65 Add your name/email
* 4c4dde94b04b02679598634a78ec3303769d469e (tag: v1) Added the last line in another commit
* df24d44e803f0922602b437ae0ac5053a4acf0e2 (tag: v1-beta) Added a default value
* edaa2aaa06ea4c73c79017f739bf7861aefeeb36 USING ARGV
* 29d7d039a9830e3f59317d23e97bb7e0f210d322 Changes for c
* 95f9caeb58cf786a33d74787fb3a2acc89d92d95 Changes for a and b
* 4b0a8745a25819224109b0bc352336d698ac52fe First commit lab3

C:\Users\saqlain\training\work\hello>git commit -m "Added rakefile"
[greet 93babe0] Added rakefile
 1 file changed, 1 insertion(+)
 create mode 100644 lib/rakefile.txt

C:\Users\saqlain\training\work\hello>git hist
* 93babe0072dbafe7f05aa9fd683b3a0cc5727912 (HEAD -> greet) Added rakefile
* 428c614694b10ee19f2c0dda856d0263845af520 Hello updated after greet
* 57aff6c20f384d7fe3cc2698b47ee120d45b4d47 Added greet.txt
* 62f92aed88ad45a74816caa580543a9bdc149dc4 (master) Moved hello.txt to lib
* 88a9eb767dbf518129b1fe156219ed9bd47d2a65 Add your name/email
* 4c4dde94b04b02679598634a78ec3303769d469e (tag: v1) Added the last line in another commit
* df24d44e803f0922602b437ae0ac5053a4acf0e2 (tag: v1-beta) Added a default value
* edaa2aaa06ea4c73c79017f739bf7861aefeeb36 USING ARGV
* 29d7d039a9830e3f59317d23e97bb7e0f210d322 Changes for c
* 95f9caeb58cf786a33d74787fb3a2acc89d92d95 Changes for a and b
* 4b0a8745a25819224109b0bc352336d698ac52fe First commit lab3

C:\Users\saqlain\training\work\hello>git checkout master
Switched to branch 'master'

C:\Users\saqlain\training\work\hello>git add lib/readme.txt

C:\Users\saqlain\training\work\hello>git commit -m "Added readme"
[master 4955398] Added readme
 1 file changed, 1 insertion(+)
 create mode 100644 lib/readme.txt

C:\Users\saqlain\training\work\hello>git hist
* 49553981e8cc0d40d650c4c309d3c690ef591a00 (HEAD -> master) Added readme
| * 93babe0072dbafe7f05aa9fd683b3a0cc5727912 (greet) Added rakefile
| * 428c614694b10ee19f2c0dda856d0263845af520 Hello updated after greet
| * 57aff6c20f384d7fe3cc2698b47ee120d45b4d47 Added greet.txt
|/
* 62f92aed88ad45a74816caa580543a9bdc149dc4 Moved hello.txt to lib
* 88a9eb767dbf518129b1fe156219ed9bd47d2a65 Add your name/email
* 4c4dde94b04b02679598634a78ec3303769d469e (tag: v1) Added the last line in another commit
* df24d44e803f0922602b437ae0ac5053a4acf0e2 (tag: v1-beta) Added a default value
* edaa2aaa06ea4c73c79017f739bf7861aefeeb36 USING ARGV
* 29d7d039a9830e3f59317d23e97bb7e0f210d322 Changes for c
* 95f9caeb58cf786a33d74787fb3a2acc89d92d95 Changes for a and b
* 4b0a8745a25819224109b0bc352336d698ac52fe First commit lab3

### MERGING BRANCHES
C:\Users\saqlain\training\work\hello>git checkout greet
Switched to branch 'greet'

C:\Users\saqlain\training\work\hello>git merge master
Merge made by the 'recursive' strategy.
 lib/readme.txt | 1 +
 1 file changed, 1 insertion(+)
 create mode 100644 lib/readme.txt

C:\Users\saqlain\training\work\hello>git hist
*   067b3f76216fa9551efcca79c4455db4f5e488d4 (HEAD -> greet) Merge branch 'master' into greet
|\
| * 49553981e8cc0d40d650c4c309d3c690ef591a00 (master) Added readme
* | 93babe0072dbafe7f05aa9fd683b3a0cc5727912 Added rakefile
* | 428c614694b10ee19f2c0dda856d0263845af520 Hello updated after greet
* | 57aff6c20f384d7fe3cc2698b47ee120d45b4d47 Added greet.txt
|/
* 62f92aed88ad45a74816caa580543a9bdc149dc4 Moved hello.txt to lib
* 88a9eb767dbf518129b1fe156219ed9bd47d2a65 Add your name/email
* 4c4dde94b04b02679598634a78ec3303769d469e (tag: v1) Added the last line in another commit
* df24d44e803f0922602b437ae0ac5053a4acf0e2 (tag: v1-beta) Added a default value
* edaa2aaa06ea4c73c79017f739bf7861aefeeb36 USING ARGV
* 29d7d039a9830e3f59317d23e97bb7e0f210d322 Changes for c
* 95f9caeb58cf786a33d74787fb3a2acc89d92d95 Changes for a and b
* 4b0a8745a25819224109b0bc352336d698ac52fe First commit lab3


### CREATING CONFLICT
C:\Users\saqlain\training\work\hello>git checkout master
Switched to branch 'master'

C:\Users\saqlain\training\work\hello>git hist
*   067b3f76216fa9551efcca79c4455db4f5e488d4 (greet) Merge branch 'master' into greet
|\
| * 49553981e8cc0d40d650c4c309d3c690ef591a00 (HEAD -> master) Added readme
* | 93babe0072dbafe7f05aa9fd683b3a0cc5727912 Added rakefile
* | 428c614694b10ee19f2c0dda856d0263845af520 Hello updated after greet
* | 57aff6c20f384d7fe3cc2698b47ee120d45b4d47 Added greet.txt
|/
* 62f92aed88ad45a74816caa580543a9bdc149dc4 Moved hello.txt to lib
* 88a9eb767dbf518129b1fe156219ed9bd47d2a65 Add your name/email
* 4c4dde94b04b02679598634a78ec3303769d469e (tag: v1) Added the last line in another commit
* df24d44e803f0922602b437ae0ac5053a4acf0e2 (tag: v1-beta) Added a default value
* edaa2aaa06ea4c73c79017f739bf7861aefeeb36 USING ARGV
* 29d7d039a9830e3f59317d23e97bb7e0f210d322 Changes for c
* 95f9caeb58cf786a33d74787fb3a2acc89d92d95 Changes for a and b
* 4b0a8745a25819224109b0bc352336d698ac52fe First commit lab3

C:\Users\saqlain\training\work\hello>git add hello.txt
fatal: pathspec 'hello.txt' did not match any files

C:\Users\saqlain\training\work\hello>git commit -m "Conflict created in hello.txt"
[master 1b9e08c] Conflict created in hello.txt
 1 file changed, 1 insertion(+), 1 deletion(-)

C:\Users\saqlain\training\work\hello>git hist
* 1b9e08c3f9e7f214479d81f4868eaa9899699b3f (HEAD -> master) Conflict created in hello.txt
| *   067b3f76216fa9551efcca79c4455db4f5e488d4 (greet) Merge branch 'master' into greet
| |\
| |/
|/|
* | 49553981e8cc0d40d650c4c309d3c690ef591a00 Added readme
| * 93babe0072dbafe7f05aa9fd683b3a0cc5727912 Added rakefile
| * 428c614694b10ee19f2c0dda856d0263845af520 Hello updated after greet
| * 57aff6c20f384d7fe3cc2698b47ee120d45b4d47 Added greet.txt
|/
* 62f92aed88ad45a74816caa580543a9bdc149dc4 Moved hello.txt to lib
* 88a9eb767dbf518129b1fe156219ed9bd47d2a65 Add your name/email
* 4c4dde94b04b02679598634a78ec3303769d469e (tag: v1) Added the last line in another commit
* df24d44e803f0922602b437ae0ac5053a4acf0e2 (tag: v1-beta) Added a default value
* edaa2aaa06ea4c73c79017f739bf7861aefeeb36 USING ARGV
* 29d7d039a9830e3f59317d23e97bb7e0f210d322 Changes for c
* 95f9caeb58cf786a33d74787fb3a2acc89d92d95 Changes for a and b
* 4b0a8745a25819224109b0bc352336d698ac52fe First commit lab3

C:\Users\saqlain\training\work\hello>git checkout greet
Switched to branch 'greet'

C:\Users\saqlain\training\work\hello>git merge master
Auto-merging lib/hello.txt
CONFLICT (content): Merge conflict in lib/hello.txt
Automatic merge failed; fix conflicts and then commit the result.

### RESOLVING CONFLICT
C:\Users\saqlain\training\work\hello>git add lib/hello.txt

C:\Users\saqlain\training\work\hello>git commit -m "Resolved Conflict manually"
[greet f356d7a] Resolved Conflict manually

C:\Users\saqlain\training\work\hello>git hist
*   f356d7a59744c51c139ff22f49bcdd2785333ff3 (HEAD -> greet) Resolved Conflict manually
|\
| * 1b9e08c3f9e7f214479d81f4868eaa9899699b3f (master) Conflict created in hello.txt
* |   067b3f76216fa9551efcca79c4455db4f5e488d4 Merge branch 'master' into greet
|\ \
| |/
| * 49553981e8cc0d40d650c4c309d3c690ef591a00 Added readme
* | 93babe0072dbafe7f05aa9fd683b3a0cc5727912 Added rakefile
* | 428c614694b10ee19f2c0dda856d0263845af520 Hello updated after greet
* | 57aff6c20f384d7fe3cc2698b47ee120d45b4d47 Added greet.txt
|/
* 62f92aed88ad45a74816caa580543a9bdc149dc4 Moved hello.txt to lib
* 88a9eb767dbf518129b1fe156219ed9bd47d2a65 Add your name/email
* 4c4dde94b04b02679598634a78ec3303769d469e (tag: v1) Added the last line in another commit
* df24d44e803f0922602b437ae0ac5053a4acf0e2 (tag: v1-beta) Added a default value
* edaa2aaa06ea4c73c79017f739bf7861aefeeb36 USING ARGV
* 29d7d039a9830e3f59317d23e97bb7e0f210d322 Changes for c
* 95f9caeb58cf786a33d74787fb3a2acc89d92d95 Changes for a and b
* 4b0a8745a25819224109b0bc352336d698ac52fe First commit lab3

### RESETTING BACK TO NO CONFLICTS
C:\Users\saqlain\training\work\hello>git hist
*   f356d7a59744c51c139ff22f49bcdd2785333ff3 (HEAD -> greet) Resolved Conflict manually
|\
| * 1b9e08c3f9e7f214479d81f4868eaa9899699b3f (master) Conflict created in hello.txt
* |   067b3f76216fa9551efcca79c4455db4f5e488d4 Merge branch 'master' into greet
|\ \
| |/
| * 49553981e8cc0d40d650c4c309d3c690ef591a00 Added readme
* | 93babe0072dbafe7f05aa9fd683b3a0cc5727912 Added rakefile
* | 428c614694b10ee19f2c0dda856d0263845af520 Hello updated after greet
* | 57aff6c20f384d7fe3cc2698b47ee120d45b4d47 Added greet.txt
|/
* 62f92aed88ad45a74816caa580543a9bdc149dc4 Moved hello.txt to lib
* 88a9eb767dbf518129b1fe156219ed9bd47d2a65 Add your name/email
* 4c4dde94b04b02679598634a78ec3303769d469e (tag: v1) Added the last line in another commit
* df24d44e803f0922602b437ae0ac5053a4acf0e2 (tag: v1-beta) Added a default value
* edaa2aaa06ea4c73c79017f739bf7861aefeeb36 USING ARGV
* 29d7d039a9830e3f59317d23e97bb7e0f210d322 Changes for c
* 95f9caeb58cf786a33d74787fb3a2acc89d92d95 Changes for a and b
* 4b0a8745a25819224109b0bc352336d698ac52fe First commit lab3

C:\Users\saqlain\training\work\hello>git reset --hard 93babe0072dbafe7f05aa9fd683b3a0cc5727912
HEAD is now at 93babe0 Added rakefile

C:\Users\saqlain\training\work\hello>git hist
* 1b9e08c3f9e7f214479d81f4868eaa9899699b3f (master) Conflict created in hello.txt
* 49553981e8cc0d40d650c4c309d3c690ef591a00 Added readme
| * 93babe0072dbafe7f05aa9fd683b3a0cc5727912 (HEAD -> greet) Added rakefile
| * 428c614694b10ee19f2c0dda856d0263845af520 Hello updated after greet
| * 57aff6c20f384d7fe3cc2698b47ee120d45b4d47 Added greet.txt
|/
* 62f92aed88ad45a74816caa580543a9bdc149dc4 Moved hello.txt to lib
* 88a9eb767dbf518129b1fe156219ed9bd47d2a65 Add your name/email
* 4c4dde94b04b02679598634a78ec3303769d469e (tag: v1) Added the last line in another commit
* df24d44e803f0922602b437ae0ac5053a4acf0e2 (tag: v1-beta) Added a default value
* edaa2aaa06ea4c73c79017f739bf7861aefeeb36 USING ARGV
* 29d7d039a9830e3f59317d23e97bb7e0f210d322 Changes for c
* 95f9caeb58cf786a33d74787fb3a2acc89d92d95 Changes for a and b
* 4b0a8745a25819224109b0bc352336d698ac52fe First commit lab3

C:\Users\saqlain\training\work\hello>git checkout master
Switched to branch 'master'

C:\Users\saqlain\training\work\hello>git reset --hard 49553981e8cc0d40d650c4c309d3c690ef591a00
HEAD is now at 4955398 Added readme

C:\Users\saqlain\training\work\hello>git checkout greet
Switched to branch 'greet'

C:\Users\saqlain\training\work\hello>git hist
* 49553981e8cc0d40d650c4c309d3c690ef591a00 (master) Added readme
| * 93babe0072dbafe7f05aa9fd683b3a0cc5727912 (HEAD -> greet) Added rakefile
| * 428c614694b10ee19f2c0dda856d0263845af520 Hello updated after greet
| * 57aff6c20f384d7fe3cc2698b47ee120d45b4d47 Added greet.txt
|/
* 62f92aed88ad45a74816caa580543a9bdc149dc4 Moved hello.txt to lib
* 88a9eb767dbf518129b1fe156219ed9bd47d2a65 Add your name/email
* 4c4dde94b04b02679598634a78ec3303769d469e (tag: v1) Added the last line in another commit
* df24d44e803f0922602b437ae0ac5053a4acf0e2 (tag: v1-beta) Added a default value
* edaa2aaa06ea4c73c79017f739bf7861aefeeb36 USING ARGV
* 29d7d039a9830e3f59317d23e97bb7e0f210d322 Changes for c
* 95f9caeb58cf786a33d74787fb3a2acc89d92d95 Changes for a and b
* 4b0a8745a25819224109b0bc352336d698ac52fe First commit lab3

### REBASING
C:\Users\saqlain\training\work\hello>git rebase master
First, rewinding head to replay your work on top of it...
Applying: Added greet.txt
Applying: Hello updated after greet
Applying: Added rakefile

C:\Users\saqlain\training\work\hello>git hist
* 0c5d8e972e27c6f7ee416a2e7018afb4b0ab1bca (HEAD -> greet) Added rakefile
* 175aa8b7f92733c0e01c2ef1d9c3463d326abd61 Hello updated after greet
* 586ffe2c901ac9c250563ad68eee2affe990fb6f Added greet.txt
* 49553981e8cc0d40d650c4c309d3c690ef591a00 (master) Added readme
* 62f92aed88ad45a74816caa580543a9bdc149dc4 Moved hello.txt to lib
* 88a9eb767dbf518129b1fe156219ed9bd47d2a65 Add your name/email
* 4c4dde94b04b02679598634a78ec3303769d469e (tag: v1) Added the last line in another commit
* df24d44e803f0922602b437ae0ac5053a4acf0e2 (tag: v1-beta) Added a default value
* edaa2aaa06ea4c73c79017f739bf7861aefeeb36 USING ARGV
* 29d7d039a9830e3f59317d23e97bb7e0f210d322 Changes for c
* 95f9caeb58cf786a33d74787fb3a2acc89d92d95 Changes for a and b
* 4b0a8745a25819224109b0bc352336d698ac52fe First commit lab3

C:\Users\saqlain\training\work\hello>git checkout master
Switched to branch 'master'

C:\Users\saqlain\training\work\hello>git merge greet
Updating 4955398..0c5d8e9
Fast-forward
 lib/greet.txt    | 1 +
 lib/hello.txt    | 2 +-
 lib/rakefile.txt | 1 +
 3 files changed, 3 insertions(+), 1 deletion(-)
 create mode 100644 lib/greet.txt
 create mode 100644 lib/rakefile.txt

C:\Users\saqlain\training\work\hello>git hist
* 0c5d8e972e27c6f7ee416a2e7018afb4b0ab1bca (HEAD -> master, greet) Added rakefile
* 175aa8b7f92733c0e01c2ef1d9c3463d326abd61 Hello updated after greet
* 586ffe2c901ac9c250563ad68eee2affe990fb6f Added greet.txt
* 49553981e8cc0d40d650c4c309d3c690ef591a00 Added readme
* 62f92aed88ad45a74816caa580543a9bdc149dc4 Moved hello.txt to lib
* 88a9eb767dbf518129b1fe156219ed9bd47d2a65 Add your name/email
* 4c4dde94b04b02679598634a78ec3303769d469e (tag: v1) Added the last line in another commit
* df24d44e803f0922602b437ae0ac5053a4acf0e2 (tag: v1-beta) Added a default value
* edaa2aaa06ea4c73c79017f739bf7861aefeeb36 USING ARGV
* 29d7d039a9830e3f59317d23e97bb7e0f210d322 Changes for c
* 95f9caeb58cf786a33d74787fb3a2acc89d92d95 Changes for a and b
* 4b0a8745a25819224109b0bc352336d698ac52fe First commit lab3

### REMOTE REPOSITORIES
C:\Users\saqlain\training\work>git clone hello cloned_hello

C:\Users\saqlain\training\work>cd cloned_hello

C:\Users\saqlain\training\work\cloned_hello>git hist
* 0c5d8e972e27c6f7ee416a2e7018afb4b0ab1bca (HEAD -> master, origin/master, origin/greet, origin/HEAD) Added rakefile
* 175aa8b7f92733c0e01c2ef1d9c3463d326abd61 Hello updated after greet
* 586ffe2c901ac9c250563ad68eee2affe990fb6f Added greet.txt
* 49553981e8cc0d40d650c4c309d3c690ef591a00 Added readme
* 62f92aed88ad45a74816caa580543a9bdc149dc4 Moved hello.txt to lib
* 88a9eb767dbf518129b1fe156219ed9bd47d2a65 Add your name/email
* 4c4dde94b04b02679598634a78ec3303769d469e (tag: v1) Added the last line in another commit
* df24d44e803f0922602b437ae0ac5053a4acf0e2 (tag: v1-beta) Added a default value
* edaa2aaa06ea4c73c79017f739bf7861aefeeb36 USING ARGV
* 29d7d039a9830e3f59317d23e97bb7e0f210d322 Changes for c
* 95f9caeb58cf786a33d74787fb3a2acc89d92d95 Changes for a and b
* 4b0a8745a25819224109b0bc352336d698ac52fe First commit lab3

C:\Users\saqlain\training\work\cloned_hello>git remote show origin
* remote origin
  Fetch URL: C:/Users/saqlain/training/work/hello
  Push  URL: C:/Users/saqlain/training/work/hello
  HEAD branch: master
  Remote branches:
    greet  tracked
    master tracked
  Local branch configured for 'git pull':
    master merges with remote master
  Local ref configured for 'git push':
    master pushes to master (up to date)

C:\Users\saqlain\training\work\cloned_hello>git branch -a
* master
  remotes/origin/HEAD -> origin/master
  remotes/origin/greet
  remotes/origin/master

C:\Users\saqlain\training\work\cloned_hello>cd ../hello

C:\Users\saqlain\training\work\hello>git add README

C:\Users\saqlain\training\work\hello>git commit -m "Changed README in original repo"
[master bda0f73] Changed README in original repo
 1 file changed, 1 insertion(+)
 create mode 100644 README

### FETCH AND MERGE
C:\Users\saqlain\training\work\hello>cd ../cloned_hello

C:\Users\saqlain\training\work\cloned_hello>git fetch
remote: Enumerating objects: 4, done.
remote: Counting objects: 100% (4/4), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 3 (delta 1), reused 0 (delta 0)
Unpacking objects: 100% (3/3), done.
From C:/Users/saqlain/training/work/hello
   0c5d8e9..bda0f73  master     -> origin/master

C:\Users\saqlain\training\work\cloned_hello>git hist --all
* bda0f7382b1ff10a2c0a0e1b8358e2c92499bbd1 (origin/master, origin/HEAD) Changed README in original repo
* 0c5d8e972e27c6f7ee416a2e7018afb4b0ab1bca (HEAD -> master, origin/greet) Added rakefile
* 175aa8b7f92733c0e01c2ef1d9c3463d326abd61 Hello updated after greet
* 586ffe2c901ac9c250563ad68eee2affe990fb6f Added greet.txt
* 49553981e8cc0d40d650c4c309d3c690ef591a00 Added readme
* 62f92aed88ad45a74816caa580543a9bdc149dc4 Moved hello.txt to lib
* 88a9eb767dbf518129b1fe156219ed9bd47d2a65 Add your name/email
* 4c4dde94b04b02679598634a78ec3303769d469e (tag: v1) Added the last line in another commit
* df24d44e803f0922602b437ae0ac5053a4acf0e2 (tag: v1-beta) Added a default value
* edaa2aaa06ea4c73c79017f739bf7861aefeeb36 USING ARGV
* 29d7d039a9830e3f59317d23e97bb7e0f210d322 Changes for c
* 95f9caeb58cf786a33d74787fb3a2acc89d92d95 Changes for a and b
* 4b0a8745a25819224109b0bc352336d698ac52fe First commit lab3

C:\Users\saqlain\training\work\cloned_hello>git merge origin/master
Updating 0c5d8e9..bda0f73
Fast-forward
 README | 1 +
 1 file changed, 1 insertion(+)
 create mode 100644 README

### TRACKING BRANCH
C:\Users\saqlain\training\work\cloned_hello>git branch --track greet origin/greet
Branch 'greet' set up to track remote branch 'greet' from 'origin'.

C:\Users\saqlain\training\work\cloned_hello>git branch -a
  greet
* master
  remotes/origin/HEAD -> origin/master
  remotes/origin/greet
  remotes/origin/master

C:\Users\saqlain\training\work\cloned_hello>git hist --max-count=2
* bda0f7382b1ff10a2c0a0e1b8358e2c92499bbd1 (HEAD -> master, origin/master, origin/HEAD) Changed README in original repo
* 0c5d8e972e27c6f7ee416a2e7018afb4b0ab1bca (origin/greet, greet) Added rakefile

### BARE REPOSITORY
C:\Users\saqlain\training\work\cloned_hello>cd ..

C:\Users\saqlain\training\work>git clone --bare hello hello.git
Cloning into bare repository 'hello.git'...
done.

C:\Users\saqlain\training\work>ls hello.git
'ls' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\saqlain\training\work>dir hello.git
 Volume in drive C has no label.
 Volume Serial Number is 30B0-B0C5

 Directory of C:\Users\saqlain\training\work\hello.git

19-06-2019  13:07    <DIR>          .
19-06-2019  13:07    <DIR>          ..
19-06-2019  13:07               166 config
19-06-2019  13:07                73 description
19-06-2019  13:07                23 HEAD
19-06-2019  13:07    <DIR>          hooks
19-06-2019  13:07    <DIR>          info
19-06-2019  13:07    <DIR>          objects
19-06-2019  13:07               276 packed-refs
19-06-2019  13:07    <DIR>          refs
               4 File(s)            538 bytes
               6 Dir(s)  1,034,662,391,808 bytes free

### ADDING A REMOTE REPO
C:\Users\saqlain\training\work>cd hello

C:\Users\saqlain\training\work\hello>git remote add shared ../hello.git
PUSHING A CHANGE
C:\Users\saqlain\training\work\hello>git add README

C:\Users\saqlain\training\work\hello>git commit -m "Updated readme to push a change"
[master f0a49f6] Updated readme to push a change
 1 file changed, 1 insertion(+), 1 deletion(-)

C:\Users\saqlain\training\work\hello>git push shared master
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 423 bytes | 211.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To ../hello.git
   bda0f73..f0a49f6  master -> master

### PULLING THE CHANGE
C:\Users\saqlain\training\work\hello>cd ../cloned_hello

C:\Users\saqlain\training\work\cloned_hello>git remote add shared ../hello.git

C:\Users\saqlain\training\work\cloned_hello>git branch --track shared master
Branch 'shared' set up to track local branch 'master'.

C:\Users\saqlain\training\work\cloned_hello>git pull shared master
From ../hello
 * branch            master     -> FETCH_HEAD
Updating bda0f73..f0a49f6
Fast-forward
 README | 2 +-
 1 file changed, 1 insertion(+), 1 deletion(-)

### HOSTING GIT REPOSITORIES
C:\Users\saqlain\training\work\cloned_hello>cd ..

C:\Users\saqlain\training\work>git daemon --verbose --export-all --base-path=.
[14124] Ready to rumble
[26520] Connection from [::1]:55926
[26520] unable to set SO_KEEPALIVE on socket: No such file or directory
[26520] Extended attribute "host": localhost
[26520] Request upload-pack for '/hello.git'



C:\Users\saqlain\training\work>git clone git://localhost/hello.git network_hello
Cloning into 'network_hello'...
remote: Enumerating objects: 48, done.
remote: Counting objects: 100% (48/48), done.
remote: Compressing objects: 100% (33/33), done.
remote: Total 48 (delta 9), reused 0 (delta 0)
Receiving objects: 100% (48/48), done.
Resolving deltas: 100% (9/9), done.

C:\Users\saqlain\training\work\network_hello>dir
 Volume in drive C has no label.
 Volume Serial Number is 30B0-B0C5

 Directory of C:\Users\saqlain\training\work\network_hello

19-06-2019  13:21    <DIR>          .
19-06-2019  13:21    <DIR>          ..
19-06-2019  13:21                 1 a.txt
19-06-2019  13:21                 1 b.txt
19-06-2019  13:21                28 c.txt
19-06-2019  13:21    <DIR>          lib
19-06-2019  13:21                52 README
               4 File(s)             82 bytes
               3 Dir(s)  1,034,660,519,936 bytes free
