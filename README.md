# Project Title

Database Design & Application 

## Introduction
In this project, we design a database application. We use the phpPgAdmin as our DBMS. The web server is Apache Web Server. The database server is PostgreSQL.  

## Getting Started

### Prerequisites

Download the AWS tool MAPP or use the installer (https://bitnami.com/stack/mapp/installer)
included in this directory if using a mac.

### Installing

1. Open AWS tool MAPP installer, start with installation.
Note: Install all the components 
<img width="607" alt="screen shot 2018-12-04 at 12 02 39 am" src="https://user-images.githubusercontent.com/36175498/49427413-1bc6db80-f758-11e8-9a7a-f74cb764e2dc.png">

2. Set the path for MAPP, since you are going to put html packages and run the AWS through this folder, pick a easy one.
<img width="469" alt="screen shot 2018-12-04 at 12 06 06 am" src="https://user-images.githubusercontent.com/36175498/49427717-ed95cb80-f758-11e8-9c21-e5ec6c26d85d.png">

3. Set the web server port, which is going to be used for access the web page on localhost. For example, my port# is 8080, then, when I access web pages on local host, the link looks like “http:// 127.0.0.1:8080/COEN280/businessrule.html”
<img width="475" alt="screen shot 2018-12-04 at 12 10 08 am" src="https://user-images.githubusercontent.com/36175498/49427814-2e8de000-f759-11e8-9360-1d39846108e3.png">

4. Set the database server port, which is going to be used to connect php DataBase Adaptor with the database server.
<img width="477" alt="screen shot 2018-12-04 at 12 12 39 am" src="https://user-images.githubusercontent.com/36175498/49427911-70b72180-f759-11e8-9227-4f930448ff00.png">
For example, my port# is 5433, so my connection looks like
<img width="270" alt="screen shot 2018-12-04 at 12 14 31 am" src="https://user-images.githubusercontent.com/36175498/49428038-d2778b80-f759-11e8-997c-f546779c3ca0.png">

5. Enter you password for default user in order to login the DB server, which also used for the DBAdaptor connection.
<img width="394" alt="screen shot 2018-12-04 at 12 17 14 am" src="https://user-images.githubusercontent.com/36175498/49428127-136fa000-f75a-11e8-8778-1fd079d40bc3.png">

6. Click next, skip the cloud part if you want, then, the installation starts.

7. Go to the folder you install the MAPP
<img width="228" alt="screen shot 2018-12-04 at 12 19 38 am" src="https://user-images.githubusercontent.com/36175498/49428293-7eb97200-f75a-11e8-83d6-f3d2c5bfe9a9.png">

8. Open the manager, and go to manage server page to start both PostgreSQL database server and AWS.
<img width="261" alt="screen shot 2018-12-04 at 12 22 06 am" src="https://user-images.githubusercontent.com/36175498/49428367-b9230f00-f75a-11e8-877c-1a8123960d9d.png">

9. Put the html files which is the directory called COEN280 into directory “apache2/htdocs” (the apache2 should be in the same directory with the AWS manager)
<img width="564" alt="screen shot 2018-12-04 at 12 23 52 am" src="https://user-images.githubusercontent.com/36175498/49428453-f5566f80-f75a-11e8-90f1-718d9b2d25e3.png">

10. open the browser and go to http://127.0.0.1:8080/phppgadmin/ to find the postgres admin for
this AWS. (If you are not using the web server port 8080, change 8080 to what ever port you used in step 3)
<img width="998" alt="screen shot 2018-12-04 at 12 26 13 am" src="https://user-images.githubusercontent.com/36175498/49428586-52522580-f75b-11e8-88a6-9dd9254e38f1.png">

11. login to the DBMS with the password set in step 5.
<img width="792" alt="screen shot 2018-12-04 at 12 28 44 am" src="https://user-images.githubusercontent.com/36175498/49428749-ba087080-f75b-11e8-896b-4040b71f51b4.png">

12. Click the postgres on left side and choose SQL code. Then, we either open the “Database.sql” file and copy paste all from that file to this input field or do the upload an SQL script under this field to load the “Data_query.sql”.
<img width="667" alt="screen shot 2018-12-04 at 12 31 22 am" src="https://user-images.githubusercontent.com/36175498/49428885-0358c000-f75c-11e8-967d-dd554d15b266.png">

13. Then, go to “project” schema you should be able to see all the tables.
<img width="842" alt="screen shot 2018-12-04 at 12 33 22 am" src="https://user-images.githubusercontent.com/36175498/49428984-487cf200-f75c-11e8-9824-507ebc63d2e1.png">


## Running the project

1. Make sure both of your AWS and Postgres server are running, and the COEN280 directory for html files are under correct directory as described in step 10. Open the browser and go to the link “http://127.0.0.1:8080/COEN280/index.html” (if your web server port# is not 8080, use your own port# replace 8080)
<img width="466" alt="screen shot 2018-12-04 at 12 36 32 am" src="https://user-images.githubusercontent.com/36175498/49429168-bde8c280-f75c-11e8-8d4c-e5cdfc810eaf.png">

2. Just in case you are using different database server port (mine is 5433), go to DatabaseAdaptor.php file and change the port number to your own port number. Also, change the user name, dbname, password to your own setting.
<img width="343" alt="screen shot 2018-12-04 at 12 38 04 am" src="https://user-images.githubusercontent.com/36175498/49429287-01433100-f75d-11e8-8c6c-d45efab250cf.png">

3. You should be ready to go. The application is divided into to html pages. The index.html tells all the Metric Report required in the Final project requirements. In this page, enter the query number from 1-14 to see all metric report for project requirement which based on our schema design. The query 15 shows the report for “any person with his(her) all classes or project and resource used”, so you should enter a valid user id in the second field.
<img width="307" alt="screen shot 2018-12-04 at 12 40 22 am" src="https://user-images.githubusercontent.com/36175498/49429445-53845200-f75d-11e8-855c-2506fd594a1b.png">
<img width="358" alt="screen shot 2018-12-04 at 12 42 10 am" src="https://user-images.githubusercontent.com/36175498/49429526-81699680-f75d-11e8-8f96-186c8aeb73ad.png">

4. The second page which is businessrule.html. This page is making insertions to all these tables including the three business rules.

## Business rules (since the resource based database do not have space for the permission)

#1 Only the chairperson or the person with permission can add new jobs for user
#2 a student cannot have more than 3 active jobs in order not have too much course load, however, we can add job for student with the chairperson’s permission or the student is a honor student.
#3 Only the chairperson can add more project, but others may add project if he/she gets permission from the chair person

For rule 1 and 2:
<img width="530" alt="screen shot 2018-12-04 at 12 44 48 am" src="https://user-images.githubusercontent.com/36175498/49429657-e91fe180-f75d-11e8-81ef-0e2646cdcda2.png">


Check the box “Have permission?” to pass rule 1 to show you are the chairperson or you got the permission. Check the box “Honor student?” to show the user to be assigned with new job is an honor student who can afford such heavy work loads. The check for “if this user have more than three job” is included in DatabaseAdaptor.php function “public function get_Qij1” if you do not check the “Honor student?” check box.

For rule 3:



## Built With

* [Dropwizard](http://www.dropwizard.io/1.0.2/docs/) - The web framework used
* [Maven](https://maven.apache.org/) - Dependency Management
* [ROME](https://rometools.github.io/rome/) - Used to generate RSS Feeds

## Contributing

Please read [CONTRIBUTING.md](https://gist.github.com/PurpleBooth/b24679402957c63ec426) for details on our code of conduct, and the process for submitting pull requests to us.

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/your/project/tags). 

## Authors

* **Billie Thompson** - *Initial work* - [PurpleBooth](https://github.com/PurpleBooth)

See also the list of [contributors](https://github.com/your/project/contributors) who participated in this project.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* Hat tip to anyone whose code was used
* Inspiration
* etc
