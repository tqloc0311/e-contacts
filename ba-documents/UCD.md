# **Use Case Document: ContactWave**

## **Actors**
- User: A person who creates an account, inputs their contact information, and writes their unique ID to an NFC card.
- Recipient: A person who taps the NFC card with their smartphone to display the user's contact information on a website.
  
## **Use Cases**

### **Create Account**

#### **Description**
The user creates an account on the ContactWave platform.

#### **Actors**
- User

#### **Preconditions**
- The user has access to a smartphone or computer with internet connectivity.

#### **Flow of Event**
1. The user navigates to the ContactWave website.
2. The user clicks the "Sign Up" button.
3. The user enters their name, email address, and password.
4. The user clicks the "Create Account" button.
5. The platform creates a new user account with a unique ID.
   
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
The user uploads an avatar image to be displayed on their NFC card and website.
The user clicks the "Save" button to save their changes.
#### **Postconditions**
The user's contact information is now saved in their account and can be displayed on their NFC card and website.

### **Write NFC Card**

#### **Description**
The user writes their unique ID to an NFC card using their smartphone.

#### **Actors**
- User
#### **Preconditions**
The user has created an account on the ContactWave platform.
The user has ordered an NFC card through the website or obtained an NFC card from another source.
#### **Flow of Event**
1. The user navigates to the "Write NFC Card" section of the ContactWave website on their smartphone.
2. The user taps the "Write to NFC Card" button.
3. The user holds their smartphone near the NFC card.
4. The user taps the "Write" button on their smartphone to write their unique ID to the NFC card.
5. The platform confirms that the ID has been successfully written to the NFC card.

#### **Postconditions**
- The user's unique ID is now stored on the NFC card and can be read by others using an NFC-enabled smartphone.

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

### **Generate QR Code**

#### **Description**
The user generates a QR code that contains their unique ID for sharing with others who do not have NFC-enabled smartphones.

#### **Actors**
- User

#### **Preconditions**
- The user has created an account on the ContactWave platform.
- The user wants to share their contact information with someone who does not have an NFC-enabled smartphone.

#### **Flow of Event**
1. The user navigates to the "Generate QR Code" section of the ContactWave website.
2. The user taps the "Generate QR Code" button.
3. The platform generates a QR code that contains the user's unique ID.
4. The user can download the QR code image to their smartphone or computer.
5. The user can share the QR code image with others via email, text message, or other means.

#### **Postconditions**
- The recipient can scan the QR code with their smartphone to view the user's contact information on the ContactWave website.

### **View Analytics**

#### **Description**
The user views analytics about their NFC card usage and website visits.

#### **Actors**
- User

#### **Preconditions**
- The user has created an account on the ContactWave platform.
- The user's NFC card has been used by recipients to view their contact information.

#### **Flow of Event**
1. The user logs in to their account on the ContactWave website.
2. The user navigates to the "Analytics" section of the website.
3. The platform displays analytics about the user's NFC card usage, including the number of taps and unique visitors.
4. The platform displays analytics about the user's website visits, including the number of visits and which contact information fields were viewed.

#### **Postconditions**
- The user can use the analytics to track the effectiveness of their NFC card and website in sharing their contact information.

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

### **Manage NFC Cards**

#### **Description**
The user can manage their NFC cards, including viewing, creating, and deleting them.

#### **Actors**
- User

#### **Preconditions**
- The user has created an account on the ContactWave platform.
- The user has previously created one or more NFC cards.

#### **Flow of Event**
1. The user logs in to their account on the ContactWave website.
2. The user navigates to the "Manage NFC Cards" section of the website.
3. The platform displays a list of the user's existing NFC cards.
4. The user can view details about an existing NFC card by clicking on it.
5. The user can create a new NFC card by tapping the "Create NFC Card" button.
6. The user can delete an existing NFC card by clicking the "Delete" button next to it.

#### **Postconditions**
- The user can manage their NFC cards on the ContactWave website, including creating new cards, deleting existing cards, and viewing details about existing cards.

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

### **Integration with CRM Systems**

#### **Description**
The ContactWave platform can integrate with CRM (customer relationship management) systems to provide the user with more advanced analytics and management tools.

#### **Actors**
- User
- CRM System

#### **Preconditions**
- The user has created an account on the ContactWave platform.
- The user uses a CRM system to manage their contacts and leads.

#### **Flow of Event**
- The platform can integrate with the user's CRM system to automatically sync contact information and activity data.
- The user can view more advanced analytics and management tools in their CRM system, such as lead scoring, automated workflows, and sales funnel tracking.
- The user can use their CRM system to manage their leads and contacts, including creating tasks, sending emails, and scheduling meetings.

#### **Postconditions**
- The user can use the ContactWave platform to seamlessly integrate with their CRM system, providing them with more advanced analytics and management tools for their contacts and leads.
  
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