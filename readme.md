## Repos have one branche: 
  - Master(deployed to staging + production sites) 

## Deploying features and bugfixes to Staging:
 1. Pull from master repo
 1. If you want create a local feature branch.
 1. Dev and test locally
 1. Merge feature or bug branch into local master repo
 1. Deploy to remote master repo (which is set to auto deploy through beanstalk to staging site)
 1. Test on staging site
 1. Notify QA with link to staging url
 
## Deploying to Production site:
 if your feature or bug has been approved on the staging site.
 1. Notify QA deploy to production is about to begin on "live deployments" slack channel.
 1. In beanstalk do a manaul deploy to live site.
