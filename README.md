/** This is a simple project for Email Configuration */
/** Please pre-install PostgreSql before follow the steps bellow, you can check this tutorial : https://youtu.be/fZQI7nBu32M

/*If you want to follow the code you simple follow the steps bellow */

1) Install Intellij Idea for run the project. (You can choose what ever you like, but intellij is an easy full-build environment)

2)Clone this current project (Open your terminal and write this command  -> git clone https://github.com/SylvanasGr/RegLoginProject.git  OR  go to intellij file>new>Project from Version Control

2a) go to application.yml and connect your postgre database and if you have error still error with lombook install this dependency at your pom.xml file:

<dependency>
  <groupId>org.projectlombok</groupId>
  <artifactId>lombok</artifactId>
  <version>1.18.22</version>
</dependency>

and you're api is good :) !

3) You also need to install Postman and NodeJs and PostGre

4)Then open NodeJs and run the command -> node -v ( This command must show you the version of your nodeJs, if it throws you an error you need  to install nodeJs again,you can check this video: https://www.youtube.com/watch?v=__7eOCxJyow&ab_channel=ProgrammingKnowledge2)

5)After you successfully installed node js you need to run this command -> npm install -g maildev

6)After all the steps :

	open a tab for your backend(Intellij): http://localhost:8080
	for your postman(Postman) and send a Post Request at: http://localhost:8080/api/v1/registration
	for postman you need this format(choose body->raw>Json) :

		{
    			"firstName": "Konstantinos",
    			"lastName": "Kolios",
    			"email": "email@email.com",
    			"password":"password"
		}


	then open another tab at: http://localhost:1080

7)Press "Confirm your Email" and then press "Click Here"  and you can log in successfully to the localhost:8080 (you should see Whitelabel Error Page , because i dont have build the view yet ! :D )

/** Please send me message at KonstantinosKolios@windowslive.com if you have technical issues :) ! */
