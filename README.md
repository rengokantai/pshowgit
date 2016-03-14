#### pshowgit
#####1
######2
Git will generate 40-digit hash according content.
```
echo "content" | git hash-object --stdin
```
######3
```
echo "content" | git hash-object --stdin -w  //save in repo .git/objects/
git cat-file 123213143141231213 -t  //show type of the content
git cat-file 123213143141231213 -p  //pretty printing content
```
######4
```
git count-objects
```
#####4
annotated tag is same as commit.(git objects: blobs,trees,commits,annotatedtags)
```
git cat-file -p tagname    //tag is symbolink of object
```
#####2
######1 branchs? is just a reference to a commit. HEAD is refreence to a branch
go to .git/refs/heads/master
```
cat .git/HEAD
```
checkout =move head + change working area
###### checkout a commit
```
git checkout 213213
(Then create several commits)(we must create a new branch to avoid these commits become garbage)
git branch new branch
```
the head will not be on any branch,just on a commit.(detached head)  
#####3
```
```
#####4
```
git show-ref master
```
a branch is just a reference to a commit.
