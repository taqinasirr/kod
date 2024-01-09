# `Github`
<br>  

## Clone

### 1) Clone a branch using `download ZIP`
clone using `download ZIP` kita cuma dapat branch yg kita download tu shj. sebab x pakai git  
clone main branch or branch2 lain, sama je cara dia. 

https://github.com/taqinasirr/kod/assets/21170527/6107f090-380f-4229-8f17-8b624591e97f

### 2) Clone a repository using `git clone`

step
* copylinkremote
* git clone pastelinkremote


clone using command `git clone` kita dapat clone a repository. so dapat semua branch

`git branch`    show local (current) branch  
`git branch -r`   show all remote branches  
`git branch -a` show local (current) branch and all remote branches

`git checkout namaBranch`    utk checkout to that branch

<br>

> *local folder yg di clone tu automatic dah set origin sebgai alias kpd remote. so takyah `git remote add origin linkremote`*

https://github.com/taqinasirr/kod/assets/21170527/f97b7810-f3c8-45fc-aa38-695de8b5b38f


<br>

## Repository

### 1) Drag n drop local files to github repo

step
* create repo
* drag n drop
* commit

https://github.com/taqinasirr/kod/assets/21170527/0d4b585f-e4c7-433b-b697-959a61abba77

### 2) Push local files to remote pakai vscode

step
* create repo
* git init
* git remote add origin linkremote
* commit changes
* push local files to romote

 > *remote = online repo. dlm kes ni, remote = github repo*
 

https://github.com/taqinasirr/kod/assets/21170527/82ef6b4d-4ace-4bf0-8d57-e33ac50eba71

### 3) Delete github repo

https://github.com/taqinasirr/kod/assets/21170527/23e07794-cc03-4329-a0d4-14159496db9d



<br><br>

# `VS Code`

https://code.visualstudio.com/docs/sourcecontrol/overview

<br>

boleh terus commit.  
vscode sendiri yg akan add untracked files to staging area


> *Untracked files - files yg takdak kat staging area. (git tak tau dia wujud)*  
> *tracked files - files yg ada kat staging area. (git tau dia wujud)*



https://github.com/taqinasirr/kod/assets/21170527/6776a90b-8d36-4d23-9e62-fca408f53a21

<br>

synchronize changes = apa yg ada kat branch remote sebijik mcm apa yg ada kat branch local.    
berlaku pull & push  
1. pull remote changes down to your local repo
2. push local commits to remote

https://github.com/taqinasirr/kod/assets/21170527/1f3af76e-bd6a-4404-96f8-ff34d1710911

<br>

Commit options

<img src = "https://github.com/taqinasirr/kod/assets/21170527/23c97d74-ebd5-4cec-8306-cd5d3a39e59c" width="800">

<br><br>

Command options

https://github.com/taqinasirr/kod/assets/21170527/ab90bb15-c746-4bf4-8a4a-7aeb4a0b9223

<br>

Symbols

