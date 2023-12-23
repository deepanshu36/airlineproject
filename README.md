# airlineproject
∗ Developed a data pipeline on daily flights data we recieve in s3 bucket in a particular folder
∗ Flights data is combined after filtering with airport dimesity table which is preloaded in my redshift tables
∗ s3 event put object create an event notification in our eventBridge which has my aws state machine as a target
∗ AWS state machines triggers my AWS glue crawler and create metadata only for the new data we have in our
data lake
∗ Glue job creates pyspark dataframe with my data, filters it, performs joins with airport dimensity table to finally
load it into my redshift tables for furthur analytical process


please look at the youtube video to see the project flow
https://youtu.be/yf4L8LtJpEw?si=E-FmRuaPPb0wRMx6
![airline drawio (2)](https://github.com/deepanshu36/airlineproject/assets/38796030/3595b55f-e42e-4a82-9822-dc0d39440365)
