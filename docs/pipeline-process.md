### Pipeline Process

- Committing new code to the GitHub repo master branch triggers the below build job in circleci:
  1. Install Node, AWS cli and EB cli.
  2. Install the Front-End's dependencies
  3. Build the Front-End
  4. Deploy the Front-End to S3 bucket
  5. Install the Back-End's dependencies
  5. Build the Back-End (from ts to js)
  6. Deploy the back-End to AWS EB
