# **Car Maintenance Tracker** 
<img src="/assets/readmeAssets/car-mtn-tracker.jpg">

- - - -

## Project Live Link https://car-mtn-tracker.herokuapp.com/
The project is deployed and live on Heroku

- - - -
## Index

- [Introduction](#Introduction)
- [Project Motivation](#Project_Motivation)
- [UX](#UX) 
    - [User Stories](#User_Stories)
    - [Wireframes](#Wireframes)
- [Features](#Features)
    - [Existing Features](#Existing_Features)
    - [Future Enhancements](#Future_Enhancements)
- [Technologies Used](#Technologies_Used)
- [Testing](#Testing)
    - [UX Testing](#UX_Testing)
    - [Functional Testing](#Functional_Testing)
    - [User Testing](#User_Testing)
    - [Code Validation](#Code_Validation)
- [Deployment](#Deployment)
    - [Live Deployment](#Live_Deployment)
    - [Local Deployment](#Local_Deployment)
- [Database](#Database) 
- [Credits](#Credits)
    - [Content](#Content)
    - [Media](#Media)
    - [Acknowledgements](#Acknowledgements)

- - - -
## **<ins>Introduction</ins>**
This is the third of my milestone projects, as part of the Code Institute full stack developer course. The project is a car maintenance tracking tool. It has a front end using Flask framework, 
with Materlize CSS library for the majority of the styling. The project also contains, custom HTML, CSS & JavaScript.

## **<ins>Project_Motivation</ins>**

The car maintenance tracker site is designed to be an application that allows organisations or individuals to record and track maintenance carried out on their vehicles.
The system has two aspects to it;
1. User Side. <br>
    The user would have the ability to register a car(s) and input maintenance records for that car. 
2. Admin Side. <br>
    The administrator would have the ability to add Garages (which are approved for use) and deactivate them from user view if required. 

The concept was to create an application, that was easy to use, accessible on all device types and would require minimum training for users. 

## **<ins>UX</ins>**
For the UX, I choose the Materialize CSS library for the primary CSS elements, applying custom CSS where required. The design of the applications, was a minimalist design on white background. 
As the application is a functional one I felt the simpler design with minimal graphics was best. The app is used to input data (records), edit and view the records so I don't expect the 
user to be on the site longer than is necessary for them to complete the task. 
In the base HTML, a common header and footer is used, across all the pages, the only element that varies are the page links depending on the user type and session cookie. 

### <ins>User_Stories</ins>

**Fleet Owner;**
1. Having a fleet of company cars, I want a single tool, where all the maintenance records are logged.
2. Company cars are operated by employees, service & maintenance is arranged by employee, so they system should allow for the employee to input the records & update records.
3. There is a list of approved garages where service and maintenance can be carried out, a list of the garages should be available to the employee when entering the record and the list should be able to be updated by the admin. 

**Record Owner;**
1. Simple form when entering data. 
2. Ability to register a car to the system.
3. View the records entered by me, with the ability to view, edit & delete as required. 

**Site Administrator Owner;**
1. Ability to view all records entered in to the system. 
2. Access to add garages or edit the current list in the DB.
3. Ability to edit or delete records if required from the system.

### <ins>Wireframes</ins>
Linked below, wireframes for the individual pages of the site.

| Title | Link to Wireframe (pdf) |
| --- | --- |
| Wireframes | https://app.box.com/s/vv4zin9yayy6prcylrb7gz2zwltx4coz |

[Index](#Index)
- - - -

## **<ins>Features</ins>**
This section describes the features that are available in the current release of the application and planned features for future releases.

### <ins>Existing_Features</ins>

The initial deploy of the application comes with the following features,

**User;**
-   can register account
-   can register a car under their ID
-   can see all records they have created
-   can create, edit and delete a record for a registered car

**Admin**
-   can view, edit and delete all records
-   can add a garage to the database
-   can deactivate a garage (meaning it is no longer available for selection by user)
-   can reactivate a garage (making it available to user)

### <ins>Future_Enhancements</ins>

In addition to the existing features, some future planned features included.

**User;**
-   ability to change password
-   ability to update their contact e-mail
-   generate reports from the DB for their records
-   ability to remove registered car (without impacting records for that car)

**Admin**
-   ability to manage users, suspend, delete, update & force password reset.
-   generate reports for all records in the DB

[Index](#Index)
- - - -
## <ins>Technologies_Used</ins>
**Balsamiq**  https://balsamiq.com/wireframes/
- Basamiq was used in the design phase to create wireframes of the proposed web site.

**Github** https://github.com/
- Github is the repository used for version control & storage of the project.
- Github pages was used for the deployment of the site.

**Gitpod** https://www.gitpod.io/
- Gitpod was the IDE used for the development throughout the project.

**Heroku** https://id.heroku.com/login
- Heroku cloud used for hosting the live application

**MongoDB** https://www.mongodb.com
- MongoDB was used as the backend DB for the project

**Google Fonts** https://fonts.google.com/
- Google fonts provided fonts for the project (Roboto Condensed & Serrat)

**Materializec** https://materializecss.com/about.html
- CSS Framework

**Font Awesome** https://fontawesome.com/
- Icons used through the web site are sourced from Font Awesome

**W3C Validation Service** https://validator.w3.org/
- HTML & CSS code was checked on W3C validator at the end of the project.

**HTML Formatter** https://webformatter.com/html
- HTML code was run through HTML formatter to fix any indentation issues.

**JSHint** https://jshint.com/
- JavaScript code validate through JSHint

**ami.responsivedesign** http://ami.responsivedesign.is/#
- The project was tested on ami.responsivedesign
- image used in readme file was taken from ami.responsivedesign site

**w3schools** https://www.w3schools.com
- For additional code explanations & features to use.

[Index](#Index)
- - - -
## <ins>Testing</ins>

### <ins>UX_Testing</ins>
As part of the UX testing all pages were tested for the following criteria;
1. All pages renders on the device, with no obvious distortion.
2. All colours and text is consistent and displays well to the user
3. All links within the page work as expected
4. All fields, that should be accessible for editing / adding data work as expected
5. Any buttons on the page are accessible and displayed appropriately for the screen size.
6. Any other issues the tester sees related to UX. 

| Page | Desktop | Tablet | Mobile | Issues |
| --- | --- | --- | --- | --- |
| register | Pass | Pass | Pass | Link below register box failed on live site, link was for git pot test site.|
| login | Pass | Pass | Pass | Link below register box failed on live site, link was for git pot test site.||
| tracker | Pass | Pass | Pass | Some modifications were made to better display the lists. One column was removed from the list of records for display on mobile to improve the lay out|
| detailed information |Pass |Pass | Pass |The cards on the top of the page, were different sizes depending on the data from the record, set a min height to ensure they all remain the same height.|
| add record | Pass |Pass | Pass ||
| edit record | Pass | Pass | Pass ||
| manage garages | Pass | Pass | Pass ||
| add car | Pass |Pass | Pass | spelling error on text above form.|
| user profile |Pass | Pass | Pass ||

**Note:** Early in testing, it was obvious that there were issues with the site on a table device. 
Testing was suspended and all pages were updated with addition size for medium devices to improve the layout on a tablet device. 
Testing, was resumed after this fix was applied to all pages. 

[Index](#Index)
### <ins>Functional_Testing</ins>

**Register (register.html)**
| Test | Expected outcome | Results | Issues|
| --- | --- | --- | --- |
| Fields are accessible | Fields should accept data and validate for min requirements set. | Pass ||
| Register Button | Button should collect data from the form and create an account.<br> Data should be validated with DB to ensure userid does not already exist | Pass ||

**Login (login.html)**
| Test | Expected outcome | Results | Issues|
| --- | --- | --- | --- |
|Fields are accessible| The username and password accept data from the user | Pass||
|login Button | Button logs user on and presents message if there is an issue. Redirects user to profile page upon login | Pass||

**User profile (userprofile.html)**
| Test | Expected outcome | Results | Issues|
| --- | --- | --- | --- |
|Data Check | All data is correct for the logged in user | Pass||

**Maintenance Records (tracker.html)**
| Test | Expected outcome | Results | Issues|
| --- | --- | --- | --- |
|Check data is rederived and populated from DB| Results should include all cars registered to a user with a list of records for each car listed | Pass | Some UX detailed in UX Testing section|
|Test Details button | Button should launch detailed records page for selected record and populate all data | Pass | None|

**Service Record (detailed record.html)**
| Test | Expected outcome | Results | Issues|
| --- | --- | --- | --- |
|All data populates | Validate that all data is populating, the correct data is populating | Pass | None|
|Return Button | Return button should take the user back to the main record page |Pass||
|Edit Button | The edit button should take the user to the edit record page and populate the correct record information | Pass |Initial issues, with the two drop down menu, the options were populating but the information from the selected record was now <br> Updated to check the list of the selected data and mark as selected when found|
|Delete Button | Open a modal to confirm deletion | Pass| Note: Delete button does not process and DB action, it only launches the modal for confirmation.|
|Confirmation Modal<br>1. Confirm it opens correctly <br> 2. Test No button. <br> 3. Test yes button.<br> 4. Confirm the correct record is deleted and no other record is effected | Selecting No on the confirmation panel should return the user to the edit screen with no action taken <br> selecting yes should initiate the update to the DB to delete the record. The selected record should be removed from the DB.| Pass | Page & functions work as expected|

**Add Maintenance Record (addrecord.html)**
| Test | Expected outcome | Results | Issues|
| --- | --- | --- | --- |
|Drop down ??? Cars | Only cars registered to the a user should be shown in the list |Pass||
|Drop down ??? Garages | Only active garages should show in the list | Pass| One issue to resolve, Garages that were disabled, and should not be selectable where showing in the list. <br> updated to the DB query in Python to only pull records with active flag set.|
|Date Picker| Displays and allows date to be selected |Pass||
|Toggle Switch| Toggles on / off| Pass||
|+ - Buttons| Add / Remove lines from the detailed list section | Pass| Opted to hide the - (remove) button on load, as its only needed if user adds line they then want to remove.|
| Add Record Button| Collects all data & adds new record to the DB| Pass||

**Edit Record (edit_record.html)**
| Test | Expected outcome | Results | Issues|
| --- | --- | --- | --- |
|Fields accept data |data can be entered without issue |Pass| Had to fix issue on service cost field, it was only taking numbers but as field for cost, it needed to take up to two decimal places if required. <br> added step=".01" to the field.|
| Data| All record data is correctly entered to the form| Pass| See above for initial issue on reg no & garage fields|
|Editable | All data fields can be edited | Pass| All fields where tested to ensure they could be edited|
|Return Button | Returns user to detailed record page | Pass||
|+ / - buttons | Ensure buttons work to add remove lines | Pass| Save button, sent the edited data to the DB and updated the correct record|
|Save Change Button | Sends the updates to the DB and saves the updated record | Pass| Initially failed, <br> the initial page was a copy of the add record and the - (remove button) was hidden, updated JS to not hide on edit page. <br> Due to the way the buttons were coded in the add record page, JS had to be updated to allow them function on edit page.|

**Add Car (addcar.html)**
| Test | Expected outcome | Results | Issues|
| --- | --- | --- | --- |
|Fields are accessible & function | All fields in the form are working | Pass||
|Drops downs are populated with correct data | User should see only cars register to their userid. <br>only garages marked as active should be available for selection | Pass|||
|+ / - Buttons | Buttons should add or remove lines from the Form. | Pass||
|Add record Button | Button should collect the data from the form and create a new record in the DB and take the user to the maintenance record page | Pass||

**Manage Garages Record (add_garage.html)**
Manage Garage pages has two functions, 
1. Add a new garage to the DB
2. Update existing garages to activate or deactivate them.
    (With only active garages being available for selection by users. )

| Test | Expected outcome | Results | Issues|
| --- | --- | --- | --- |
|Add garage form, fields are accessible | Fields are accessible and can be filled out | Pass||
|Button | Button collects data from Form and creates a record in the DB.| Pass ||
|List of Garages is displayed and accessible | List can be read and button shows | Pass| Initially, the list was not working on mobile and table, it was not responsive and the button was off the phone screen<br> updated the table to a responsive class table from Materlize.|
|Activate / Deactivate Button | The button should toggle the status of the garage and reload the page | Pass||

[Index](#Index)

## **<ins>User_Testing</ins>**
User testing was completed on the site, having a user complete the following steps to ensure there were no issues;

| Test | Expected outcome | Results | Issues|
| --- | --- | --- | --- |
| Create an ID| New ID on the database | Pass||
| Login | successful login | Pass||
| Register a car | add a new car to the DB | Pass | |
| Create a record | add new maintenance record to the DB | Pass | On the add record page user testing raised two issues <br> 1. If user forgets to select the car or garage from the drop down, <br> the submit button did not work but there was no obvious indication what the issue was. <br> 2. Some fields that should be required were not set as such. <br> **Fix.** <br> Added error message for car & garage fields. <br> Added required class to the fields that must b e filled.  |
| View records | View list of records & detailed view of individual record  | Pass | |
| Edit a record | edit an existing record | Pass | |
| Delete a record | remove a record from the DB | Pass | |

In addition, the admin has additional functionality.

| Test | Expected outcome | Results | Issues|
| --- | --- | --- | --- |
| Register a garage| Add a new garage to the DB and ensure it shows up for users | Pass||
| Deactivate a garage | update the active flag on the garage in the DB and ensure its not shown for users to select | Pass||
| Reactivate a garage | update the active flag in the DB for a previously deactivated garage. Ensure garage shows up for user | Pass | |


### <ins>Code_Validation</ins>

|Code| Testing| Tool| Link|
| --- | --- | --- | --- |
|HTML| Validate HTML code|W3C - Markup Validation Service| https://validator.w3.org/|
|CSS| Validate CSS code|W3C - CSS Validation Service | https://jigsaw.w3.org/css-validator/|
|JS | Validate JS code | JSHint - Static Code Analysis Tool | https://jshint.com/|
|Python | Python PEP8 compliant|PEP8 online | http://pep8online.com/checkresult|

As part of the validation process, I generated a Lighthouse report for the site, to check for any serios issues.
Report summary below. 

<img src="/assets/readmeAssets/LH_Report_MS3.png">

[Index](#Index)
- - - -

## <ins>Deployment</ins>
The live version of the site is deployed on Heroku (free cloud account) or as an alternate you can create a copy and run the app locally.

### <ins>Live_Deployment</ins>
I choose Heroku as the cloud platform to deploy the project. 
- At www.heroku.com, you can create a free account. 
- Once you have your account set-up, create an app on Heroku (will require a unique name).
- Link the app, to you git repository for the project, you can connect to your git and search for the repository. 
- I chose to set my app to automatically deploy, meaning any update pushed to git auto deploys on Heroku. 
- In the settings tab, you need to add the config variables, (IP / DB / URI / Port  Secret_Key) mirroring what???s in the env.py file.

### <ins>Local_Deployment</ins>

To Clone the repository;
From the Github repository (@ https://github.com/meltaylor78/car_maintenance_tracker)
- click on the code button <img src="/assets/readmeAssets/Code_button.jpg"> and copy the link provided.
- In a Terminal or IDE
- Change the directory to the desired location on your drive
- Type git clone, followed by the url you copied above
Note: as an alternate, Git also allows the repository to be downloaded as a zip file. 


[Index](#Index)
- - - -
## **<ins>Database</ins>**
The application, would require a database backend, I chose mongoDB for the project. 
The database has four collections within it;

**Directory;**

The directory collection holds all the user data, records are created when a user registers on the site.
Data in the collection;
- Name
- e-mail address
- user Name
- password (stored in hashed format for security)

**Cars;**

The cars collections, holds data on cars registered on the site. Users can register their cars and only registered cars are available to create maintenance records for.
Data in the collection;
- Car Registration
- make
- model
- user
- e-mail
Note: user & e-mail are auto populated to the DB based on logon user at the time of registration.


**Garage;**

The garages collection has a list of garages that can be used when creating a record. Only the Admin can add or edit the list of garages. 
Data in the collection;
- Garage Name
- Garage Contact Name
- Garage Contact Phone No.
- Garage Status (active, when available for selection by user)


**Maintenance;**

The maintenance collection is populated with the records created by users. 
Data in the collection;
- Car Registration (user can only select pre-registered cars under their username)
- Car make - Populated from Car collection based on reg number selected
- Car Model - same as car make.
- username - based on the user logged when the record is created
- Service Date - user input as the time of record creation
- Service cost - user input as the time of record creation
- Service Paid - user input as the time of record creation, can be yes / no
- Service Description -  - user input at the time of record creation short description of service
- Odometer Reading  - user input as the time of record creation
- Garage Name - selected from list of active garages in garage collection
- Garage Contact - populated from Garage collection based on reg number selected
- Garage Phone No. - as garage name above
- Service Items - as garage name above

<img src="/assets/readmeAssets/collections_mongoDB.jpg">

[Index](#Index)
- - - -

### <ins>Acknowledgements</ins>
| Name | Area | Description |
| --- | --- | --- |
| Rahul Lakhanpal | Project Mentor | For all the guidance and input on UK and guiding me through the project with advise and direction. |
| Caroline Taylor | Testing | For help with User Testing and feedback |
|MongoDB | DB Hosting | For providing a free backend DB for the application|
|Heroku | Live Site Hosting |For providing a free cloud environment to host the application|

[Index](#Index)
- - - -
