### Infrastructure description

- A RDS database running Postgres.

- A AWS EB for hosting the backend.

- A AWS S3 bucket for hosting the frontend.

- A AWS S3 bucket for hosting uploaded pictures.

### Front-End dependencies

- [Angular](https://angular.io/) - Single Page Application Framework
- Deployed on an S3 bucket named udagram1

### Backend dependencies

- [Node](https://nodejs.org) - Javascript Runtime
- [Express](https://expressjs.com/) - Javascript API Framework
- [PostgreSQL](https://www.postgresql.org/) - PostgreSQL Database
- The DB is hosted on AWS RDS
- The app is hosted on AWS Elastic Beanstalk
- The app uses udagram-media-2 S3 backet to upload images

### Pipeline Process

- Committing new code to the GitHub repo triggers the below jobs in circleci:
  1. Front-End Install
  2. Front-End Build
  3. Front-End Deploy
  4. Back-End Install
  5. Back-End Build
  6. Back-End Deploy
