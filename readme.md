## Repos have two main branches: 
  - Master(deployed to production) and 
  - Staging (deployed to staging).

## Deploying features and bugfixes to remote staging repo / site:
 1. Pull from remote staging repo
 1. Checkout the feature "feature/my_feature" or "bug/my_bug" from local staging
 1. Dev and test locally
 1. Merge feature or bug branch into local staging repo
 1. Deploy to remote staging repo (which is set to auto deploy through beanstalk to staging site)
 1. Test on staging site
 1. Notify QA with link to staging url
 
## Deploying to master repo / site:
 if your feature or bug has been approved on the staging site.
 1. Notify QA deploy to production is about to begin.
 1. Local checkout master
 1. Pull from remote master repo
 1. Merge local staging into master
 1. Push to master repo (set to manual deploy through beanstalk).
 1. If push is successful then do manual deply
 1. Notify QA with link to production url
