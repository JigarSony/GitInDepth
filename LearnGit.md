du -c
git: content addressible system

touch coding.txt

echo I love coding > coding.txt

cat coding.txt
http://www.yourownlinux.com/2014/01/linux-ls-command-tutorial-with-examples.html

https://www.redhat.com/sysadmin/ls-command-options

ls list of files
 
ls -la list of all file with . and .. folders also 

>git init - it's git project please look into this

>for see all files  >du -c
 git ? - Content Addressible System
 
>touch coding.txt

echo I Love coding > coding.txt

to print >cat coding.txt

to add into git for takecare of
>git add coding.txt
 in ./.git/objects/e6

long #
it create hash in this folders
90065515b5188b40a5c0df4a975849d1677aea

when you add in git read the content and create hash

cat - print content of the file

decompression file
printf "\x1f\x8b\x08\x00\x00\x00\x00\x00" |cat - /tmp/data |gzip -dc 

$ printf "\x1f\x8b\x08\x00\x00\x00\x00\x00" |cat - ./.git/objects/e6/90065515b5188b40a5c0df4a975849d1677aea |gzip -dc

blob 14I love coding

$ git cat-file -p e690 - pretty formate

$ git cat-file -s e690 - size of file

$ git cat-file -t e690 - type of file


what is 90065515b5188b40a5c0df4a975849d1677aea > sha1hash

$ echo -e 'blob 14\0I love coding' |shasum

in that 1st 2 characters are bucket and others are identified

https://www.bitdegree.org/learn/git-commit-command

The following example shows how to save a snapshot of changes done in the whole working directory. This code only works for tracked files.

git commit -a

This Git commit example shows how you set the description with the commit function:

git commit -m "<message>"


git commit -am "First commit"

this created on commit objects

du -c  > it have created 2 objects - why ?

 git cat-file -p ./.git/objects/25/0a95fbb73b35fd1cff38a409e4063887f9fb14


 git cat-file -p 250a95fbb73b35fd1cff38a409e4063887f9fb14 
  it will give tree objct
  
   git cat-file -s 250a
   
    git cat-file -t 250a
	
	
	now lets check for tree
	
	
	 git cat-file -p e2ad > 100644 blob e690065515b5188b40a5c0df4a975849d1677aea    coding.txt

	 it will give 
	 tree with 
	 file type blob 
	 and object e690 is file we have created 
	 with file name coding.txt
	 
	  git cat-file -t e2ad > tree

git it self a like a database


what if we can change the file name? - sha1hash changed ?

No

mv coding.txt youtube.txt


what if you added minor change in the file (like add .) I added to git 	  does git create new object or diff of object 

vim 1.png -> i > add . in last > :wq

git gc --aggressive > 


git log

check last and track that till parent disappear
all objects in git are inmutable

to check inside the pack files

>git verify-pack -v .git/objects/pack/pack-.idx


git checkout -b new_feature

Rebase - changed the history of project
Rebase - changed the history of project
  
  
  https://github.com/coding-parrot/projects/blob/master/git_commands.txt
	 
  
  




