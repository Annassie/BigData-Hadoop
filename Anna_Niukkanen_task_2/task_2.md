### 1. Download and replace "ppkm_sentiment"-dataset into HDFS, and give full permissions to all users.

"ppkm_sentiment"-dataset was downloaded from Kaggle.com:

https://www.kaggle.com/datasets/mochkholil/ppkm-sentiment?resource=download

And replaced from Downloads-folder to bghdp-container in Docker:

![ppkm dataset downloading](https://github.com/Annassie/BigData-Hadoop/blob/Anna_Niukkanen_task_2/Anna_Niukkanen_task_2/images/cp_dataset_into_docker.png)

Cheking datset in HDFS (here 'archive'-folder):

![dataset in HDFS](https://github.com/Annassie/BigData-Hadoop/blob/Anna_Niukkanen_task_2/Anna_Niukkanen_task_2/images/dataset_in_gbhdp.png)

Creating ppkm-folder and moving files into it:

![ppkm-folder](https://github.com/Annassie/BigData-Hadoop/blob/Anna_Niukkanen_task_2/Anna_Niukkanen_task_2/images/mv_files_ppkm.png)

Giving full permissions to all users:

![Giving full permissions](https://github.com/Annassie/BigData-Hadoop/blob/Anna_Niukkanen_task_2/Anna_Niukkanen_task_2/images/giving_full_permissions.png)


### 2. Define the location of the blocks

Check the location of blocks using the command:

```diff
hdfs fsck folder/filename -files -blocks -locations
```


![Location of blocks](https://github.com/Annassie/BigData-Hadoop/blob/Anna_Niukkanen_task_2/Anna_Niukkanen_task_2/images/blocks_location.png)

So, based on the sceenshot, we can say that 

The name of block is #### blk_1073741825_1001,

 #### Size: len=43320 (bytes) and

 #### Location is 127.0.0.1:50010

### 3. You have 20 files, the size of each is 130MB. How many blocks will be allocated to the NameNode, assuming you have a default block size of 128MB and a replication factor of 3?

### 4.You have 1 file, the size of it is 1.56 TB. How many blocks will be allocated to the NameNode, assuming you have a default block size of 128MB and a replication factor of 3?

### 5. Your company has deployed a Hadoop cluster of 400 nodes. The replication factor is 3. How many machines can be disabled at a time so that there is no data loss?
