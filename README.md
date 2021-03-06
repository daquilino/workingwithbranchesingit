# Working with branches in git (GitHub)
Guide and demo working with branches in git.

[https://github.com/daquilino/workingwithbranchesingit](https://github.com/daquilino/workingwithbranchesingit)

## Working with other people
https://docs.github.com/en/github/setting-up-and-managing-your-github-user-account/inviting-collaborators-to-a-personal-repository

One member will have to host the repo on their GitHub.
They can then add the other members as collaberators
(On Gihub -> settings -> Manage acess -> Invite a callaborator ) 
Other team members will clone their repo. And create branches


# Creating a new brach
~~~
> git branch NAMEOFBRANCH
~~~

# Switching to your new branch (or any branch)
~~~
> git checkout NAMEOFBRANCH`
~~~

### **Alternatively** (Both above in a single step)
~~~
> git checkout -b NAMEOFBRANCH
~~~


#  Pushing to your new branch
~~~
> git add -A
> git commit -m "SOME COMMENT"
> git push origin NAMEOFBRANCH
~~~




# Checking which branch you are on
~~~
> git branch
~~~

# Updating (Pulling and Merging) your branch from Master (or any branch)
** THIS SHOULD ALWAYS BE DONE BEFORE COMMITING AND PUSHING YOUR BRANCH TO UNSURE YOUR BRANCE IS UP TO DATE WITH MASTER (or any other branch)



- In the master branch (this updates your local master branch)
~~~
> git checkout master
> git pull
~~~


- Then swich to the branch you want to merge
~~~
> git checkout NAMEOFBRANCH
> git merge master
~~~


- **Alternatively** from within your brach you can run
*This will (fetch and merge) the master branch into your branch. However this will **NOT** update your local master branch.
~~~
> git pull origin master
~~~