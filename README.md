# YouTube-Data-Analysis


YOU TUBE DATA ANALYSIS USING MAP REDUCE

Finding total no of vidoes uploaded in each category for given YouTube Dataset using MapReduce


           STEPS FOR RUNNING MAP REDUCE ON HADOOP CLUSTER

1.	Install Hadoop on your local machine.
                     I have installed single node Hadoop cluster on my machine.
                     
                  ![image](https://cloud.githubusercontent.com/assets/11257521/20969121/82d8065e-bc3c-11e6-944c-6fdaeac0f49d.png)
                  
                  


                  ![image](https://cloud.githubusercontent.com/assets/11257521/20969866/c5d52010-bc3f-11e6-8290-2836ddc66251.png)
                  
                  
                  
                  
                  ![image](https://cloud.githubusercontent.com/assets/11257521/20969898/e8cbe112-bc3f-11e6-9aae-64196d6008e5.png)
                  



              1.	Create a new user directory in your HDFS.
hadoop fs –mkdir/rucha

2.	Create two folders named input and output directories.
           hadoop fs –mkdir/rucha/input
           hadoop fs –mkdir/rucha/output




3.	Download Youtube Data set from  http://netsg.cs.sfu.ca/youtubedata/  and save it to desktop as youtube.txt
4.	Now put that youtube data set into HDFS’s input folder using flowing command
Hadoop dfs –copyFromLocal  users/ruchit/Desktop/youtube.txt  /rucha/input/
5.	Go to Eclipse and copy following Map Reduce program and generate jar file for it . and save that jar file to your desktop
6.	Now run that jar file
7.	Before that delete 
8.	zip -d jarfile.jar META-INF/LICENSE
hadoop jar /users/ruchit/Desktop/YouTubeJob1.jar   /rucha/input/youtube.txt /rucha/output/youtubeview/

Now run this command and output for map reduce job will be stored at /rucha/output/youtubeview/part_00000.txt

      

![image](https://cloud.githubusercontent.com/assets/11257521/20969925/0eab0836-bc40-11e6-857e-75892090bac6.png)



Now Hadoop starts executing its Map Reduce Task. First  Mapper will run and then reducer will start




![image](https://cloud.githubusercontent.com/assets/11257521/20969950/324ee1c2-bc40-11e6-84ea-49984f2f526e.png)




![image](https://cloud.githubusercontent.com/assets/11257521/20969967/438a299c-bc40-11e6-9f7e-3cbbc8d8ee4f.png)





HDFS Directory which shows  output of Map Reduce job  in localhost


![image](https://cloud.githubusercontent.com/assets/11257521/20970006/5efed47a-bc40-11e6-80ef-53120aee32d8.png)





![image](https://cloud.githubusercontent.com/assets/11257521/20970018/6c852626-bc40-11e6-9453-74d92ce19ead.png)




Output for map reduce jobs


![image](https://cloud.githubusercontent.com/assets/11257521/20970043/89a5e6c8-bc40-11e6-8d82-b78290ac9a86.png)
















