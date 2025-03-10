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
git fetch upstream
git checkout master
git merge upstream/master
```