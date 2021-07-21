### https://github.com/kishan0725/Hospital-Management-System

## E-Commerce Website: CoviTech
E-Commerce Website using MySQL, Php and Bootstrap





## Need to work on:

1. Ability to accept the appointment by the doctor to acknowledge the patient that their appointment has been approved.
2. User should not be allowed to register if he/she tries to provide the already registered email ID.
3. The password should be encrypted and the password field shouldn't be displayed in the admin panel.
4. Implementation of pagination for all the list view across the application.
5. Bug fix - Bill payment receipt contains multiple record if the patient has associated with the same doctor multiple times.
6. Addition of more fields in the prescription statement to make it more specific one.
7. Addition of more details on payment - such as date of the payment made, amount paid, etc.
8. Implementation of export button in admin module to export all details to an excel sheet.

## Prerequisites
1. Install XAMPP web server
2. Any Editor (Preferably VS Code or Sublime Text)
3. Any web browser with latest version

## Languages and Technologies used
1. HTML5/CSS3
2. JavaScript (to create dynamically updating content)
3. Bootstrap (An HTML, CSS, and JS library)
4. XAMPP (A web server by Apache Friends)
5. Php
6. MySQL (An RDBMS that uses SQL)

## Steps to run the project in your machine
1. Download and install XAMPP in your machine
2. Clone or download the repository
3. Extract all the files and move it to the 'htdocs' folder of your XAMPP directory.
4. Make a new folder 'project' in the 'htdocs' folder of your XAMPP directory. Extract all the files and move it to this folder.
6. Start the Apache and Mysql in your XAMPP control panel.
7. Click on Admin button in the Mysql Module. Alternatively you can open your web browser and type 'http://localhost/phpmyadmin/'

### Database Creation Instruction

9. In phpmyadmin page, create a new database from the left panel and name it as 'project'.

#### Creating Table "users":
11. In this 'project' database, click on "New" button.
12. On the navigation bar click on SQL, paste the following SQL commands and click on Go.

`````````````````````````````````````````````````````
CREATE TABLE `users` (
  `id` int(11) NOT NULL AUTO_INCREMENT PRIMARY KEY,
  `firstname` varchar(100) NOT NULL,
  `Lastname` varchar(100) NOT NULL,
  `gender` varchar(100) NOT NULL,
    `DOB` date NOT NULL,
    `email` varchar(100) NOT NULL,
    `password` varchar(100) NOT NULL,
    `num` int(11) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=latin1;
`````````````````````````````````````````````````````

#### Creating Table "admin":
12. In the 'project' database, again click on "New" button.
12. On the navigation bar click on SQL, paste the following SQL commands and click on Go.

`````````````````````````````````````````````````````
CREATE TABLE `admin` (
  `id` int(11) NOT NULL AUTO_INCREMENT PRIMARY KEY,
  `username` varchar(100) NOT NULL,
  `password` varchar(100) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=latin1;

`````````````````````````````````````````````````````

#### Creating Table "testing":
13. In the 'project' database, again click on "New" button.
14. On the navigation bar click on SQL, paste the following SQL commands and click on Go.

`````````````````````````````````````````````````````
CREATE TABLE `testing` (
  `id` int(11) NOT NULL AUTO_INCREMENT PRIMARY KEY,
  `Product` varchar(100) NOT NULL,
  `Price` int(11) NOT NULL,
  `Email` varchar(100) NOT NULL,
    `Quantity` int(11) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=latin1;

`````````````````````````````````````````````````````

#### Creating Table "orders":
15. In the 'project' database, again click on "New" button.
16. On the navigation bar click on SQL, paste the following SQL commands and click on Go.

`````````````````````````````````````````````````````
CREATE TABLE `orders` (
  `id` int(11) NOT NULL AUTO_INCREMENT PRIMARY KEY,
  `Product` varchar(100) NOT NULL,
  `Price` int(11) NOT NULL,
  `Email` varchar(100) NOT NULL,
  `Quantity` int(11) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=latin1;
`````````````````````````````````````````````````````

<img src="https://user-images.githubusercontent.com/78657875/126182991-e9cd47f3-b231-44e7-a119-8f3b34e25f59.png" width="180" height="200" />

NOTE: EVERYTHING IS CASE SENSITIVE


14. Open a new tab and type 'http://localhost/project/index.php' in the url of your browser
15. Hurray! That's it!
    
### SOFTWARES USED
  - XAMPP was installed on windows and APACHE Server and MySQL were initialized. And, files were built inside C:\xampp\htdocs\project.
  - VS Code was used as a text editor.
  - Google Chrome Version 91.0.4472.124 was used to run the project.
  

