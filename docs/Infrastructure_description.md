# Infrasctructure Description

![](architecture_diagram.png)

## AWS
### RDS Postgres 
- The application server uses AWS RDS Postgres as database for storing and retrieving information.
    + Endpoint: udacity835205258996.cacpeqwqb3fp.us-east-1.rds.amazonaws.com
    + Port: 5432
### Elastic Beanstack
- Used to save BE code and FrontEnd code will call the API's on  the EB through this endpoint.
    + Endpoint: http://udagramtest1-env.eba-wvujgb6f.us-east-1.elasticbeanstalk.com/
### S3 Bucket
- The frontend application is deployed using AWS S3 Bucket. The bundled assets are uploaded to an S3 bucket and that
bucket is made publicly readable. End users can access the application from the Bucket's endpoint.
    + Endpoint: http://udacity835205258996.s3-website-us-east-1.amazonaws.com