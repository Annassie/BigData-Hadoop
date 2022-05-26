### Task 1. Can the Reduce stage start before the Map stage is completed? Why?

### Task 2. Give an example of Map only and Reduce tasks


### Task 3. Deploy a hadoop cluster, build a WordCount application, run on the dataset 'ppkm_sentiment' and print the 10 rarest words


### Task 4. Change the mapper in WordCount so that it removes punctuation and converts all words to the same case


### Task 5. *You have two datasets with the same keys. You need to combine them by summing the values ​​with the same keys. How to do it in MapReduce?


### Task 6. *There is a dataset on the cluster, in which the keys are the employee id and date, and the value is the amount of the payment. 
### The manager set the task to calculate the average amount of payments for each employee for the last month. 
### In the mapper, you filtered out old entries and returned a key-value of the form: id-money. 
### And in the reducer, you summed up all the incoming numbers and divided the result by their number. But you came up with the idea to optimize the ### calculation by setting the same reducer as a combinator, thereby reducing the data shuffle. Can you do that? If so, where could the mistake have been made? If not, what should be the output of the combinator?


