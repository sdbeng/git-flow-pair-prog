## *One person create a repo*
    select initialize this repository with a readme
go to settings
    > branches
    > under protected branches
    > choose master branch
    > select protect this branch
    > select require reviews before merging

*add collaborators*
    > settings
    >  input each team members github username

*clone repo*
        send repository link to teammates
        click green clone button
    copy link
    go to designated folder in your terminal
command
    `git clone  [repo link]`
    `cd [repo name]`
you should now be on the master branch

*create branch off of master*
    `git checkout -b  BRANCH NAME`

*make commits on your branch*
    after doing work on your branch
in terminal
`git add .`
`git commit -m "message"`

push your work to main repo
    command
        `git push origin [branch name you are working on]`

*Create Pull Request*
    go to repo
    your pushed branch should be visible on main page
        click the green compare and pull request
    (optional) write a message to your team
    click create pull request

*Add Reviewers*
    on the right of the pull request page
        click the icon next to reviewers and add teammates
        ask someone on the team to review

*When review is complete*
    come to pull request page
    click merge pull request


*Make sure your local branch has the latest from master*
    from the branch you are working on
    command
        git pull origin master
    be sure to update your local master branch with the latest and the branch you are working on using command git pull origin master


*Fix merge conflicts*
    whats in between HEAD and =====
    is your current code
    whats in between ==== and (random numbers)
    is code your teammate has up the is in conflict with your code
Choose which code should be used and delete the surrounding text (i.e HEAD === / (random numbers)

Once complete
`git add .`
`git commit -m "message"`
`git push origin [your branch name]`

_Pull request will not be visible the second time you push the same branch. You can just go to that pull request and have a teammate review changes and merge_

_once complete with that specific task for that branch_
_go through the steps of making a new branch from master and work on your next task from that branch_
