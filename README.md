# gitDemo_82


CSE-KUETs-iMac:~ cse_kuet$ git clone https://github.com/himel99/gitDemo_82.git
Cloning into 'gitDemo_82'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), done.
CSE-KUETs-iMac:~ cse_kuet$ pwd
/Users/cse_kuet
CSE-KUETs-iMac:~ cse_kuet$ cd gitDemo_82
CSE-KUETs-iMac:gitDemo_82 cse_kuet$ ls
LICENSE
CSE-KUETs-iMac:gitDemo_82 cse_kuet$ echo "# gitDemo_82" >> README.md
CSE-KUETs-iMac:gitDemo_82 cse_kuet$ ls
LICENSE		README.md
CSE-KUETs-iMac:gitDemo_82 cse_kuet$ cat README.md
# gitDemo_82
CSE-KUETs-iMac:gitDemo_82 cse_kuet$ ls -a
.		..		.git		LICENSE		README.md
CSE-KUETs-iMac:gitDemo_82 cse_kuet$ git add readme.md
CSE-KUETs-iMac:gitDemo_82 cse_kuet$ git status
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)

	README.md

nothing added to commit but untracked files present (use "git add" to track)
CSE-KUETs-iMac:gitDemo_82 cse_kuet$ git commit readme.md -m "add readme file"
error: pathspec 'readme.md' did not match any file(s) known to git.
CSE-KUETs-iMac:gitDemo_82 cse_kuet$ git add README.md
CSE-KUETs-iMac:gitDemo_82 cse_kuet$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

	new file:   README.md

CSE-KUETs-iMac:gitDemo_82 cse_kuet$ git commit README.md -m "add readme file"
[main cc55df3] add readme file
 1 file changed, 1 insertion(+)
 create mode 100644 README.md
CSE-KUETs-iMac:gitDemo_82 cse_kuet$ git status
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
CSE-KUETs-iMac:gitDemo_82 cse_kuet$ git push origin main
Username for 'https://github.com': himel99
Password for 'https://himel99@github.com': 
remote: Support for password authentication was removed on August 13, 2021. Please use a personal access token instead.
remote: Please see https://github.blog/2020-12-15-token-authentication-requirements-for-git-operations/ for more information.
fatal: Authentication failed for 'https://github.com/himel99/gitDemo_82.git/'
CSE-KUETs-iMac:gitDemo_82 cse_kuet$ git push origin main
Username for 'https://github.com': himel99
Password for 'https://himel99@github.com': 
remote: Support for password authentication was removed on August 13, 2021. Please use a personal access token instead.
remote: Please see https://github.blog/2020-12-15-token-authentication-requirements-for-git-operations/ for more information.
fatal: Authentication failed for 'https://github.com/himel99/gitDemo_82.git/'
CSE-KUETs-iMac:gitDemo_82 cse_kuet$ git push -u origin main
Username for 'https://github.com': himel99
Password for 'https://himel99@github.com': 
remote: Support for password authentication was removed on August 13, 2021. Please use a personal access token instead.
remote: Please see https://github.blog/2020-12-15-token-authentication-requirements-for-git-operations/ for more information.
fatal: Authentication failed for 'https://github.com/himel99/gitDemo_82.git/'
CSE-KUETs-iMac:gitDemo_82 cse_kuet$ gitk --all
DEPRECATION WARNING: The system version of Tk is deprecated and may be removed in a future release. Please don't rely on it. Set TK_SILENCE_DEPRECATION=1 to suppress this warning.
    
^Z
[1]+  Stopped                 gitk --all
CSE-KUETs-iMac:gitDemo_82 cse_kuet$ git log
commit cc55df368659bb0be51d14741914cf16ea1074bc (HEAD -> main)
Author: Rahat Mahmud Khan <rahat.rmk462@gmail.com>
Date:   Thu Nov 11 11:55:22 2021 +0600

    add readme file

commit 217d807bd84fbdbee0f86dd8c39fd72fb08e3063 (origin/main, origin/HEAD)
Author: Asiful Islam Himel <42843551+himel99@users.noreply.github.com>
Date:   Thu Nov 11 11:46:08 2021 +0600

    Initial commit
CSE-KUETs-iMac:gitDemo_82 cse_kuet$ git branch -a
* main
  remotes/origin/HEAD -> origin/main
  remotes/origin/main
CSE-KUETs-iMac:gitDemo_82 cse_kuet$ git branch -a
* main
  remotes/origin/HEAD -> origin/main
  remotes/origin/main
CSE-KUETs-iMac:gitDemo_82 cse_kuet$ touch db1.txt
CSE-KUETs-iMac:gitDemo_82 cse_kuet$ git branch -a database
fatal: -a and -r options to 'git branch' do not make sense with a branch name
CSE-KUETs-iMac:gitDemo_82 cse_kuet$ git branch database
CSE-KUETs-iMac:gitDemo_82 cse_kuet$ git checkout main
Already on 'main'
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)
CSE-KUETs-iMac:gitDemo_82 cse_kuet$ git checkout database
Switched to branch 'database'
CSE-KUETs-iMac:gitDemo_82 cse_kuet$ git add .
CSE-KUETs-iMac:gitDemo_82 cse_kuet$ git push origin database
Username for 'https://github.com': himel99
Password for 'https://himel99@github.com': 
remote: Support for password authentication was removed on August 13, 2021. Please use a personal access token instead.
remote: Please see https://github.blog/2020-12-15-token-authentication-requirements-for-git-operations/ for more information.
fatal: Authentication failed for 'https://github.com/himel99/gitDemo_82.git/'
CSE-KUETs-iMac:gitDemo_82 cse_kuet$ gitk --all
DEPRECATION WARNING: The system version of Tk is deprecated and may be removed in a future release. Please don't rely on it. Set TK_SILENCE_DEPRECATION=1 to suppress this warning.

