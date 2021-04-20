### Git

#### Remove all local branches but BRANCH_NAME
`git branch | grep -v "BRANCH_NAME" | xargs git branch -D`
