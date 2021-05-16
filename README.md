# How-to-clone-a-git-repo-to-an-existing-folder-not-empty-

How to clone a git repo to an existing folder (not empty)

1. First get to the existing directory
   $ cd my/folder/

2. Now start a new git repository
   $ git init

3. Identify if the current elements on the directory are needed or not and add them to the .gitignore file. When ready...
   $ vim .gitignore

4. When ready create the first commit on the server
   git add .
   git commit -m 'my first commit'

5. Now add the remote from where you want to clone
   $ git remote add origin https|ssh:path/to/the/repository.git

6. Now just pull and merge with local git
   git pull origin master --allow-unrelated-histories
   git push -u origin master

other method

1. git init
2. echo \* > .gitignore
3. git remote add origin https://github.com/MatviyRoman/How-to-clone-a-git-repo-to-an-existing-folder-not-empty-.git
4. git fetch
5. git checkout origin/master -b master
