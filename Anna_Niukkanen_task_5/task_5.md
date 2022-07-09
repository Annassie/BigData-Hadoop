### Task 5

#### 1. Create a lego_inventory_parts_cut table without STRING columns

Creating lego_inventory_parts_cut-table and inserting data into it from lego_inventory_parts-table:

![Creating lego_inventory_parts_cut-table](https://github.com/Annassie/BigData-Hadoop/blob/Anna_Niukkanen_task_5/Anna_Niukkanen_task_5/screenshots/create_parts_cut.png)

![Inserting data into table](https://github.com/Annassie/BigData-Hadoop/blob/Anna_Niukkanen_task_5/Anna_Niukkanen_task_5/screenshots/insert_data_to_parts_cut.png)

#### 2. Compare the compression ratio (ratio of uncompressed file to compressed file) of a table that has STRING columns with a table without columns of this type

First creating and zipping table into PARQUET

***Parquet SNAPPY***

![Parquet Snappy](https://github.com/Annassie/BigData-Hadoop/blob/Anna_Niukkanen_task_5/Anna_Niukkanen_task_5/screenshots/cut_par_snappy.png)

***Parquet GZ**

![Parquet GZ](https://github.com/Annassie/BigData-Hadoop/blob/Anna_Niukkanen_task_5/Anna_Niukkanen_task_5/screenshots/cut_par_gz.png)

***And Parquet RAW**

![Parquet RAW](https://github.com/Annassie/BigData-Hadoop/blob/Anna_Niukkanen_task_5/Anna_Niukkanen_task_5/screenshots/cut_par_raw.png)

Second creating tables in ORC:

***ORC Snappy**

![ORC Snappy](https://github.com/Annassie/BigData-Hadoop/blob/Anna_Niukkanen_task_5/Anna_Niukkanen_task_5/screenshots/cut_orc_snappy.png)

***And ORC RAW**

![Orc raw](https://github.com/Annassie/BigData-Hadoop/blob/Anna_Niukkanen_task_5/Anna_Niukkanen_task_5/screenshots/cut_orc_raw.png)

And the last one is creating table in Avro:

![Avro](https://github.com/Annassie/BigData-Hadoop/blob/Anna_Niukkanen_task_5/Anna_Niukkanen_task_5/screenshots/cut_avro.png)

And then we can compare the comprassion of them:

![Comprassion ratio](https://github.com/Annassie/BigData-Hadoop/blob/Anna_Niukkanen_task_5/Anna_Niukkanen_task_5/screenshots/check_size.png)

Based on it, it is possible to say that the comprassion of files without STRING columns takes almost two times less than the comprassion of files with STRING columns.

#### 3. Write the differences and similarities between AVRO and CSV formats in relation to each other
