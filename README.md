## User Classes and Characteristics

- **Patient -**
    
    This user is the one who registers as a patient in the application. 
    
- **Doctor -**
    
    This user is the one who registers as a doctor in the application. 
    
- **Admin -**
    
    Admin is a user which will have specific controls to the application which will allow them to control certain modules in the application. The admin can change the forum settings to make the users happy. Admin will administer the overall control of the website and can override any setting, or constraints in any module as he/she wants but he is not able to change the transaction details which are stored in the blockchain. In our case we can consider this as a person who can validate blockchain requests on the backend.

  ## Operating Environment

This web application can be deployed on Linux or Window machine with Apache Server and MySQL server

- Minimum RAM 4 GB
- 320 GB Storage Space.
- Intel i3 Processor.

## Assumptions and Dependencies

**Assumptions**

1. Every user has a metamask account with which they can register on our platform
2. The EHR record database is a singular entity that we have spanning across all hospitals and all doctors.

**Dependencies**

Backend - 

`web3j-spring-boot-starter`,`org.web3j.core`,`io.reactivex`,`org.springframework.boot`,`io.jsonwebtoken`,`mysql-connector-java`,`springfox-swagger-ui`,`spring-boot-maven-plugin`

Frontend -
![Untitled](https://github.com/nkhatri558/e-consent/assets/43436155/7b3a3f32-1487-4c68-9c55-f66da1bf5065)

# External Interface

## User Interfaces

1. Login/Signup Page: This is the first page any user of the Consent Management System has to go through. There are two options, one lets you login as a patient and the other as a doctor.
2. Navigation Bar: All the pages contains a Navigation Bar which allows the user(Patient/Doctor) to move between the different pages in the web application.
3. E-health Records Page: This page is common to the patients and the doctor. In the Patient’s page, it displays all the records of the patient, whereas in the doctor’s page it shows all the E-health records to which the doctor has consent
4. My Account Page: This is also a common page for both the doctor and the patient which shows the personal information of the user like Name, Phone number, Email etc.
5. Notifications Page: Again this page is common for both the patient and the doctor but with different functionality. In the doctor’s notification page he gets the notification of a patient accepting his consent request. The patient’s notification page receives notification about doctor asking for consent as well as confirmation notification when a doctor connects with the patient.
6. Connected Doctors Page: This is a Patient exclusive page, this page contains the list of all the doctors to which the patient is connected.
7. Consent Page: This is also a Patient page, it shows the list of records for which consent has been given to some doctor, with the details of the consent in a tabular form.
8. Request Consent Page: This is a Doctor exclusive page, where the doctor can see all the consents he has, along with which he can request consent for selected records from a patient.
9. Logout: This is a button which lets the user logout of the application.

## Hardware Interfaces

**Screen resolution of at least 800X600 is required for proper and complete viewing of screens. Higher resolution will be accepted. The user will need pointing and a typing interface for the proper functioning of the application.**

## Software Interfaces

The below Software interface is still in consideration:

- **Client: `Web Browser**, **React**`
- **Backend: `Springboot`**
- **Database Server: `MYSQL, Ethereum Based Blockchain`**
- **Development Tools: `Postman`, `Swagger-UI`, `Chrome Dev tools`**

## Communications Interfaces

- Client on Internet will be using HTTP/HTTPS protocol.
- Firewall security is required for securing the server.
- TCP/IP protocol is a basic need for the client-side.
- JWT Token for protecting the API calls
- Security Modifiers are set up in our smart contract for permission access over public TCP calls.


# Key Challenges

- **Usability**:
    
    Now, this is another main issue that we are looking at and is called usability. Since we are working with a Decentralized application (*Dapp),* the way that it works is a bit different from a normal app. So should we make it more like the present system or should we take a more standardized approach. The Standardized approach seems to be the correct option but it comes with some costs to the developer.
    
- **Efficiency**:
    
    The system must provide easy and fast access without consuming more cost. This is one of the main issues that we have right now since each transaction that we send to a blockchain requires some gas(i.e. money) and this money is comparative to how you make a monthly payment for a centralized server. 
    
- **Reliability**:
    
    The software should be as failure-free as possible, i.e. most of the error cases should be handled so as to not affect the user experience and thus the usability of the application.

  

# e_consent_framework
CIDRI Africa REDCap template for e-consent framework in genomics research 

## General project settings

- Use surveys ENABLED
    - This activates the e-consent framework 
- Longitudinal data collection ENABLED
    - Only enabled to showcase examples of an fully executed framework
- Enable optional modules and customizations
    - Auto-numbering for records

### Additional customizations
-  PDF Customizations
    - Downloadable PDFs of data entry forms and surveys can be customized using the options below.
-  Enable the Data History 
    - History of all data entered into that field for that record will be listed chronologically and will display all previous values
-  Enable the File Version History
    - Allows you to maintain previous versions of a file for a File Upload field
-  Require a 'reason' when making changes to existing records
    - Require users to enter a reason for changes made to an already captured field




