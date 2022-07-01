### 1. Install Apache Hive in your Apache Hadoop container

Installing HIVE into container and unziping:

Install: wget https://apache-mirror.rbc.ru/pub/apache/hive/hive-2.3.9/apache-hive-2.3.9-bin.tar.gz

Unzip: tar xzf apache-hive-2.3.9-bin.tar.gz 

![Installing HIVE](https://github.com/Annassie/BigData-Hadoop/blob/Anna_Niukkanen_task_4/Anna_Niukkanen_task_4/screenshots/install_hive.png)

Removing .tar.gz and renaming .bin-file:

![Installing HIVE](https://github.com/Annassie/BigData-Hadoop/blob/Anna_Niukkanen_task_4/Anna_Niukkanen_task_4/screenshots/remove_tar_gz.png)

Then we always need to declare necessary environment HOME-variables for utilities:

export HIVE_HOME=/home/hduser/hive

And for using HIVE-tools, add Path to HIVE:

export PATH=$PATH:$HIVE_HOME/bin

But when we Exit the hduser@localhost, this installions will lose and we need to declare them again while the next session.

If we don't want to declare them every bash-session, we can add them into .bashrc-file (Shift+G -> go to the end of the file):

![Installing HIVE](https://github.com/Annassie/BigData-Hadoop/blob/Anna_Niukkanen_task_4/Anna_Niukkanen_task_4/screenshots/bashchange.png)



### 2. Download the lego-database dataset and import it into Hive

Downloading and moving lego-dataset to docker:

![Moving lego-dataset to docker](https://github.com/Annassie/BigData-Hadoop/blob/Anna_Niukkanen_task_4/Anna_Niukkanen_task_4/screenshots/download_lego.png)

To run Hive Server in the background:
      $ hiveserver2 &> /dev/null&

Then we connect via beeline cli: /n
      $ beeline -u jdbc:hive2://localhost:10000 

Creating lego_sets- and lego_themes_tables:

![Creating lego_sets- and lego_themes_tables](https://github.com/Annassie/BigData-Hadoop/blob/Anna_Niukkanen_task_4/Anna_Niukkanen_task_4/screenshots/tables_creating.png)


Loading data from dataset into lego_sets- and lego_themes_tables:

![Loading sets data into lego_sets-table](https://github.com/Annassie/BigData-Hadoop/blob/Anna_Niukkanen_task_4/Anna_Niukkanen_task_4/screenshots/data_sets.png)

![Loading sets data into lego_themes-table](https://github.com/Annassie/BigData-Hadoop/blob/Anna_Niukkanen_task_4/Anna_Niukkanen_task_4/screenshots/load_data_themes.png)

### 3. Write a query that will display the name of the set (sets.name) with the largest number of parts (sets.num_parts)
### 4. Compose a query that will display in which year (sets.year) the most sets were released
### 5. Write a query that will display the total number of parts (inventory_parts.quantity) for each of the colors (colors.name)
### 6. Modify the Dockerfile so that Hive is installed and launched with Hadoop *
