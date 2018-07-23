## written by FancyAction

# Initial Set up

* clone the repo
> $ git clone https://github.com/chingu-voyage4/Toucans-Team-3.git
* switch to development branch
> $ git checkout development

# When you start working on something

* create a new branch that’s based on the development branch
> $ git checkout -b <NAMEOFBRANCH>
* sample
> $ git checkout -b style/pink-buttons
* this is where you code if you forgot to create a branch and already started coding if you haven’t committed yet
> $ git stash

> $ git checkout -b feature/rubber-duck-cta

> $ git stash pop
* if you already committed
> $git push origin development:fix/your-smart-fix
* delete development branch and get it back again pure
> $ git checkout master

> $ git branch -D development

> $ git fetch

> $ git checkout development

> $ git checkout fix/your-smart-fix

# Naming branches

* Include #issueNumber the branch is addressing after the /. This automates issue in Waffle

bug/#14-fixed-all-caps

feature/#6-giant-duck-modal

refactor/#102-add-prop-types

style/#99999everything-is-black

# Commit titles

* If a commit closes an issue, write within the commit "closes #issueNumber"
* Capitalize the first letter
* Keep it short and clear
* Sample
> $ git commit -m “Fix routes priority closes #15"
* If you have more to say, use the commit body
* Sample
> $ git commit -m “My commit title closes #6” -m “My commit body message”

# Push commits

* start from the branch you were working on
> $ git checkout development

> $ git pull

> $ git checkout fix/my-branch

> $ git merge development

* In Github, in either the Pull Request title or description, write "closes #IssueNumber" so Waffle automates to Done.
(via @Jon)