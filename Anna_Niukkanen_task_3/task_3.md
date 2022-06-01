### Task 1. Can the Reduce stage start before the Map stage is completed? Why?

### Task 2. Give an example of Map only and Reduce tasks

Map only task means that the mapper does all task with its InputSplit and no job is done by the reducer. Mapper's output is the final output.
Example of Map Only Job: 

![MapOnly](https://github.com/Annassie/BigData-Hadoop/blob/Anna_Niukkanen_task_3/Anna_Niukkanen_task_3/screenshots/MapOnly.png)

The example of the Reduce task:

![Reduce](https://github.com/Annassie/BigData-Hadoop/blob/Anna_Niukkanen_task_3/Anna_Niukkanen_task_3/screenshots/Reduce.png)

### Task 3. Deploy a hadoop cluster, build a WordCount application, run on the dataset 'ppkm_sentiment' and print the 10 rarest words


#### First we creat mapper.py and reducer.py - files locally:

![mapper.py](https://github.com/Annassie/BigData-Hadoop/blob/Anna_Niukkanen_task_3/Anna_Niukkanen_task_3/screenshots/mapper_py.png)

![reducer.py](https://github.com/Annassie/BigData-Hadoop/blob/Anna_Niukkanen_task_3/Anna_Niukkanen_task_3/screenshots/reducer_py.png)

#### And give executing rights to everyone:

![executing_rights](https://github.com/Annassie/BigData-Hadoop/blob/Anna_Niukkanen_task_3/Anna_Niukkanen_task_3/screenshots/executing_rights.png%20.png)

#### Then we locate it into ppkm_sentiment-dataset using 'hadoop-streaming'-library:

![in ppkm_sentiment](https://github.com/Annassie/BigData-Hadoop/blob/Anna_Niukkanen_task_3/Anna_Niukkanen_task_3/screenshots/Screenshot%202022-05-27%20at%202.06.32.png)


#### Finally we can run WordCount application on ppkm_sentiment-dataset and print 10 rare words:

![10 rare words](https://github.com/Annassie/BigData-Hadoop/blob/Anna_Niukkanen_task_3/Anna_Niukkanen_task_3/screenshots/sort_10_rare_words.png)

### Task 4. Change the mapper in WordCount so that it removes punctuation and converts all words to the same case


### Task 5. *You have two datasets with the same keys. You need to combine them by summing the values ​​with the same keys. How to do it in MapReduce?


### Task 6. *There is a dataset on the cluster, in which the keys are the employee id and date, and the value is the amount of the payment. 
### The manager set the task to calculate the average amount of payments for each employee for the last month. 
### In the mapper, you filtered out old entries and returned a key-value of the form: id-money. 
### And in the reducer, you summed up all the incoming numbers and divided the result by their number. But you came up with the idea to optimize the  calculation by setting the same reducer as a combinator, thereby reducing the data shuffle. Can you do that? If so, where could the mistake have been made? If not, what should be the output of the combinator?


