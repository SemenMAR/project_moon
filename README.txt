
admin@DESKTOP-IE83URQ MINGW64 ~
$ git config --global
usage: git config [<options>]

Config file location
    --[no-]global         use global config file
    --[no-]system         use system config file
    --[no-]local          use repository config file
    --[no-]worktree       use per-worktree config file
    -f, --[no-]file <file>
                          use given config file
    --[no-]blob <blob-id> read config from given blob object

Action
    --[no-]get            get value: name [value-pattern]
    --[no-]get-all        get all values: key [value-pattern]
    --[no-]get-regexp     get values for regexp: name-regex [value-pat
    --[no-]get-urlmatch   get value specific for the URL: section[.var
    --[no-]replace-all    replace all matching variables: name value [ern]
    --[no-]add            add a new variable: name value
    --[no-]unset          remove a variable: name [value-pattern]
    --[no-]unset-all      remove all matches: name [value-pattern]
    --[no-]rename-section rename section: old-name new-name
    --[no-]remove-section remove a section: name
    -l, --[no-]list       list all
    --[no-]fixed-value    use string equality when comparing values tottern'
    -e, --[no-]edit       open an editor
    --[no-]get-color      find the color configured: slot [default]
    --[no-]get-colorbool  find the color setting: slot [stdout-is-tty]

Type
    -t, --[no-]type <type>
                          value is given this type
    --bool                value is "true" or "false"
    --int                 value is decimal number
    --bool-or-int         value is --bool or --int
    --bool-or-str         value is --bool or string
    --path                value is a path (file or directory name)
    --expiry-date         value is an expiry date

Other
    -z, --[no-]null       terminate values with NUL byte
    --[no-]name-only      show variable names only
    --[no-]includes       respect include directives on lookup
    --[no-]show-origin    show origin of config (file, standard input,mand line)
    --[no-]show-scope     show scope of config (worktree, local, globa command)
    --[no-]default <value>
                          with --get, use default value when missing e


admin@DESKTOP-IE83URQ MINGW64 ~
$ git config --global user.name "Semyon Martinovich"

admin@DESKTOP-IE83URQ MINGW64 ~
$ git config --global user.email "semmartin71@gmail.com"

admin@DESKTOP-IE83URQ MINGW64 ~
$ cd C:\Users\admin\Desktop\CS\2023project1
bash: cd: C:UsersadminDesktopCS2023project1: No such file or directory

admin@DESKTOP-IE83URQ MINGW64 ~
$ cd 2023project1
bash: cd: 2023project1: No such file or directory

admin@DESKTOP-IE83URQ MINGW64 ~
$ cd C:/Users/admin/Desktop/CS/2023project1

admin@DESKTOP-IE83URQ MINGW64 ~/Desktop/CS/2023project1
$ git init
Initialized empty Git repository in C:/Users/admin/Desktop/CS/2023proj

admin@DESKTOP-IE83URQ MINGW64 ~/Desktop/CS/2023project1 (master)
$ git remote add origin https://github.com/SemenMAR/project_moon

admin@DESKTOP-IE83URQ MINGW64 ~/Desktop/CS/2023project1 (master)
$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.txt

nothing added to commit but untracked files present (use "git add" to

admin@DESKTOP-IE83URQ MINGW64 ~/Desktop/CS/2023project1 (master)
$ git add .

admin@DESKTOP-IE83URQ MINGW64 ~/Desktop/CS/2023project1 (master)
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   README.txt


admin@DESKTOP-IE83URQ MINGW64 ~/Desktop/CS/2023project1 (master)
$ git commit -m
error: switch `m' requires a value

admin@DESKTOP-IE83URQ MINGW64 ~/Desktop/CS/2023project1 (master)
$ git commit -m "Readme 1 update"
[master (root-commit) aad2d71] Readme 1 update
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 README.txt

admin@DESKTOP-IE83URQ MINGW64 ~/Desktop/CS/2023project1 (master)
$ git add .

admin@DESKTOP-IE83URQ MINGW64 ~/Desktop/CS/2023project1 (master)
$ git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   README.txt


admin@DESKTOP-IE83URQ MINGW64 ~/Desktop/CS/2023project1 (master)
$ git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   README.txt

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory
        modified:   README.txt


admin@DESKTOP-IE83URQ MINGW64 ~/Desktop/CS/2023project1 (master)
$ git add .

admin@DESKTOP-IE83URQ MINGW64 ~/Desktop/CS/2023project1 (master)
$ git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   README.txt


admin@DESKTOP-IE83URQ MINGW64 ~/Desktop/CS/2023project1 (master)
$ git commid -m "readme 2 update"
git: 'commid' is not a git command. See 'git --help'.

The most similar command is
        commit

admin@DESKTOP-IE83URQ MINGW64 ~/Desktop/CS/2023project1 (master)
$ git commit -m "readme 2 update"
[master c398730] readme 2 update
 1 file changed, 1 insertion(+)

admin@DESKTOP-IE83URQ MINGW64 ~/Desktop/CS/2023project1 (master)
$ git log
commit c398730d68681076fdaedc0464b991e29ff476b7 (HEAD -> master)
Author: Semyon Martinovich <semmartin71@gmail.com>
Date:   Thu Nov 30 13:47:04 2023 +0300

    readme 2 update

commit aad2d7144b4228d65bb9682d8296075c8654cf26
Author: Semyon Martinovich <semmartin71@gmail.com>
Date:   Thu Nov 30 13:41:54 2023 +0300

    Readme 1 update

admin@DESKTOP-IE83URQ MINGW64 ~/Desktop/CS/2023project1 (master)
$ git checkout ^C

admin@DESKTOP-IE83URQ MINGW64 ~/Desktop/CS/2023project1 (master)
$ git checkout aad2d7144b4228d65bb9682d8296075c8654cf26
Note: switching to 'aad2d7144b4228d65bb9682d8296075c8654cf26'.

You are in 'detached HEAD' state. You can look around, make experiment
changes and commit them, and you can discard any commits you make in t
state without impacting any branches by switching back to a branch.

If you want to create a new branch to retain commits you create, you m
do so (now or later) by using -c with the switch command. Example:

  git switch -c <new-branch-name>

Or undo this operation with:

  git switch -

Turn off this advice by setting config variable advice.detachedHead to

HEAD is now at aad2d71 Readme 1 update

admin@DESKTOP-IE83URQ MINGW64 ~/Desktop/CS/2023project1 ((aad2d71...))
$ git add README.txt

admin@DESKTOP-IE83URQ MINGW64 ~/Desktop/CS/2023project1 ((aad2d71...))
$ git commit -m "readme 3 update"
[detached HEAD f3dbe52] readme 3 update
 1 file changed, 1 insertion(+)

admin@DESKTOP-IE83URQ MINGW64 ~/Desktop/CS/2023project1 ((f3dbe52...))
$ git log
commit f3dbe52c66c5601a1a6be4f5405b2e27356acc33 (HEAD)
Author: Semyon Martinovich <semmartin71@gmail.com>
Date:   Thu Nov 30 13:50:30 2023 +0300

    readme 3 update

commit aad2d7144b4228d65bb9682d8296075c8654cf26
Author: Semyon Martinovich <semmartin71@gmail.com>
Date:   Thu Nov 30 13:41:54 2023 +0300

    Readme 1 update

admin@DESKTOP-IE83URQ MINGW64 ~/Desktop/CS/2023project1 ((f3dbe52...))
$ git push origin
fatal: You are not currently on a branch.
To push the history leading to the current (detached HEAD)
state now, use

    git push origin HEAD:<name-of-remote-branch>


admin@DESKTOP-IE83URQ MINGW64 ~/Desktop/CS/2023project1 ((f3dbe52...))
$ git push origin master
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 12 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (6/6), 461 bytes | 461.00 KiB/s, done.
Total 6 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/SemenMAR/project_moon
 * [new branch]      master -> master

admin@DESKTOP-IE83URQ MINGW64 ~/Desktop/CS/2023project1 ((f3dbe52...))
$ git branch
* (HEAD detached from aad2d71)
  master

admin@DESKTOP-IE83URQ MINGW64 ~/Desktop/CS/2023project1 ((f3dbe52...))
$ git branch feature

admin@DESKTOP-IE83URQ MINGW64 ~/Desktop/CS/2023project1 ((f3dbe52...))
$ git branch
* (HEAD detached from aad2d71)
  feature
  master

admin@DESKTOP-IE83URQ MINGW64 ~/Desktop/CS/2023project1 ((f3dbe52...))
$ git checkout feature
Switched to branch 'feature'

admin@DESKTOP-IE83URQ MINGW64 ~/Desktop/CS/2023project1 (feature)
$ git branch
* feature
  master

admin@DESKTOP-IE83URQ MINGW64 ~/Desktop/CS/2023project1 (feature)
$ git checkout master
Switched to branch 'master'

admin@DESKTOP-IE83URQ MINGW64 ~/Desktop/CS/2023project1 (master)
$ git checkout feature
Switched to branch 'feature'

admin@DESKTOP-IE83URQ MINGW64 ~/Desktop/CS/2023project1 (feature)
$ git origin feature
git: 'origin' is not a git command. See 'git --help'.

admin@DESKTOP-IE83URQ MINGW64 ~/Desktop/CS/2023project1 (feature)
$ git push origin feature
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Writing objects: 100% (3/3), 262 bytes | 262.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'feature' on GitHub by visiting:
remote:      https://github.com/SemenMAR/project_moon/pull/new/feature
remote:
To https://github.com/SemenMAR/project_moon
 * [new branch]      feature -> feature

admin@DESKTOP-IE83URQ MINGW64 ~/Desktop/CS/2023project1 (feature)
$ git branch
* feature
  master

admin@DESKTOP-IE83URQ MINGW64 ~/Desktop/CS/2023project1 (feature)
$ git checkout master
Switched to branch 'master'

admin@DESKTOP-IE83URQ MINGW64 ~/Desktop/CS/2023project1 (master)
$ git merge feature
Auto-merging README.txt
CONFLICT (content): Merge conflict in README.txt
Automatic merge failed; fix conflicts and then commit the result.

admin@DESKTOP-IE83URQ MINGW64 ~/Desktop/CS/2023project1 (master|MERGING)
$ git log
commit c398730d68681076fdaedc0464b991e29ff476b7 (HEAD -> master, origin/master)
Author: Semyon Martinovich <semmartin71@gmail.com>
Date:   Thu Nov 30 13:47:04 2023 +0300

    readme 2 update

commit aad2d7144b4228d65bb9682d8296075c8654cf26
Author: Semyon Martinovich <semmartin71@gmail.com>
Date:   Thu Nov 30 13:41:54 2023 +0300

    Readme 1 update

admin@DESKTOP-IE83URQ MINGW64 ~/Desktop/CS/2023project1 (master|MERGING)
