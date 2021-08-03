```bash

beoo@DESKTOP-L7L23IA MINGW64 ~
$ git config --list

diff.astextplain.textconv=astextplain
filter.lfs.clean=git-lfs clean -- %f
filter.lfs.smudge=git-lfs smudge -- %f
filter.lfs.process=git-lfs filter-process
filter.lfs.required=true
http.sslbackend=openssl
http.sslcainfo=C:/Program Files/Git/mingw64/ssl/certs/ca-bundle.crt
core.autocrlf=true
core.fscache=true
core.symlinks=false
pull.rebase=false
credential.https://dev.azure.com.usehttppath=true
init.defaultbranch=master
filter.lfs.required=true
filter.lfs.clean=git-lfs clean -- %f
filter.lfs.smudge=git-lfs smudge -- %f
filter.lfs.process=git-lfs filter-process
user.name=Esanov Otabek
user.email=esanovotabek688@gmail.com

beoo@DESKTOP-L7L23IA MINGW64 ~
$ git config user
error: key does not contain a section: user

beoo@DESKTOP-L7L23IA MINGW64 ~
$ git config user.name
Esanov Otabek

beoo@DESKTOP-L7L23IA MINGW64 ~
$ git config user.email
esanovotabek688@gmail.com

beoo@DESKTOP-L7L23IA MINGW64 ~
$ git config user.password

beoo@DESKTOP-L7L23IA MINGW64 ~
$ cd desktop

beoo@DESKTOP-L7L23IA MINGW64 ~/desktop
$ cd github

beoo@DESKTOP-L7L23IA MINGW64 ~/desktop/github
$ git init
Initialized empty Git repository in C:/Users/beoo/Desktop/github/.git/

beoo@DESKTOP-L7L23IA MINGW64 ~/desktop/github (master)
$ git add readme.md

beoo@DESKTOP-L7L23IA MINGW64 ~/desktop/github (master)
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   readme.md


beoo@DESKTOP-L7L23IA MINGW64 ~/desktop/github (master)
$ git commit -m "first commit"
[master (root-commit) dc9aae3] first commit
 1 file changed, 69 insertions(+)
 create mode 100644 readme.md

beoo@DESKTOP-L7L23IA MINGW64 ~/desktop/github (master)
$ git branch -M main

beoo@DESKTOP-L7L23IA MINGW64 ~/desktop/github (main)
$ git remote add origin https://github.com/EsanovOtabek/github.git

beoo@DESKTOP-L7L23IA MINGW64 ~/desktop/github (main)
$ git push -u origin main
To https://github.com/EsanovOtabek/github.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/EsanovOtabek/github.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

beoo@DESKTOP-L7L23IA MINGW64 ~/desktop/github (main)
$ git push -u origin main
To https://github.com/EsanovOtabek/github.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/EsanovOtabek/github.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

beoo@DESKTOP-L7L23IA MINGW64 ~/desktop/github (main)
$ git pull -u origin main
error: unknown switch `u'
usage: git pull [<options>] [<repository> [<refspec>...]]

    -v, --verbose         be more verbose
    -q, --quiet           be more quiet
    --progress            force progress reporting
    --recurse-submodules[=<on-demand>]
                          control for recursive fetching of submodules

Options related to merging
    -r, --rebase[=(false|true|merges|preserve|interactive)]
                          incorporate changes by rebasing rather than merging
    -n                    do not show a diffstat at the end of the merge
    --stat                show a diffstat at the end of the merge
    --log[=<n>]           add (at most <n>) entries from shortlog to merge commi
                                                                               it message
    --signoff[=...]       add a Signed-off-by trailer
    --squash              create a single commit instead of doing a merge
    --commit              perform a commit if the merge succeeds (default)
    --edit                edit message before committing
    --cleanup <mode>      how to strip spaces and #comments from message
    --ff                  allow fast-forward
    --ff-only             abort if fast-forward is not possible
    --verify-signatures   verify that the named commit has a valid GPG signature
                                                                               e

    --autostash           automatically stash/stash pop before and after
    -s, --strategy <strategy>
                          merge strategy to use
    -X, --strategy-option <option=value>
                          option for selected merge strategy
    -S, --gpg-sign[=<key-id>]
                          GPG sign commit
    --allow-unrelated-histories
                          allow merging unrelated histories

Options related to fetching
    --all                 fetch from all remotes
    -a, --append          append to .git/FETCH_HEAD instead of overwriting
    --upload-pack <path>  path to upload pack on remote end
    -f, --force           force overwrite of local branch
    -t, --tags            fetch all tags and associated objects
    -p, --prune           prune remote-tracking branches no longer on remote
    -j, --jobs[=<n>]      number of submodules pulled in parallel
    --dry-run             dry run
    -k, --keep            keep downloaded pack
    --depth <depth>       deepen history of shallow clone
    --shallow-since <time>
                          deepen history of shallow repository based on time
    --shallow-exclude <revision>
                          deepen history of shallow clone, excluding rev
    --deepen <n>          deepen history of shallow clone
    --unshallow           convert to a complete repository
    --update-shallow      accept refs that update .git/shallow
    --refmap <refmap>     specify fetch refmap
    -o, --server-option <server-specific>
                          option to transmit
    -4, --ipv4            use IPv4 addresses only
    -6, --ipv6            use IPv6 addresses only
    --negotiation-tip <revision>
                          report that we have only objects reachable from this o
                                                                               object
    --show-forced-updates
                          check for forced-updates on all updated branches
    --set-upstream        set upstream for git pull/fetch


beoo@DESKTOP-L7L23IA MINGW64 ~/desktop/github (main)
$ git pull -a origin main
remote: Enumerating objects: 6, done.
remote: Counting objects: 100% (6/6), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 6 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (6/6), 1.18 KiB | 2.00 KiB/s, done.
From https://github.com/EsanovOtabek/github
 * branch            main       -> FETCH_HEAD
 * [new branch]      main       -> origin/main
fatal: refusing to merge unrelated histories

beoo@DESKTOP-L7L23IA MINGW64 ~/desktop/github (main)
$ git checkout -- readme.md

beoo@DESKTOP-L7L23IA MINGW64 ~/desktop/github (main)
$ git status
On branch main
nothing to commit, working tree clean

beoo@DESKTOP-L7L23IA MINGW64 ~/desktop/github (main)
$ git status
On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   readme.md

no changes added to commit (use "git add" and/or "git commit -a")

beoo@DESKTOP-L7L23IA MINGW64 ~/desktop/github (main)
$ ^

```