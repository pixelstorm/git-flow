
## Overview
Firstly, commit regularly. 
Every commit is its own "solution to a self contained problem". In your commit message, simply explain the problem that you fixed.

## Wordpress
If working on a wordpress theme just commit the theme folder. ie run your git init command in your theme folder.

## Repos have one master branch: 
  - Master(deployed to staging + production sites) 

## Deploying features and bugfixes to Staging site:
 1. Pull from master repo
 1. If you want create a local feature branch.
 1. Dev and test locally (Do your own QA locally)
 1. Merge feature or bug branch into local master repo
 1. commit msg - use the asana task name or similar
 1. Deploy to remote master repo (which is set to auto deploy through beanstalk to staging site)
 1. Test on staging site
 1. Notify QA with link to staging url
 
## Deploying to Production site:
 if your feature or bug has been approved on the staging site.
 1. Notify QA deploy to production is about to begin on "live deployments" slack channel.
 1. In beanstalk do a manaul deploy to live site.
