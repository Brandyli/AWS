# AWS_Athena_yelp_dataset

- Set up Glue to provision and run the ETL pipeline, taking JSON format of Yelp data set that stores in S3 bucket to queryable format
- Create S3 Bucket to hold Athena query result
- Configure Glue Crawler to connect to data source
- write a series of queries in Athena to implement aggregate calculationlike the state rank then download the result in csv. format

Query example:

SELECT state, COUNT (*) as num_states
FROM yelp
GROUP BY state
ORDER BY num_states DESC
LIMIT 10;

### AWS Glue
<img width="1440" alt="AWS Glue" src="https://user-images.githubusercontent.com/46945617/81243877-02762e80-8fdf-11ea-9599-f51e4c09f679.png">

### AWS Crawler
<img width="1432" alt="Screen Shot 2020-05-06 at 3 16 40 PM" src="https://user-images.githubusercontent.com/46945617/81243953-20dc2a00-8fdf-11ea-9c0f-0fdb7c5eeed7.png">

### Queries with AWS Athena 
<img width="1410" alt="Screen Shot 2020-05-06 at 10 02 36 PM" src="https://user-images.githubusercontent.com/46945617/81246400-7d424800-8fe5-11ea-8679-4862bbd5f5da.png">


