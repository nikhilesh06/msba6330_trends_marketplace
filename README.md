# msba6330_trends_marketplace
This is group 12 work for Big Data Trends Marketplace 

## PREDICTING TRANSPORTATION PRICES

### Trends Marketplace - Group 12


### Motivation

In recent years, ride-share apps such as Uber and Lyft have been continuously outperforming taxi companies such as the New York City Yellow Taxis. Our task in this project is to address this problem by predicting taxi prices in a similar fashion as ride-share apps in order to provide taxi companies with the opportunity to compete with these companies. These predictions can be implemented into an app which would allow users to know the price prior to ordering a ride, similar to Uber and Lyft apps. This project also demonstrates how to use AWS with big data and illustrates how to take the steps to create a predictive model in a big data environment.

### Technology

We used Amazon S3 to store our data. S3 is Amazon’s unlimited cloud object storage server that allows people to store files and images. It has the advantage that it is scalable, secure, highly available and durable. We created a bucket and then took the 12 months taxi data from the website of the New York government and uploaded those files into S3. Once the data was stored, we used Redshift for data preparation. Redshift is a scaled data warehouse. It is SQL-based and is useful for large scale OLAP and BI reporting. We built a table in Redshift to integrate the 12 months data into a single table. Afterwards, we exported the merged data files back to S3. Lastly, we used Amazon SageMaker to build, train, and deploy our machine learning solutions. In Sagemaker, we take the data that we have stored in S3 and perform basic feature engineering. Post that, we train models in the processed data to predict the taxi fare prices.

From this analysis, we were able to predict the price of a taxi ride accurately based on a set of readily available characteristics. We would recommend taxi companies utilize tactics like ours to implement a price-before-ride product in order to better compete with the large ride-sharing competition. In addition to taxi companies, we believe any business leader, interested in Big Data predictive analytics, could utilize the above process flow for their own development. We ran in to one main limitation: AWS only offers a certain amount of storage space in their free tier. This can be mitigated by others by upgrading to tiers with more storage capacity. 

This project repository is created in partial fulfillment of the requirements for the Big Data Analytics course offered by the Master of Science in Business Analytics program at the Carlson School of Management, University of Minnesota.
 
Set Up Instructions
Set up an Amazon S3 bucket. 
For instructions:  https://docs.aws.amazon.com/AmazonS3/latest/user-guide/create-bucket.html
Open Redshift to create a database using data on S3. 
For instructions: https://docs.aws.amazon.com/redshift/latest/gsg/bring-own-data.html
Create an Amazon SageMaker Notebook Instance and launch it. 
For instructions: https://docs.aws.amazon.com/sagemaker/latest/dg/gs-console.html.
Reference https://github.com/krishnaik06/AWS-SageMaker/blob/master/Untitled2.ipynb

### Video Link to our presentation
https://youtu.be/o_PtZhIF9k8
 
 
 

