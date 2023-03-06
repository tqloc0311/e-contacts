# **Use Case Document: ContactWave**

## **Actors**
- User: A person who creates an account, inputs their contact information.
- Recipient: A person who taps the NFC card with their smartphone to display the user's contact information on a website.
- Admin: A person who manages ContactWave system.
  
## **Use Cases**

### **Create Account**

#### **Description**
The admin creates an account on the ContactWave platform, then send it to the user manually.

#### **Actors**
- Admin
- User

#### **Preconditions**
- The admin has access to a smartphone or computer with internet connectivity.

#### **Flow of Event**
1. The admin navigates to the ContactWave control panel.
2. The admin login with the admin account.
3. The admin clicks the "New user" button.
4. The admin enters an unique username and password.
5. The admin clicks the "Create" button.
6. The platform creates a new user account with a unique ID.
7. The admin send username and password to the user via email manually.
   
#### **Postconditions**
- The user can now log in to their account and input their contact information.

### **Input Contact Information**

#### **Description**
The user inputs their contact information into their account on the ContactWave platform.

#### **Actors**
- User
#### **Preconditions**
- The user has created an account on the ContactWave platform.
  
#### **Flow of Events**
- The user logs in to their account on the ContactWave website.
- The user clicks the "Edit Contact Info" button.
- The user inputs their contact information, including their name, phone number, email address, and social profiles.
- The user selects which contact information fields they want to display on their NFC card and website.
- The user uploads an avatar image to be displayed on their NFC card and website.
- The user clicks the "Save" button to save their changes.

#### **Postconditions**
The user's contact information is now saved in their account and can be displayed on their page.

### **Read NFC Card**

#### **Description**
The recipient taps the user's NFC card with their smartphone to display the user's contact information on a website.

#### **Actors**
- Recipient

#### **Preconditions**
- The recipient has an NFC-enabled smartphone.
- The user has written their unique ID to an NFC card using the ContactWave platform.

#### **Flow of Event**
1. The recipient holds their smartphone near the user's NFC card.
2. The smartphone automatically opens the ContactWave website and displays the user's contact information.
3. The website displays the user's name, avatar image, and all contact information fields that the user has enabled.

#### **Postconditions**
- The recipient can view the user's contact information on their smartphone and can choose to save the information to their contacts.

### **Update Contact Information**

#### **Description**
The user can update their contact information that is displayed on the ContactWave website.

#### **Actors**
- User

#### **Preconditions**
- The user has created an account on the ContactWave platform.
- The user has previously added contact information to their account.

#### **Flow of Event**
1. The user logs in to their account on the ContactWave website.
2. The user navigates to the "Profile" section of the website.
3. The user can update their contact information, including name, avatar, phone number, email, social profiles, etc.
4. The user taps the "Save" button to update their contact information.

#### **Postconditions**
- The user's updated contact information is displayed on the ContactWave website and is available to recipients who tap their NFC card.

### **Security and Privacy**

#### **Description**
The ContactWave platform takes security and privacy seriously to protect the user's personal information.

#### **Actors**
- User
- Platform

#### **Preconditions**
- The user has created an account on the ContactWave platform.

#### **Flow of Event**
1. The platform uses industry-standard encryption to protect user data, both during transmission and storage.
2. The platform implements authentication and access control measures to ensure that only authorized users can access user data.
3. The platform uses best practices to prevent and detect unauthorized access, such as firewalls, intrusion detection systems, and regular security audits.
4. The platform provides the user with options to control their privacy, such as the ability to choose which contact information fields are displayed on their NFC card and website.

#### **Postconditions**
- The user's personal information is securely stored and protected on the ContactWave platform.

### **Error Handling**

#### **Description**
The ContactWave platform provides error handling and feedback to the user in case of any errors or issues.

#### **Actors**
- User
- Platform

#### **Preconditions**
- The user has created an account on the ContactWave platform.

#### **Flow of Event**
1. The platform provides clear and descriptive error messages to the user in case of any errors or issues, such as invalid login credentials, missing or incorrect information, or system errors.
2. The platform uses logging and monitoring tools to track and diagnose any system errors or issues, to ensure quick resolution and minimal impact on the user experience.
3. The platform provides feedback to the user during the NFC card writing process, such as indicating when the card has been successfully written or if there were any issues during the process.

#### **Postconditions**
- The user can receive clear and descriptive error messages and feedback during the ContactWave process, ensuring a smooth and error-free experience. Any system errors or issues are quickly diagnosed and resolved, minimizing impact on the user.