# Learn CPP into Visual Studio Code editor

https://www.youtube.com/watch?v=DIw02CaEusY

https://www.eclipse.org/4diac/documentation/html/installation/minGW.html

https://code.visualstudio.com/docs/cpp/config-mingw#_cc-configurations

## C++ std versions

$ g++  --version
g++.exe (x86_64-win32-seh-rev0, Built by MinGW-W64 project) 8.1.0
Copyright (C) 2018 Free Software Foundation, Inc.
This is free software; see the source for copying conditions.  There is NO
warranty; not even for MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.

$ g++ -std=c++98 -g test.cpp -o test

>> 199711

$ g++ -std=c++11 -g test.cpp -o test

>> 201103

$ g++ -std=c++17 -g test.cpp -o test

>> 201703

$ g++ -std=c++2a -g test.cpp -o test

>> 201709

$ g++ -std=c++20 -g test.cpp -o test

g++.exe: error: unrecognized command line option '-std=c++20'; did you mean '-std=c++2a'?

>>> References:
https://gcc.gnu.org/projects/cxx-status.html


# git Learn

> git init

>>> create a repository on github, then copy the path (https://xyz.git)

> git remote add  origin https://xyz.git

> git config --global user.name "pqrs" 

> git config --global user.email "abc@gmail.com"

> git pull origin master

>>> set the branch

> git branch --set-upstream-to=origin/master

>  git add file1 file2

or

> git add -A

> git commit -m "message"

> git push

(enter user name & password)

>>> some file / folder to remove

> git rm -r folder_name

or

> git rm -r -f folder_name

> git add -A

> git commit -m "Removed folder_name"

> git push

>>> git to completely ignore folder

> git-ignore folder_name/*

>> check it

> vi .gitignore

>>> fetch & merge & merge conflict

> git fetch origin master

> git merge

>>> resolve the merge conflicts (HEAD is my current changes)

> git add -A

> git commit -m "Merge conflicts resolved"

> git push origin master



### merge conflicts:

https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/resolving-a-merge-conflict-using-the-command-line

https://git-scm.com/docs/git-merge

https://www.atlassian.com/git/tutorials/using-branches/merge-conflicts