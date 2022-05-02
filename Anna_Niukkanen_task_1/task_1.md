### 1. Installing Hadoop into Docker and running

![Hadoop installing](https://github.com/Annassie/BigData-Hadoop/blob/Anna_Niukkanen_task_1/Anna_Niukkanen_task_1/images/hadoop_installing.png)

Runnig using the next command:

docker run -it --name gbhdp \
               -p 50090:50090 \
               -p 50075:50075 \
               -p 50070:50070 \
               -p 8042:8042 \
               -p 8088:8088 \
               -p 8888:8888 \
               -p 4040:4040 \
               -p 4044:4044 \ --hostname localhost \ img-hdp-hadoop


![Hadoop running](https://github.com/Annassie/BigData-Hadoop/blob/Anna_Niukkanen_task_1/Anna_Niukkanen_task_1/images/hadoop_running.png)

### 2. Checking the status of resource manager, name node, data node

![Resource manager](https://github.com/Annassie/BigData-Hadoop/blob/Anna_Niukkanen_task_1/Anna_Niukkanen_task_1/images/check_status_of_manager.png)

Name node:

![Name Node](https://github.com/Annassie/BigData-Hadoop/blob/Anna_Niukkanen_task_1/Anna_Niukkanen_task_1/images/nameNode.png)

Data Node:

![Data Node](https://github.com/Annassie/BigData-Hadoop/blob/Anna_Niukkanen_task_1/Anna_Niukkanen_task_1/images/dataNode.png)

### 3. Stopping the cluster

https://github.com/Annassie/BigData-Hadoop/blob/Anna_Niukkanen_task_1/Anna_Niukkanen_task_1/images/stop_cluster.png
