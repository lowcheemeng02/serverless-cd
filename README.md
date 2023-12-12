# serverless-cd

Pipeline jobs:
1. pre-deploy: print some messages
2. read-from-secrets-mgr: Use aws cli to retrieve a secret from AWS Secrets Manager
3. install-dependencies: Install the libraries that the Node application needs
4. deploy: test and deploy node app

The jobs are executed in parallel usually but with the "needs" set up in the repo they are run in sequence