# Aws-lambda-graphql-serverless


This is an example for using GraphQl in AWS lambda.
### Prerequisites
  - Nodejs
  - AWS account
  - Serverless framework (optional)

This project intended to build a GraphQL application that queries Subreddits and display its posts. It uses Reddit api in order to suply api with some json data. You can replase json source as you want.

### Installation

Aws-lambda-graphql-serverless requires [Node.js](https://nodejs.org/) v6+ to run.

Clone the repo, install the dependencies.

```sh
$ git clone git@github.com:svaqqosov/aws-lambda-graphql.git
$ cd aws-lambda-graphql
$ npm install
```


For dev environment you can use express...

```sh
$ node run server.js
```
Open http://127.0.0.1:1337 in your brouser.


In order to run lambda locally run:

```sh
$ sls offline start --skipCacheInvalidation
```
Open http://127.0.0.1:3000 in your brouser.




For deployment to AWS you need to have AWS account [`credentials installed`](https://serverless.com/framework/docs/providers/aws/guide/credentials).
If you already have AWS account credentials configured run this to deploy:
```sh
$ serverless deploy -f app --aws-profile dev --stage dev
```

