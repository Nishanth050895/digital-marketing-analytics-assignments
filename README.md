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

# Assignment 2

## Same architecture as above

### Objective
Customer acquisition is one of the important aspect of an organization which helps them to understand more about their expenditure and also the revenue generated from it, so that they can plan accordingly and focus more on those customers which bring value to them.

Margin metrics helps the company to know how much profits they are making and also use it to enhance their business.

### Topics

1. Customer Acquisition -- Nishanth Manjunatha

2. Margin Metrics -- Uthsav Shetty

3. Happy Customers -- Srikanth Reddy Gubballi

### Customer Acuquisition Cost
Customer acquisition cost (CAC) is a metric that has been growing in use, along with the emergence of Internet companies and web-based advertising campaigns that can be tracked.

CAC, as you probably know, is the cost of convincing a potential customer to buy a product or service.

CAC is not just what you spend on advertising! There are many hidden costs that go into customer acquisition, which may include:

Discounts and promotions
Publicity costs (including PR)
Events and conferences
We need to know the company's CAC so that we understand if the customer's lifetime value (LTV). If LTV is more than you pay to acquire the customer, then we are losing money with every customer.

Attribution: Who gets the credit?

There are a few common attribution models

Last Touch Attribution
Distributed Attribution
Decaying Attribution
Calculating your customer acquisition cost would be much easier if all users came from the same channel

Step 1: Determine how much each channel costs you.

Step 2: Weighted distribution.

Finally, we would also like to know the payback period of the customer after acquisition.

For some businesses, the payback is immediate because the customer makes a product purchase that is more than their CAC. However, for many subscription and recurring revenue businesses the payback period can be very long!

### Margin Metrics
Margin Metrics

The most important metrics to track about the business are margins. Margins measure the profitability and are calculated by comparing profits to the revenue. Typically, margins are measured as a percent of revenue.
Why Does It Matter?

Although there are slight variations on the definition, a profit margin typically represents the percent of revenue earned after all costs, business taxes, depreciation, interests, and other expenses have been deducted.

These are some reasons you should track your profit margins:

It helps you grow your business: Figuring out your profit margins can help you determine excess spending or underperforming products and practices for your business. It's helpful data to have on hand when evaluating how your business moves forward as it grows and expands.
It helps you flag and resolve issues: Staying in tune with what your profit margin in helps you identify issues you might be having running your business. For instance, if your profit margin is low, you might be having some pricing errors, expense management problems, or accounting issues.
It's required for financing: You might have a very compelling product, idea, or service that your business offers, but lenders are going to want to know where your profit margin stands before offering you a small business loan. Even if you're already making millions, if lenders don't know whether you're not profitable, it's more difficult to secure financing.
Once you have your profit margin, you can see how many revenue dollars are actually going to your bottom line, as opposed to covering your business expenses. The profit margin can also reveal whether you've priced your product too high or too low.

How do you calculate Margins?

Gross Margin is calculated by subtracting your total cost of goods sold (COGS) from your total revenue and then dividing by total revenue.

margins

gross_margin

Here,

Total Revenue is sum of Total gifts sold and fee

COGS is total gifts sold

Net Margin is calculated similarly to Gross Margin but instead of subtracting just COGS, you subtract all variable costs which include your COGS, marketing, sales, etc.

Total Revenue is sum of Total gifts sold and fee

Total variable costs is sum of total gifts sold and variable costs (personnel salaries)

The easiest way to blend margins together is a simple weighted averaged, calculated by weighting the margins by the amount of revenue for each product or service.

Grouping all services together to measure the overall service margins

Services like One to One gifting, Swag select & Measurement and Tracking.

How Can You Improve Your Profit Margin?

Of course, knowing what a good profit margin is and understanding the profit margin is the first step in improving margins. Once we have that data, these are just a few ways we can help the business improve its profit margin:

Decrease expenses: Knowing the profit margin can help uncover bloated spending practices or help you make decisions about where to cut costs. It's all about keeping your overhead as low as possible, while still being able to produce a quality business product.

Cut underperforming products or services: Same here. Perhaps your gross profit margin analysis determines that one of your products is manufactured at a higher cost but isn't selling as well as other products on the market. Making that call is only yours to make, but it's certainly one way to bring up your profit margin percentage if that is indeed the goal.

Increase product offerings or services: Could the business be doing more while maintaining equivalent overhead expenses? If so, this means more money in the pocket. Consider going the extra mile with what you already have, and if we don't need to make huge financial investments in order to accomplish that, then it might be time to just go for it. Remember, your best customer is often the customer you've already won, so consider increasing product offerings or level of services to your most loyal customers to get more out of them.

Increase pricing: Raising prices can be a difficult decision for small businesses that are competing with larger companies, but sometimes it's necessary for your business's long-term survival. Make sure we're not overcharging, but we also want to ensure that we're not undercutting our self with very low prices.

### Happy Customer
WHY?

Customer acquisition is good in getting to know how many customers are frequent users and like the product, but how to identify that these customers or clients are likely to stay in the near future? Majority of the customers stay back mainly because of the services provided by a company or they really like the platform that they do not want to let go. And that is where getting to know the HAPPY CUSTOMERS is crucial.

HOW?

These customers are the people who like the product they are using and will continue to do so unless we really screw it up. So to understand more about this we will have to some form of a survey or analysis to get to know more about it.

We came up with a new service idea of choosing the gifts for our clients rather than choosing by themselves. To do this we will send them a set of questionnaire that they will fill and based on those answers Alyce will choose the gift on behalf of them.

To understand more about this, we will demo this service for a couple of customers, get their reviews and send out a survey to everyone to fill out. Based on their response we can decide that the service is a good idea to retain majority of them or lose all of them.

The is_present? column gives information about clients response if the above service is introduced and is_not_present? column gives information about clients response who are happy with the present set up.

Based on the response we can segregate customers into 5 categories.

Attractive features — Attractive features trigger feelings of satisfaction and delight when present, but users are not dissatisfied if the feature is not included.
One dimensional feature —These features result in satisfaction if present and dissatisfaction when they are not.
Must have features — These features are ones that customers expect the product to contain.
Unimportant features — Users are ambivalent about unimportant features, they simply do not care if they are included or not.
Undesired features — Including undesired features negates the positive impact of Attractive and One-Dimensional features
The above study of the survey is based on Kano model, in which he specifies that the customers are not most likely to stay forever if they do not like the product or service anymore and we can draw the graph as shown below.



Based on the responses, we can ask the customers how likely are they to refer us to others. This is similar to net promoter score which helps us identify who are happy with us or who are not and market accordingly.
