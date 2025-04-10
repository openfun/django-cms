# django-cms FUN fork

## This a fork from django-cms

This fork adds a feature that has not been yet accepted in the main django-cms 
repository. This feature improve page admin ux by making the page tree drillable.
*This feature has been developed for Django CMS 3.x. It may not work with 
Django CMS 4.x and above.*

## Repository details

This repository has two remotes (`git remote -v`):
- origin: https://github.com/django-cms/django-cms.git
- upstream: https://github.com/divio/django-cms.git

## How to update the fork

Here it is a step by step guide to update the fork when a new release of
Django CMS 3.x is available.

```bash
# Go the branch with the latest changes (e.g: 3.11.9-with-drillable-limit)
# Do a new branch with the latest changes
git checkout -b 3.11.10-with-drillable-limit

# Fetch the latest changes from the upstream repository
git fetch upstream

# Rebase the local branch on the upstream tag of the release you want to upgrade
git rebase 3.11.10

# Rebuild front
npx gulp sass icons bundle

# Commit changes, push and apply a tag on this commit
git add.
git commit -m "Rebuild 3.11.10"
git tag fun-3.11.10
git push
git push --tags
```