![git status bar - publish and synchronize](https://github.com/taqinasirr/kod/assets/21170527/81f26a02-bdaf-4c53-983f-bcfed5fd6809)


![untracked, modified](https://github.com/taqinasirr/kod/assets/21170527/9078bb73-e51e-4262-9b23-6bb63485c5e5)

<br><br><br>





# `Git`

<img src = 'https://github.com/taqinasirr/kod/assets/21170527/70b9856f-97bd-40aa-8c28-315c2949e381' width ='500'>  
<br><br><br>

<img src = 'https://github.com/taqinasirr/kod/assets/21170527/92b4ae17-0637-47ee-aefd-012733d18962' width ='400'>\  
<br><br>
<img src = 'https://github.com/taqinasirr/kod/assets/21170527/3f5b7b75-b2d6-46a2-ae93-90bb531d5f8c' width ='400'>
<br><br><br>

```php
 git fetch  //copies commit from remote (online repo) into local repo
 git pull   //copies commit from remote into local repo & working directory  
 git pull vs pull request  //pull dgn pull request takde kaitan mart...
 //Pull request is a process for a developer to notify team members that they have completed a feature.
 git stash  // cth kita dari branchX nak tukar ke main branch tanpa commit. git tak bagi.
            //git suruh commit or buat stash dulu
            //stash = save apa benda yg kita tgh buat kat branchX, tanpa commit
```





<br>

### Git commands

```php
git
  --version atau -v
  config 
    --global user.name namakau              //identify yourself (to track who made change)
    --global user.email emailkau            //identify yourself (to track who made change)
    user.name                               //show nama user
    user.email                              //show email user
  init
  status                                    //show branch, changes to be commit , untracked files
  add 
    index.html                              //add file to staging area.
    index.html style.css script.js          //add multiple files
    .                                       //add all files to staging area.
  rm --cached index.html                    //remove from staging area	
  commit -m 'message disini'                //commit with messages
  log                                       //show all commit, commit id, who made the commit, date&time of commit,commit msg
  log --oneline                             //show all commit, shortened commit id, commit message
  checkout 
    5ab48ca                                 //go to commit with that shortened id
    main                                    //switch to main branch
    branch1                                 //switch to branch1 (branch1 dah wujud)
    -b branch1                              //create branch1 and switch to that branch
  branch                                    //show current branch
    branch1                                 //create branch1
    -d branch1                              //delete branch1. pastikan berada kat branch lain sblum delete branch1
    -a                                      //show all branches  
  merge branch1                             //merge branch1 dgn main branch. pastikan berada kat main branch sblum merge
  remote                                    //show all remote yg ada
  remote -v                                 //show all remote punya url
```


<br>

### How to git ignore

create file `.gitignore`, buh kat root directory.
dlm file tu:
```php
  /ayam           //ignore folder ayam kat root directory shj
  ayam/           //ignore folder ayam kat semua directory
  /ayam.txt       //ignore file ayam.txt kat root directory shj
  ayam.txt        //ignore file ayam.txt kat semua directory
  /*.txt          //ignore all text file kat root directory shj
  *.txt           //ignore all text file kat semua directory
```

<br>

### Jump to specific or latest commit

`git log`  show commit history  
`git log --oneline`  show commit history.  shorter version  
`git checkout xxxxxxx` go to commit xxxxxxx  
`git checkout namaBranch`   go to lastest commit pada branch tree

cth ada 5 commit  
checkout to 1st commit, bila git log, dia hanya tunjuk 1 commit je. sebab waktu tu belum 5 commit.  
so utk ke commit ke 5 (latest commit), pakai git checkout namaBranch

https://github.com/taqinasirr/kod/assets/21170527/16d67704-c851-44b5-ab72-5179e87f29a9

<br>

### Checkout branch

https://github.com/taqinasirr/kod/assets/21170527/ba0412ce-d156-4353-a73a-435947a7af03





<br>

### Merge conflict:  
 ada main branch  
 create branch bernama branchX  
 katalah branchX ni adalah copy kpd main branch.  
 fungsi branchX adalah supaya tak kacau main branch.  
 
 kat branch, ada file makan.html    dlm dia tulis ni:  
   ```<p>saya suka makan </p>```
   
 kat branchX aku ubah dia jadi    
   ```<p>saya suka makan nasik ayam</p>```
   
 kat main branch pulak berlaku perubahan dia jadi  
   ```<p>saya suka makan nasik lembu</p>```
   
 bila aku nak merge branchX dgn main branch, terminal bagitau merge conflict in makan.html    
 pastu kat belah kanan tu dia tulis (main|MERGING)  
 maksudnya kita bukan kat branchX, bukan kat main branch. tapi kat branch merging yg belum selesai.  
   
 bila bukak makan.html tu, dia jadi gini:  
 
 ```
  <<<<<<< HEAD
  <p>saya suka makan nasik lembu</p>
  =======
  <p>saya suka makan nasik ayam</p>
  >>>>>>> branchX
```

katalah kita nak yg branchX tu. so, just delete benda yg tak berkaitan. so jadi gini
   ```
   <p>saya suka makan nasik ayam</p>
   ```
   
then, just commit mcm biasa. so kita berjaya lah merge branchX dgn main branch






