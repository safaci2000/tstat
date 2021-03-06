## 2019 FEB WEEK THIRD

#### Things to do

- [x] Rewrite the README.md file.

  I rewrote the tstat/src/process/README.md file.
  
- [x] Pull & Request to master branch.

- [x] Skip the port number 22 in progress file.

- [x] Total number of processed lines is written in progress file.

- [ ] Fix query in Grafana.

	I found it can be more efficient to use 'custom all value' in variable. When user select 'ALL' and suppose I set the 'custom all value' as 80 in port dashboard, then the dashboard display the data points where port number is 80. But, I can't adapt to it. I fix the query that it can extract the value of data just over than zero. And I understood there's no reason to use aggregation function but without aggregation function, I can't grouping the graphs. I have tried to fix it for a two weeks, but the result of searching on google is same.  

- [x] Change 'classes' to 'python codes' in tstat/src/process/README.md

- [x] 'Naming Schema' go in 'python codes' in tstat/src/process/README.md

- [x] Write how to install Grafana in setup.

- [x] Write what user needs to input in config.py in tstat/src/process/README.md

- [x] Clearfy the environment that commands is run in tstat/src/process/READM.md. (Local or Server)

- [x] Write example the run tstat_to_influx.py command in tstat/src/process/REAMD.md

- [x] Write how to create dashboard (veirfy)

- [x] Process the exception when program run the curl command through 'os.system' function.

	If the return value of os.system is zero, there's no error in running command. But the other value is returned, it means there's a error.


Write a summary

1. what do you think about this project: was it useful, too long, too short, too difficult, etc

 The project was very useful to me because I haven't ever handled the huge data like this. In previous, the max number of data that I handled is just about 200. So, I learned the importance of coding the program efficiently. 

2. what did you learn that you did not know before and how can you apply what you learned in another project

 I learned about the influxDB and visualization platform (Chronograf and Grafana). I had thought that query of mySQL DB would be similar to query of influxDB. But, influxDB is based on serial data and use the tag key and field. So, first I was confused about the difference between tag and field in influxDB query but after I understood, I think it's useful.
 
 If I do the project which is important to handle data based on time, I can use the influxDB. And the writting documentation skill I learned during this project is very useful to me.

3. what goals did you accomplish and what goals are left for the future

- What goals did I accomplish

   Shorten time to process and insert into DB than previous.

   Move the visualization platform to Grafana.

   Learn how to write the documentation easy to view.

- What goals are left for the future

   More exact know about aggregation function to display the data points in Grafana.

   Shorten time to process and insert into DB less than 3 min.

   Visualize the data point by each port number group and each host ip address group. For example, group by 80, 100~199, 200~299, etc in port and by 110.xxx.xxx.000~110.xxx.xxx.255 and etc in host.
