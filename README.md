# Demo Deployments with Github Actions using Tagging

The purpose of this repository is to use a release strategy to production using Github Actions tags. The requirements:
- All production deployment workflows should be manual
- All production deployments should use the tip of master
- A way to rollback production
- A way to immediate rollback production without reverting master (more optional)
- Handle potential concurrency issues. To avoid issues, it should queue releases to have a FIFO, but since we are a small team, it should just fail if someone else is mid deploy. GCP handles versioning too.
