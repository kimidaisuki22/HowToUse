# Git

## install Git

## config Git

refrence: https://ocw.mit.edu/ans7870/6/6.005/s16/getting-started/index.html#config-git
<br>
set user name: ` git config --global user.name "kixxxx" ` 
<br>
set user mail: ` git config --global user.mail sona@ki.com `
<br>
set editor: `git config --global core.editor vim`
<br>
add color: <br>
`git config --global color.branch auto` <br>
`git config --global color.diff auto` <br>
`git config --global color.interactive auto`<br>
`git config --global color.status auto `<br>
`git config --global color.grep auto `<br>

### alias 
`git config --global alias.loglite "log --graph --oneline --decorate --color --all"`
`git loglite`

### config file

## add file to stage
`git add filename`
`git add .`
## show status
` git status`

## show different

### show no staged file
`git diff`
### show staged file
`git diff --staged`

## commit 

`git commit`

## push
` git push origin main`
origin is remote repository
main is you local repo
## merge

## pull
update local repo
