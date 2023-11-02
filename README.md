# GIT Cheatsheet

## Resources
- https://www.youtube.com/watch?v=SWYqp7iY_Tc&t=15s
- https://www.youtube.com/watch?v=IHaTbJPdB-s  
- https://www.youtube.com/watch?v=NcoBAfJ6l2Q  -- Harvard Lecture
- https://www.youtube.com/watch?v=eulnSXkhE7I  -- Harvard Lecture
- https://www.youtube.com/watch?v=nT8KGYVurIU  -- Fork and Pull request (Specific)
## What is Git and GitHub?
- Git : VCS software application
- GitHub : VCS cloud-based repository host, collaboration web application, CI/CD

# CLI

## Creating a new repo

### After creating repo on GitHub
`git init`

### Add README.md to staging
`git add README.md`

### Commit to local repo
`git commit -m "first commit"`

### Switch branch to main (master -> main)
`git branch -M main`

### Set origin to your github repo url
`git remote add origin https://github.com/<your-username>/<your-repo-name>.git`

### Push to repo
`git push -u origin main`

## Updating local master with remote changes from a different branch (origin/dev_frontend)
```
git checkout master
git fetch origin
# you should now have dev_frontend locally
# now we merge dev_frontend into master (our current branch)
git merge dev_frontend 
# assuming you already had the dev_frontend branch and you get merge conflicts
```

# Useful commands
### Check remote repo url
`git remote -v`

### Force push a single branch
`git push origin +main`
> https://stackoverflow.com/questions/5667884/how-to-squash-commits-in-git-after-they-have-been-pushed