### Starting Apache And MySQL in XAMPP:
  The XAMPP Control Panel allows you to manually start and stop Apache and MySQL. To start Apache or MySQL manually, click the ‘Start’ button under ‘Actions’.

<p align="center"><img src="https://user-images.githubusercontent.com/78657875/126271652-4edbcff2-deb4-41c2-9bcc-426576154549.png" width="490" height="320" />  
	
## GETTING INTO THE PROJECT:
	
### Home Page:
This website has a ‘Home’ page which contains links to the following from where the user & admin can login into their accounts by toggling the tabs accordingly. Fig 1.1 shows the ‘Home’ page of our project.

This is the 'Home' page of our website. (Fig 1.1)
	
![image](https://user-images.githubusercontent.com/78657875/126287259-333c4540-d5a9-41a4-9e03-0e0a5dd268ed.png)
	
It contains following sections:-

A) Services (Fig 1.1.1)
	
B) Live Updates (Fig 1.1.2)
	
C) Useful Youtube Videos (Fig 1.1.3)

### Services: 
This Section (in the home page itself) contains link to various services like Register for Vaccine, donate to PM Care Fund, find nearest vaccination center and read information about COVID-19 and its prevention.
	
![image](https://user-images.githubusercontent.com/78657875/126288270-d9f70962-185c-451e-b062-3f9eb973ace9.png)

### Live Updates:
This Section (in the home page itself) displays (COVID-19) statistics of confirmed Covid Cases, Deaths and number of people vaccinated. The user can select any country and can also compare covid cases by region.
	
![image](https://user-images.githubusercontent.com/78657875/126289050-0b69d131-1e1c-4aad-9966-4bae9bc0132a.png)

### USEFUL YOUTUBE VIDEOS:
This Section (in the home page itself) displays various embedded Youtube videos on Symptoms, Precautions and Prevention of Coronavirus.

![image](https://user-images.githubusercontent.com/78657875/126289294-558c67d8-a13a-4587-99f4-f9df042a82b5.png)

<h2 align = "center">About Us</h2>
'About Us' page (Fig 1.2) allows us to get some more information about goals and the services of our E-commerce website.
	
![image](https://user-images.githubusercontent.com/78657875/126289979-6b986ef7-9608-499c-9239-e2ee8976ae45.png)

The website consists of 2 modules:

1. User Module
2. Admin Module

## User Module:

This module allows customers to create their account, login to their account, view products, add/delete products to their cart and place/cancel their orders.

### Registration Page

The registration page asks customers to enter their First Name, Last Name, DOB, Email Address, Password, Home Address, Phone Number, and radio buttons to select their gender.

![image](https://user-images.githubusercontent.com/78657875/126368397-ae9f69f3-cef3-415d-b151-2c9071ae4938.png)

### Login Page

Once the user has created his/her own account after clicking the ‘Register’ button, then he/she will be redirected to Login Page (Fig 1.5).

![image](https://user-images.githubusercontent.com/78657875/126290347-ef304607-3202-497e-996d-864a70a6108e.png)



![image](https://user-images.githubusercontent.com/78657875/126366865-496348ec-fa66-4ee5-8cb5-3ef8db2b7bf4.png)




	




![image](https://user-images.githubusercontent.com/78657875/126368896-fb81e26d-4e81-4a8f-a3c1-1cddd5438ca0.png)

![image](https://user-images.githubusercontent.com/78657875/126370427-c2a742f0-665c-448c-8375-d2953c93133f.png)
	
![image](https://user-images.githubusercontent.com/78657875/126373563-0f661675-9db1-4168-8376-b589536c9408.png)

![image](https://user-images.githubusercontent.com/78657875/126390486-53d6f78b-a00d-46ab-b351-fa3bcbe7c65b.png)

![image](https://user-images.githubusercontent.com/78657875/126390951-3eeccbb3-01e7-47db-981c-731506884a71.png)

![image](https://user-images.githubusercontent.com/78657875/126391158-50a23edd-c3e3-46c0-9bb5-12cf09793d88.png)


	







![image](https://user-images.githubusercontent.com/36665975/66569676-ad2d8800-eb89-11e9-94e5-ea407622a1fe.png)



![image](https://user-images.githubusercontent.com/36665975/66569816-f4b41400-eb89-11e9-9377-d9ce53ded088.png)

‘Contact’ page allows users to provide feedback or queries about the services of the hospital. Fig 1.3 shows the ‘Contact’ page.

![image](https://user-images.githubusercontent.com/36665975/66569890-157c6980-eb8a-11e9-9b2f-c0e8a6ef702e.png)


### Patient Module:

  &nbsp; &nbsp; &nbsp; This module allows patients to create their account, book an appointment to see a doctor and see their appointment history.
  The registration page(in the home page itself) asks patients to enter their First Name, Last Name, Email ID, Contact Number, Password and radio buttons to select their gender.
  
  ![image](https://user-images.githubusercontent.com/36665975/66570027-5b393200-eb8a-11e9-9e97-088630b5e583.png)

Once the patient has created his/her own account after clicking the ‘Register’ button, then he will be redirected to his/her Dashboard(Fig 1.5).

![image](https://user-images.githubusercontent.com/36665975/66570123-8c196700-eb8a-11e9-845f-ea02013f1d5c.png)

The Dashboard page allows patients to perform two operations:

**1. Book his/her appointment:**

  &nbsp; &nbsp; &nbsp; Here, the patients can able to book their appointments to see a doctor. The appointment form(Fig 1.6) requires patients to select the doctor that they want to see, Date and Time that they want to meet with the doctor. The consultancy fee will be shown accordingly to the patient as it was already determined by the doctor.

![image](https://user-images.githubusercontent.com/36665975/66570202-c256e680-eb8a-11e9-8839-6c7fef68ac4c.png)

After clicking on the ‘Create new entry’ button, the patient will receive an alert that acknowledges the successful appointment of the patient.(See Fig 1.7) 

![image](https://user-images.githubusercontent.com/36665975/66570280-ec100d80-eb8a-11e9-96c2-08e5441954d0.png)

**2. View patients’ Appointment History:**

  &nbsp; &nbsp; &nbsp; Here, the patient can see their appointment history which contains Doctor Name, Consultancy Fee, Appointment Date and Time.(See Fig 1.8).
	
![image](https://user-images.githubusercontent.com/36665975/66570349-0ea22680-eb8b-11e9-94fe-22a86070a274.png)

Once the patient has logged out of his account, if he wants to go into his account again, he can login his account, instead of register his account again. Fig 1.9 shows the login page.
Clicking on ‘Login’ button will redirect the patient to his dashboard page which we have seen earlier (Fig 1.5)

![image](https://user-images.githubusercontent.com/36665975/66570502-588b0c80-eb8b-11e9-88e3-5294ae896ace.png)

This is how the patient module works. On the whole, this module allows patients to register their account or login their account(if he/she has one), book an appointment and view his/her appointment history.

### Doctor Module:

  &nbsp; &nbsp; &nbsp; The doctors can login into their account which can be done by toggling the tab from ‘Patient’ to ‘Doctor’. Fig 1.10 shows the login form for a doctor. Registration of a doctor account can be done only by admin. We will discuss more about this in Admin Module.
  
![image](https://user-images.githubusercontent.com/36665975/66570609-8bcd9b80-eb8b-11e9-8099-9f285aa7fe0f.png)

Once the doctor clicking the ‘Login’ button, they will be redirected to their own dashboard which is shown in Fig 1.11

![image](https://user-images.githubusercontent.com/36665975/66570642-a0119880-eb8b-11e9-8d23-be898e1bfa29.png)

In this page, doctor can able to see their appointments which has been booked by the patients. Fig 1.12 shows the appointment of the doctor ‘Ganesh’ which has been booked by the patient ‘Kenny Sebastian’ (Fig 1.6). This means that the doctor ‘Ganesh’ will have an appointment with the patient ‘Kenny Sebastian’ on 10-10-2019 10AM. 

![image](https://user-images.githubusercontent.com/36665975/66570704-be779400-eb8b-11e9-92ae-21d8e0e4aba4.png)

In real-time, the doctors will have thousands of appointments. It will be easier for a doctor to search for appointment in the case of more appointments. To make it easier, I have a ‘Search’ box in the navigation bar (See Fig 1.12) which allows doctors to search for a patient by their contact number.
&nbsp; &nbsp; &nbsp; Once everything is done, the doctor can logout of their account. Thus, in general, a doctor can login into his/her account, view their appointments and search for a patient. This is all about Doctor Module.

### Admin Module:
   
   &nbsp; &nbsp; &nbsp; This module is the heart of our project where an admin can see the list of all patients. Doctors and appointments and the feedback/queries received from the ‘Contact’ page. Also admin can add doctor too. 
  &nbsp; &nbsp; &nbsp; Login into admin account can be done by toggling into admin tab of the Home page. Fig 1.13 shows the login page for admin.
  &nbsp; &nbsp; &nbsp; `username`: admin, `password`: admin123

![image](https://user-images.githubusercontent.com/36665975/66570795-e961e800-eb8b-11e9-94e2-79940ff1d45e.png)

On clicking the ‘Login’ button, the admin will be redirected to his/her dashboard as shown in 
Fig 1.14.

![image](https://user-images.githubusercontent.com/36665975/66570841-03032f80-eb8c-11e9-9cfc-62b6b869c918.png)

This module allows admin to perform five major operations:

**1. View the list of all patients registered:**

  &nbsp; &nbsp; &nbsp; Admin can able to view all the patients registered. This includes the patients’ First Name, Last Name, Email ID, Contact Number and Password. (See Fig 1.15).As like in doctor module, admin can also search for a patient by their contact number in the search box.
  
  ![image](https://user-images.githubusercontent.com/36665975/66571179-83c22b80-eb8c-11e9-8819-008cdd2b0c2e.png)
  
**2. View the list of all doctors registered:**

  &nbsp; &nbsp; &nbsp; Details of the doctors can also be viewed by the admin. This details include the Name of the doctor, Password, Email and Consultancy fees, shown in Fig 1.16. Searching for a doctor can be done by using the doctor’s Email ID in the search box.

![image](https://user-images.githubusercontent.com/36665975/66571329-a5bbae00-eb8c-11e9-89be-ce1a9c73e01b.png)

**3. View the Appointment lists:**

  &nbsp; &nbsp; &nbsp; Admin can also able to see the entire details of the appointment that shows the appointment details of the patients with their respective doctors. This includes the First Name, Last Name, Email and Contact Number of patients, doctor’s name, Appointment Date, Time and the Consultancy Fees. (See Fig 1.17). 
  
  ![image](https://user-images.githubusercontent.com/36665975/66571377-c3891300-eb8c-11e9-92d2-6755204564c7.png)
  
**4. Add Doctor:**

  &nbsp; &nbsp; &nbsp; Admin alone can add a new doctor since anyone can register as a doctor if we put this section on the home page. This form asks Doctor’s Name, Email ID, Password and his/her Consultancy Fees.(See Fig 1.18)
  
  ![image](https://user-images.githubusercontent.com/36665975/66571687-55911b80-eb8d-11e9-9859-54e15d4ad8a0.png)
  
  After adding a new doctor, if we check the doctor’s list, we will see the details of new doctor is added to the list as shown in the Fig 1.19
  
  ![image](https://user-images.githubusercontent.com/36665975/66571496-03e89100-eb8d-11e9-954e-7e3704bd0ca3.png)
  
**5. View User’s feedback/Queries:**

  &nbsp; &nbsp; &nbsp; Admin is allowed to view the feedback/Query that has been given by the user in the ‘Contact’ page (Refer Fig 1.3). This includes User’s Name, Email Id, Contact Number and the message(Feedback/ Query) as shown in the Fig 1.20.
  
  ![image](https://user-images.githubusercontent.com/36665975/66571573-27134080-eb8d-11e9-8c1f-191a9f491872.png)
  
  &nbsp; &nbsp; &nbsp; Taking everything into consideration, admin can able to view the details of patients and doctors, appointment details, Feedback by the user and can add a new doctor. Once everything is done, the admin can logout from his account.

## Updates

### 1. Cancel Appointments
	
   &nbsp; &nbsp; &nbsp; Patients and doctors can able to delete their appointments.
 
   ![image](https://user-images.githubusercontent.com/36665975/75169587-d0c72880-574e-11ea-9a9e-ba098c04e594.png)
    
  If the patient deletes the last record (for doctor Ganesh), then a label "deleted by you" will be displayed in the column 'Current Status' and the action will change to cancel state.
  
  ![image](https://user-images.githubusercontent.com/36665975/75169873-47642600-574f-11ea-8ca4-420b0dfd20c3.png)
  
  Now if we login to the doctor Ganesh's account and view his appointment details, then it will look like this:
  
  ![image](https://user-images.githubusercontent.com/36665975/75170076-9316cf80-574f-11ea-84ff-6a5976ce8179.png)
  
  Similarly doctors can also delete their appointments and patients can view their updated appointment details.
  
### 2. Remove Doctors by Admin

&nbsp; &nbsp; &nbsp; Admin can also delete the doctors from the system. This let admin to have more control over the system.

![image](https://user-images.githubusercontent.com/36665975/75170650-6d3dfa80-5750-11ea-8f05-455c7d704217.png)

### License
This project is licensed under the [MIT License](LICENSE)
  




