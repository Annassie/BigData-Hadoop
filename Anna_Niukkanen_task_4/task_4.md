1. Install Apache Hive in your Apache Hadoop container

Installing HIVE into container and unziping:

Install: wget https://apache-mirror.rbc.ru/pub/apache/hive/hive-2.3.9/apache-hive-2.3.9-bin.tar.gz

Unzip: tar xzf apache-hive-2.3.9-bin.tar.gz 

![Installing HIVE](https://github.com/Annassie/BigData-Hadoop/blob/Anna_Niukkanen_task_4/Anna_Niukkanen_task_4/screenshots/install_hive.png)

Removing .tar.gz:

![Installing HIVE](https://github.com/Annassie/BigData-Hadoop/blob/Anna_Niukkanen_task_4/Anna_Niukkanen_task_4/screenshots/remove_tar_gz.png)

Then adding into .bashrc-file:

![Installing HIVE](https://github.com/Annassie/BigData-Hadoop/blob/Anna_Niukkanen_task_4/Anna_Niukkanen_task_4/screenshots/bashchange.png)

2. Download the lego-database dataset and import it into Hive
4. Write a query that will display the name of the set (sets.name) with the largest number of parts (sets.num_parts)
5. Compose a query that will display in which year (sets.year) the most sets were released
6. Write a query that will display the total number of parts (inventory_parts.quantity) for each of the colors (colors.name)
7. Modify the Dockerfile so that Hive is installed and launched with Hadoop *
