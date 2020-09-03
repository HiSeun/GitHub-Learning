# How to PUSH and PULL github repository
## 1. git config
You don't need to do this all the time. Only for the first time.

```
git config --global user.email "github email"
git config --global user.name "github ID"
```
## 2. git clone
Move to the directory where you would like to download the github repository **PushPull** .
If you want to build the directory tree as below :
> Workspace
>  >  githubLearning
>  >  > **PushPull**

```
cd Workspace/githubLearning
git clone git@github.com:HiSeun/githublearning.git 
    This SSH address is for mine. Use one for you want.
```

## 3. Remove File
### 3.1. From both local and remote repository
If you want to remove file or directory **not only from local repository but also from remote repository**.
```
git rm [File Name]
```
### 3.2. Only from remote repository
If you want to remove file or directory only from remote repository follow as below.
```
git rm --cached [File Name]
```

### 3.3. Only from local repository
If you want to remove file or directory only from local repository follow as below. ```git``` command is no longer needed.
```
rm [File Name]
```

## 4. Adapt change to Remote repository
### 4.1. Check the status
<img src = "/Shots/pushpull1.png"></img>

First, check whether your change is valid.  
If the change you made is not shown in green color, make sure that you add your file using ```git add``` or something.
<img src = "/Shots/pushpull2.png"></img>
```
git status
```
### 4.2. Push the change
```
git commit -m "comment about the change"
git remote add origin "your git address"
git push origin master
```
You don't need to command the second line always, do just once.   
Go to your remote repository and check whether change was adapted or not.

### 4.3. Error
I experienced several error from the above step.
#### 4.3.1. Nothing to commit or push
<img src = "/Shots/pushpull3.png"></img>
* There should be at least one change and ```git commit``` command, before you push your local repository.

#### 4.3.2. Origin master problem    
<img src = "/Shots/pushpull4.png"></img>
* It's simple. Just remove your origin master, and reset.
```
git remote rm origin
git remote add origin "github address~~~~"
```
or
```
git remote set-url origin "github address~~~~"
```
#### 4.3.3. Changes occured in remote repository
<img src = "/Shots/pushpull5.png"></img>
* It's also simple. Before push your changes, pull the git first and then push again.
```
git pull origin master
git push origin master
```
<img src = "/Shots/pushpull6.png"></img>
