Spark Snippets

Q1. Given input address (any part of the address e.g., city or state),  nd all the business ids located at the address. You must take the input address in the command line. [For example, if the input address is Stanford then you need to  nd all businesses with stanford in the address column] [You only need business.csv  le to get the answer.]
Q2.a. Start spark-shell in local mode using all the processor cores on your system or the cluster.
List the business_id of the Top 10 businesses using the average ratings. This will require you to use review.csv. Please answer the question by calculating the average ratings given to each business using the review.csv  le. Next, sort the output based on the business_id before taking the top 10 businesses using the average ratings.b. Rerun Q2a using Yarn mode. Please solve using our cs6360 cluster. This questions shows how spark can be used on multiple systems in a cluster.Load all the dataset to hadoop cluster as you did in homework1.Use the address of the  le on the cluster as input to your scala script.Start spark-shell in YARN mode using Cs6360 spark cluster.This spark cluster consist 6 hadoop machine nodes. Using the following parameters 
Q3a:List the business_id , full address and categories of the Top 10 businesses using the average ratings.Use the  les business.csv and review.csv.Please sort the output based on the business_id before taking the top 10 business using the average ratings.
Q3b:Using broadcast variable in spark to store the business data, re implementyour solution to question 3a.Please measure the execution time of your program when using spark RDD (Q3a )and when using Broadcast variable (Q3b). Please compare the measured time.
Command to run 1:
1) Log into machine
2) Invoke the spark shell by entering spark-shell
3) Copy and paste the src file with the corresponding question number.
4) Press "Enter"
5) Output is displayed after execution

Command to run 2A:
1) Log into machine
2) Invoke the spark shell by entering spark-shell
3) Copy and paste the src file with the corresponding question number.
4) Press "Enter"
5) Output is displayed after execution

This job took 0.278468 s to execute.

Command to run 2B:
1) Log into machine
2) Invoke the spark shell by entering spark-shell --master yarn-client --executor-memory 2G --executor-cores 6 --num-executors 6
3) Copy and paste the src file with the corresponding question number.
4) Press "Enter"
5) Output is displayed after execution

This job took 1.013890 s to execute.
The time difference between the execution in local mode and in yarn mode is 0.735422


Command to run 3A:
1) Log into machine
2) Invoke the spark shell by entering spark-shell
3) Copy and paste the src file with the corresponding question number.
4) Press "Enter"
5) Output is displayed after execution

This job took 0.543209 s to execute.

Command to run 3B:
1) Log into machine
2) Invoke the spark shell by entering spark-shell
3) Copy and paste the src file with the corresponding question number.
4) Press "Enter"
5) Output is displayed after execution

This job took 0.350239 s to execute.
The time difference between the programs while running in spark RDD and when using Broadcast Variable is 0.19297