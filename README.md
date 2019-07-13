# Info7374 Assignment-1

## Brief introduction of Alyce as a company

Alyce is the AI-powered platform that’s redefining direct mail, swag and gifts with its scalable, sustainable, hyper-personalized approach to account-based marketing. Alyce builds real, human relationships that deliver up to twice the named account penetration versus traditional approaches. Founded in December of 2015, Alyce is a privately held company headquartered in Boston, MA.

## DataSets Description

- `alyce_client`: This is a dimension table which contains information about the Alyce's clients.

- `alyce_giftdata`: This is a dimension table which contains information about different types of gifts

- `alyce_services`: This is a dimension table which contains information about different types of services offered by Alyce like one-to-one gifting, swag select etc.

- `alyce_recipient`: This is a dimension table which contains information about the gifts sent by the Alyce's client to the people who they want to maintain relationship with.

- `alyce_clientexpenditure`: This table holds the information about the type of gift, recipient to which the client sent the gift and also few metrics like price, quantity etc.

- `alyce_facts`: This table holds the information about the total amount spent on the gifts ,total number of gifts sent by the clients and the type of service the client has enrolled for.

## AWS Analytics Pipeline 

## Architectural Components:

- `S3 Bucket`: https://aws.amazon.com/s3/
- `Kinesis Data Stream`: https://aws.amazon.com/kinesis/data-streams/
- `Kinesis Delivery Stream`: https://aws.amazon.com/kinesis/data-firehose/
- `Redshift Cluster`: https://aws.amazon.com/redshift/
- `IAM Policy`: https://aws.amazon.com/iam/
- `IAM Role`: https://aws.amazon.com/iam/

### Required libraries:
```
$pip install boto3
$pip install psycopg2
```
### Steps to setup the Architecture

- Set up the AWS Access keys in `IAM`.
- Configuration of respective Parameters like Name of AWS S3 Bucket ,IAM Access policy name,Redshift Database Name etc.
- Create `AWS S3 Bucket`.
- Create `IAM Policy` and `IAM Role` for Architecural access.
- Attach the Policy to the Role.
- Create the `AWS Redshift Cluster`.
- Create Database tables on Redshift.
- Create `Kinesis Stream`.
- Create Kinesis Delivery Stream: Firehose.
- Test it by Real-time data streaming.

## Visualization of Alyce Data
 
For visualiztion of Alyce data we first establish a connection between our Database and Tableau .With the implementation of Tableau on Alyce data, stock traders or company can derive meaningful insights from past data and can take appropriate business decisions for future outcomes. With the help of this assignment, A working data warehouse was developed to answer business queries and interesting trends for the growth of the company. Using Tableau, we built dashboards to show trending analysis, contribution analysis along with drill downs and ranking analysis to gather meaningful business insights and geography-wise distribution of clients to answer several new questions for the market investors. 




