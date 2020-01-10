# Udacity_Disaster-Response-Pipeline

During disaster, it may not be easy to identify appropriate relief agency apart from chief responsible parties though correct identification relieft agency can shorten communication time and help effective militation of the subsequent problems. 
For instance, during outbreak of fire, there may be needs for clearance of obstacles to incident areas, emergent supply of medicine and fresh water, truncation of power supply, and etc.
Main part of this repository is a data set containing real messages that were sent during disaster events with identification of appropriate relief agencies, a machine learning model for this purpose and a web app which can help further identication of relief agencies when message is input.

![alt text](https://github.com/nigellmo/Udacity_Disaster-Response-Pipeline/blob/master/master_html.PNG)


![alt text](https://github.com/nigellmo/Udacity_Disaster-Response-Pipeline/blob/master/go_html.PNG)

## Running Instructions
1. Save **disaster_categories.csva**,**disaster_messages.csv** and **process_data.py** under data folder in the working directory. Command "python python process_data.py disaster_messages.csv disaster_categories.csv DisasterResponse.db" to export data to a database file named "DisasterResponse.db" under the same working directory.
2. Command "python train_classifier.py ../data/DisasterResponse.db classifier.pkl" to train up the machine learning model and save in a pickle file named "classifier.pkl" under the same working directory.
3. Go to app folder and command "run.py" which will utilize "DisasterResponse.db" and "classifier.pkl" to acticate the web application. (For Udacity Student, open separate terminal window and type env|grep WORK to get SPACEID and SPACEDOMAIN,and the URL that will be https://SPACEID-3001.SPACEDOMAIN)
