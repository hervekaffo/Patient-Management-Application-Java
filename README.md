# Patient-Management-Application-Java
Patient Management System to help health care providers to add a new patient's condition or see some preview conditions of the patient. It was implemented using Netbeans and Sqlite
Author : Herve Taning Kaffo. 


1.	How to compile and run the project
This project folder will contain 3 java files (Login.java, Main_Windows.java, EmailValidator.java) the Database file (PHCP_DB.sqlite), the logo image (logo.png) and the SQLite driver for windows (sqlite-jdbc-3.8.11.2.jar) since our program connect to a SQLite Database.  
Our start page is the login page, so you simply need to compile it first using the command: 

javac Main_Windows.java 
 
To run the program you need to indicate to the compiler the path of the SQLite driver, since it is located in the same folder, the command to run the program will be

java -classpath ".;sqlite-jdbc-3.8.11.2.jar" Main_Windows
 
 
	You can login to the application using the information below: 
	Username: 123
	Password: 123
Then press Enter or click the Login button.
 
Navigate and manipulate the data using the tabs of the project frame.  To logout, go to 
File  Logout
2.	Goal of this application 
	The Goal of this application is to provide to a healthcare provider before any medical intervention: 
-	 Some important information about a Patient, the name, date of birth, address, and contact information.
-	Information about the patient’s blood anatomy : type, HIV status 
-	Some medical intervention the patient have received and their result
-	The type of medication the patient is on
-	Some feedbacks of the other health care provider who made some medical intervention on the patient.
Record the medical intervention the healthcare provider will issue, update or remove some information in the patient medical record. 

3.	Structure of the application 
This program is a windows desktop application connecting to a SQLite Database to register or manipulate the personal healthcare information for a specific patient. 
The program has 2 frames: the Login and the Main Windows.  The Main Windows has 5 tabs: the first and the main tab is for the personal information of the patient, the second tab is for the Patient blood information, the third tab is for the Medication (If the patient is in any kind of medication), the fourth tab is for the patient actual condition and the last tab is for the health care provider information.
The database has 5 tables corresponding to each tab of the Main Windows and one table to register the user’s username and passwords; the tables are: 
-	Patient: 
 



-	Details :
 
-	Medication
 
-	Condition 
 





-	Care_Provider
 

We used Mozilla Firefox SQLite Database management plugin to manage our database (Create tables, enter some information for testing purposed, see the tables structures and fields or tables specifications). 

4.	Functionalities implemented in the application
	Working functionalities implemented in the rapid PHCR Program:
Connection to a SQLite database; this is represented as a file named PHCP_DB.sqlite. The name of the Database is PHCP_DB and we created the six tables listed above. To work with the database, you need to connect to it first: java use a driver and a connection String to connect to a database. 
The main windows offers 5 tabs specific to a type of information you need to manipulate. And in each tab, you can add, observe, update, and delete information using the buttons and the Jtable. 



-	The tab Personal Information : 
 
-	The tab Blood Detail: 
 
-	The Tab Medication
 
-	The Tab Condition 
 
-	
-	The Tab Primary Care Provider
 

-	We have also implemented some functionalities like the Date and the email validation, and the phone number formatter.  
-	We have also warned the user before deleting data 
-	And we have made sure that there are a certain coordination between the data the user will enter: for example if a patient is HIV positive, he cannot be am organ donor, this can also be specific to his blood group. 

5.	Conclusion 
This project implements the most usual functionalities we encounter in the software engineering. We have a software side and the database side and connect the both to manipulate data. 
We learned how to use a lot of java libraries and how to manipulate external information using swing libraries. Since that we used java to write this code, we can transform it into a web or a mobile application by just implementing some integration to our program. 

feel free to bring any suggestions or improvements
kaffo80@gmail.com


 

