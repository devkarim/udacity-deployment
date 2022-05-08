# Delivery & Deployment Pipeline

This project uses CircleCI for continuous delivery & deployment.

## Pipeline Process

1. Changes pushed to github repo.
2. CircleCI starts a "build" containing the new changes.
3. CircleCI initializes an environment for AWS, Elastic Beanstalk & Node.
4. Installs backend dependencies.
5. Builds backend then sets an archive up containing the build files.
6. Deploys the archive to Elastic Beanstalk.
7. Installs frontend dependencies.
8. Builds frontend in production mode.
9. Deploys frontend built files to an S3 bucket.
