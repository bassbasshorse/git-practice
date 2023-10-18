# Git config


### **First - time setup**
1. System level: --system option. Affects all uses and repositories on the system (administrative)
    file: /etc/gitconfig
2. Global (user) level: --global option. Affects all repositories of a current user
    file: ~/.config/git/config
3. Local level: --local option. Specific to the current repository
    file: .git/gitconfig    
* each level overrides values in the previous level: system -> global -> local
* git config (-- list or --list --show-origin) 

git init : creat git 
git status : show git file status
git add : add staging area
git rm --cached : delete staging area file
### **.gitignore file**
- *.a : ignore all .a files
- !lib.a : but do track lib.a, even though you're ignoring .a files above
- /T0D0 : only ignore the T0D0 file in the current directory, not subdir /T0D0
- build/ ignore all files in any directory named build
- doc/*.txt : ignore doc/notes.txt, but not doc/server/arch.txt
- doc/ \** /*.pdf : ignore all .pdf files in the doc/ directory and any of its subdirectories

git commit -m "commit message" : commit git such snapshot
git branch -m master main : change branch name -m -> main
