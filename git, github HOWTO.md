# `Github`
<br>

## Clone

### 1) clone a branch 
clone using `download ZIP` kita cuma dapat branch yg kita download tu shj  
clone main branch or branch2 lain, sama je cara dia. 

https://github.com/taqinasirr/kod/assets/21170527/6107f090-380f-4229-8f17-8b624591e97f

### 2) clone a repository

step
* copylinkremote
* git clone pastelinkremote


clone using command `git clone` kita dapat clone a repository. so dapat semua branch

`git branch`    show local (current) branch  
`git branch -r`   show all remote branches  
`git branch -a` show local (current) branch and all remote branches

`git checkout namaBranch`    utk checkout to that branch

<br>

> local folder yg di clone tu automatic dah set origin sebgai alias kpd remote. so takyah `git remote add origin linkremote`

https://github.com/taqinasirr/kod/assets/21170527/f97b7810-f3c8-45fc-aa38-695de8b5b38f


<br>

## Repository

### 1) drag n drop local files to github repo

step
* create repo
* drag n drop
* commit

https://github.com/taqinasirr/kod/assets/21170527/0d4b585f-e4c7-433b-b697-959a61abba77

### 2) push local files to repo pakai vscode

step
* create repo
* git init
* git remote add origin linkremote
* commit changes
* push local files to repo

https://github.com/taqinasirr/kod/assets/21170527/82ef6b4d-4ace-4bf0-8d57-e33ac50eba71

### 3) delete repo

https://github.com/taqinasirr/kod/assets/21170527/23e07794-cc03-4329-a0d4-14159496db9d



<br><br>

# `VS Code`

<br>

boleh terus commit.  
vscode sendiri yg akan add untracked files to staging area


> Untracked files - files yg takdak kat staging area. (git tak tau dia wujud)  
> tracked files - files yg ada kat staging area. (git tau dia wujud)



https://github.com/taqinasirr/kod/assets/21170527/6776a90b-8d36-4d23-9e62-fca408f53a21

<br>

synchronize changes = apa yg ada kat branch remote sebijik mcm apa yg ada kat branch local.    
berlaku pull & push  
1. pull remote changes down to your local repo
2. push local commits to remote

https://github.com/taqinasirr/kod/assets/21170527/1f3af76e-bd6a-4404-96f8-ff34d1710911

<br>

commit options

<img src = "https://github.com/taqinasirr/kod/assets/21170527/23c97d74-ebd5-4cec-8306-cd5d3a39e59c" width="500">

<br><br>

Git commands

https://github.com/taqinasirr/kod/assets/21170527/ab90bb15-c746-4bf4-8a4a-7aeb4a0b9223






# `Git`
commit 10 kali, maksudnya u ada 10 files.
cuma files ni dlm bentuk commit lah.
u can jump to any commit


git log
git log --oneline
git checkout
git chaeckout namaBranch   go to lastest commit pada branch tree

cth ada 5 commit  
chekcout to 1st commit, bila git log, dia hanya tunjuk 1 commit je. sebab waktu tu belum 5 commit.  
so utk ke commit ke 5, pakai git checkout namaBranch






