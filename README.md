# Ex-04_RESTful_Web_Services
## Aim:

To create, deploy and execute RESTful Web service programs using Server, Client and Client-Side remote invocation
## Procedure:

### Server side:
#### Step 1: 
Create a new Java Web Project. Follow Steps 1-5 as in SOAP Based Web Service.
#### Step 2: 
Right-click on the project name and select New->RESTful Web Services from Patterns.
![image](https://github.com/danush564/Ex-04_RESTful_Web_Services/assets/98585166/ea55c753-d327-4f07-a839-2bad22e7719d)

#### Step 3: 
A new window will appear. Select “Simple Root Resource” and click Next.
![image](https://github.com/danush564/Ex-04_RESTful_Web_Services/assets/98585166/c60468c5-3069-4757-8f19-dec7bbc41eb6)

#### Step 4: 
In the next window, give a Resource Package name and choose MIME Type as “text/html”. Click Finish.

![image](https://github.com/danush564/Ex-04_RESTful_Web_Services/assets/98585166/62ab70ee-dcb9-43db-a35b-2eb062a942ae)

#### Step 5: 
Two editing tabs will appear. Close “ApplicationConfig.java”. You need to write all your required functionalities in GenericResource.java.

#### Step 6: 
Alter getHtml() method as shown below.

#### Step 7: 
Save your project, clean and build it. Deploy your project.
![image](https://github.com/danush564/Ex-04_RESTful_Web_Services/assets/98585166/66cbead3-50e3-4a16-ac5e-500b9a75c444)

#### Step 8: 
To test your web service, open a new browser window/tab and type the URL as http://localhost:8080/project_name/webresources/generic?params=45&params=35 and hit enter. (This is the easiest way of testing the web service when it makes use of List).

### Client-Side:


#### Step 1: 
Create a new Java Web Project. Follow steps 1-5 as in section 1.1.
#### Step 2: 
Right-click on the project and select New->RESTful Java Client.
![image](https://github.com/danush564/Ex-04_RESTful_Web_Services/assets/98585166/f183e43c-75b6-46a7-96a9-076b14f250f0)

#### Step 3: 
A new window will appear. In that, give a name to your client, a package name and select “From Project” under the “Select the REST resource:” tab and click Browse. 

#### Step 4: 
Carefully select your RESTful resource (web service) and click OK.
![image](https://github.com/danush564/Ex-04_RESTful_Web_Services/assets/98585166/0dbe82b6-b073-4491-b33c-9b3b7e7b0628)

#### Step 5: 
Once everything is filled, the New RESTful Java Client window should look like this. Click Finish.
![image](https://github.com/danush564/Ex-04_RESTful_Web_Services/assets/98585166/5d1bebe1-a642-4bc9-b097-5f5f3a9623a6)

#### Step 6: 
An editing tab will open. Alter getHtml() method with the following.
![image](https://github.com/danush564/Ex-04_RESTful_Web_Services/assets/98585166/a9a8f3c0-5c8a-405c-bbc8-4917fa8e9848)

#### Step 7: 
Right-click on the Libraries folder under your project and select “Add JAR/Folder”.
![image](https://github.com/danush564/Ex-04_RESTful_Web_Services/assets/98585166/f391e644-b35b-4191-8e9a-6d29a35d2f99)

#### Step 8: 
A new window will appear. Navigate to the folder where you have placed the “javax.ws.rs-api2.0.1.jar” file and select Open.
![image](https://github.com/danush564/Ex-04_RESTful_Web_Services/assets/98585166/7526450c-29a8-4bf3-a327-d86946d355d6)

 


#### Step 9:
Right-click on the Web Pages folder and select JSP. In the new window, give a name to the JSP page and click Finish.
![image](https://github.com/danush564/Ex-04_RESTful_Web_Services/assets/98585166/842b7ab1-c3d3-417e-8170-aaf089443a48)

#### Step 10: 
A new tab will appear with the default contents of the JSP page. In that, include at the top and type the following code to invoke the client java code.


#### Step 11: 
Save the project and build it.
#### Step 12: 
Run the JSP file and you should see the output in a new browser window.
![image](https://github.com/danush564/Ex-04_RESTful_Web_Services/assets/98585166/922906d2-f5ee-4d0c-8684-18f1f7a44721)


### Client-Side Remote Invocation:


#### Step 1: 
Follow steps 1-5 as in Section 2.2
#### Step 2: 
In the generated NewJerseyClient.java file, Replace BASE_URI from private static final String BASE_URI = "http://localhost:8080/RESTful_Server/webresources"; TO private static final String BASE_URI = "http://192.168.116.62:8080/RESTful_Server/webresources";
#### Step 3: 
Follow steps 6-12 as in Section 2.2


## Result:
 Thus, the RESTful web service program has been successfully created and executed.
