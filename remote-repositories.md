[*Home*](https://neba9.github.io/reading-notes/)

# Git vs github


### **Github** is the hosting platform for **Git**. Most developers are familiar with Github and it is easy to adapt to it. The difference between Git and Github is that Git is an open source version control system and Github is a web-based hosting service for Git repository.

 ### **Stashing Changes**
When you are not ready to commit changes but do not want to lose them either, git stash is a great option. This command temporarily removes changes and hides them, giving you a clean working directory. When you are ready to continue working on the changes, simply use the git stash apply command to retrieve the hidden changes.


 ### **what is Remote Repositories** :-
 it helpes to collaborate on Git projectsversions of a project residing online or on a network. You can work with multiple repositories, for which you can have read/write or read-only privileges. Teams can use remote repositories to push information to and pull data from.
 
  -**cloned repositories**:- Git will automatically give the name “origin” to the server from which you cloned and the name **“master”** to your local branch.

### **Seeing Your Remotes**
By running the **git remote** command, you can view the short names, such as **“origin,”** of all specified remote handles.
By using **git remote -v**, you can view all the remote **URLs** next to their corresponding short names.  

#### Adding Remotes
To create a new remote Git repository with a short name, use the following format:

- **git remote add shortname url**

#### Fetching
Fetching entails pulling data that you don’t have from a remote project.

Here is the command format:

**git fetch [remote-name]**
- For cloned repositories, use the command **git fetch origin** to pull down any **new changes** that were pushed to the server since you cloned or last fetched from it.
- **Note**: git fetch solely pulls new data to a local repository; it does **not merge changes** with or modify your local work

#### Pushing
To push your changes “upstream” for sharing, you would use the following git push command format:

**git push [remote-name][branch-name]**
- Example:
$ git push origin master

#### Rename
To rename a remote’s short name, use the **git remote rename** command.

- Example:
$ git remote rename js nebiyu

$ git remote

origin

nebiyu
 - In the example above, we can see that the remote’s short name has been changed from **js** to **nebiyu**.
 - **command git remote** lists our existing remotes, which **nebiyu** is now one of.
### remove 
$ git remote rm nebiyu

$ git remote

origin
- **NOTE**: Reminder: **“origin”** is simply the default remote name when you use the **git clone** command.
