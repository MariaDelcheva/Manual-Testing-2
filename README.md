# Manual-Testing-2

**Idea Center Web Application**

You are provided with a web application, the Idea Center, along with a specification of the requirements. The primary objective of the exam is to ensure the App functions as expected. This involves creating test cases for each use case provided. It also includes the detection and detailed documentation of any identified bugs. You have to document all your work in the provided Test Management and Bug Tracker Template. 

**Software Requirements**

**1. Introduction** 

**1.1. Purpose** 

The objective of this document is to provide a description of the Idea Center application (also referred to as Idea Center or The App). It will present an overview of the key functionalities. 
 
**1.2. Scope**

This document presents high-level descriptions of the basic functionalities of the Idea Center, such as user registration, login, profile editing, idea creation and management. It does not cover any special user (Administrator) functionalities. 
 
**2. Overall Description**

**2.1. System environment**

The Idea Center hosts two primary actors: unregistered/non-logged users and registered/logged users. Both can access their respective parts of the application via the internet on the following url: 
 
http://softuni-qa-loadbalancer-2137572849.eu-north-1.elb.amazonaws.com:83/   

**2.2. Key Features** 

Unregistered/non-logged users have access only to the Home page of The App, with the option to either SIGN UP FOR FREE or SIGN IN. On the other hand, registered/logged users have access to the main functionalities, including Profile editing, Idea creation, and Idea management functionalities. 
 
**2.2.1. Home Page for unregistered / non-logged users**

The Home page is the main gateway into the Idea Center. It contains a Navigation Menu on top (also referd to as Navbar) with "SIGN IN" and "SIGN UP FOR FREE" buttons on the left and back to Home page link on the right. 
The page also features a Carousel with three slides - "Be part of our community", "Already have an account?" and "Enjoy our site!". These slides change at random intervals, but users can also manually cycle through them. Two of the slides contain a call-to-action buttons prompting users to "SIGN UP FOR FREE" or "SIGN IN". 
 
**2.2.2. Sign Up Page**

The Sign Up page is accessed from the Home page. It contains form fields for entering a Username, Email, Password, and Repeat password. The form also includes a checkbox for agreeing to Terms of service,  a hyperlink to view the full Terms of service document and a Register button to submit the form. The acceptable requirements for each field are specified as follows: 
Username: A 2-30 character field, accepting all character types.  
Email: Requires a valid email, 6-254 characters long. 
Password: Any characters are acceptable, with a length of 6-30 characters 
Repeat Password: Must match password 
There is an alternative sign up options via Google or Facebook. 
 
 
**2.2.3. Sign In Page** 

The Sign In page can be reached from the Home page. The page provides fields for Email and Password, as well as a Remember password option, and a Sign In button.  
 
 
**2.2.4. Home Page for logged users**

Once a user is logged in, they are directed to a different version of the Home page. The page includes a Navbar with links to the Home page, My Profile, My Ideas, Create Idea, and a Logout button. The carousel here includes slides welcoming the user, and offering quick navigation to their profile (See your profile) or ideas (See your ideas). 

**2.2.5. My Profile Page** 

This page is accessible to logged users and includes a default empty profile picture, an Edit profile button, an empty About section by default, and a counter of the user's ideas, which is initially set to 0. If no ideas have been created yet, the Recent ideas section shows a No ideas message. There is also a Show all link which leads to My Ideas page. 

 
**2.2.6. Edit Profile Info Page** 

Accessible from the My Profile page, upon clicking on EDIT PROFILE button this page allows users to edit their profile information, including Profile picture (picture is not uploaded, but must be a valid URL of a picture), First name (max 60 characters length), Last name (max. 60 characters length), City (max. 120 characters length), and a Describe yourself section (max. 256 characters length). 

**2.2.7. My Ideas Page** 

This page is accessible from the Navbar and contains a Search ideas field and a Search button. If no ideas have been created yet, a No ideas yet! message is displayed. 
Users can enter keywords and click the Search button to initiate the search. The search functionality then filters the list of ideas based on the provided search terms. 

Upon Creating an idea, it appears on the My Ideas page where the user can VIEW, EDIT, or DELETE it. 

 
**2.2.8. Create Idea Page** 

This page can be accessed from the Navbar and contains fields for creating a new idea, including a Title (3-
70 characters length), Add picture field (picture is not uploaded, but must be a valid URL of a picture), and a Describe your idea field (3-400 characters length). Title and Description are mandatory. After entering these details, the user can click on the CREATE button to save the idea. 

**2.2.9. Idea Management** 

Managing Ideas is available for all created ideas from My Ideas Page. Each Idea has three options – VIEW, EDIT, and DELETE. 

**a.View**

Available after clicking on VIEW button.  

**b. Edit**

Available after clicking on EDIT button.  
 
**c. Delete** 

After clicking on DELETE button, the Idea is deleted and it disappers from My Ideas Page. 
 
****Functional Requirements****

**1. Use Case 1 (Home Page)**

Users can access The Idea Center from its designated URL via the internet, which will load the Home page, Carousel, and Navigation Pane, appropriate to the user's logged-in status (unregistered/non-logged or registered/logged). 
 
**2. Use Case 2 (User Registration)**

Unregistered users should be able to successfully go through the Sign Up process. This involves the utilization of fields such as Username, Email, and Password, all subject to their respective constraints and character type acceptance. User should have the option to Sign Up via Facebook or Google if he prefers. 
 
**3. Use Case 3 (User Sign In)**

Registered users should be able to successfully go through the Sign In process. They should be able to sign in using Email and Password. 
 
**4. Use Case 4 (Profile Management)**

Upon successful Sign In, logged users should be able to navigate to My Profile page, edit their Profile details, and view their Ideas count. This involves the changing of profile picture inserted via URL, and editing of user data fields including First Name, Last Name, City, and Describe Yourself. 

**5. Use Case 5 (Idea Creation)** 

Logged users should be able to navigate to the Create Idea page, where they can create a New idea with a Title, Picture (URL), and Description. After the idea creation process, users should be redirected to the My Ideas page, where the newly created idea should be present. 
 
**6. Use Case 6 (Idea Management)**

On the My Ideas page, logged users should see all their ideas listed. Each idea should have options for VIEW, EDIT, and DELETE. If no ideas have been created yet, a No ideas yet! message should be displayed. Users also should have the option to search for ideas, based on keywords. 

**Idea Center Web App Tasks**

**1. Test Cases**

You need to write test cases for each of the 6 Use cases. 
Each Use case should have at least 2 Test Cases. You should write at least 15 test cases.  

**2.	Bug Reports**  

You should find and describe at least 5 bugs. 

**3.	Template** 
Use the provided Test-Management-and-Bug-Tracking-Template.xlsx to document your work. 

