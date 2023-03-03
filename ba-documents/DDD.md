# Database Design Document: **ContactWave**

## **Table of Contents**
- Introduction
- Table Descriptions
    - Users Table
    - Contacts Table
    - Social Platforms Table
    - Social Profiles Table
    - Phone Numbers Table
    - NFC Cards Table
- Conclusion

## **1. Introduction**
This document describes the database schema and design for ContactWave. The app allows users to create accounts and share their contact information with others by tapping an NFC card. The database stores user account information, contact details, social profiles, and phone numbers associated with each contact.

## **2. Table Descriptions**
### **Users Table**
The users table stores information about registered users of the app.

|Column Name|Data Type|Description|
|---|---|---|
|user_id|integer|Primary key that uniquely identifies the user|
|username|varchar(255)|The user's username|
|password|varchar(255)|The user's password|
|created_at|datetime|Timestamp of when the user was created|
|updated_at|datetime|Timestamp of when the user was last updated|

### **Contacts Table**
The contacts table stores information about contacts shared by the user.

|Column Name|Data Type|Description|
|---|---|---|
|contact_id|integer|Primary key that uniquely identifies the contact
|user_id|integer|Foreign key that associates the contact with the user who owns it
|first_name|varchar(255)|The contact's first name|
|last_name|varchar(255)|The contact's last name|
|email|varchar(255)|The contact's email address|
|avatar|varchar(255)|The relative path of the contact's avatar|
|address|varchar(255)|The contact's address|
|website|varchar(255)|The contact's website|
|created_at|datetime|Timestamp of when the contact was created|
|updated_at|datetime|Timestamp of when the contact was last updated|

### **Social Platforms Table**
The social_platforms table stores information about the type of social platforms.

|Column Name|Data Type|Description|
|---|---|---|
|platform_id|integer|Primary key that uniquely identifies the platform|
|name|varchar(255)|The name for the platform (e.g. Facebook, Twitter)|
|icon_path|varchar(255)|The path of the image file that store in the server associates with the platform|
|created_at|datetime|Timestamp of when the platform was created|
|updated_at|datetime|Timestamp of when the platform was last updated|

### **Social Profiles Table**
The social_profiles table stores information about social profiles associated with each contact.

|Column Name|Data Type|Description|
|---|---|---|
|social_profile_id|integer|Primary key that uniquely identifies the social profile
|contact_id|integer|Foreign key that associates the social profile with the contact it belongs to
|platform_id|integer|Primary key that uniquely identifies the social platform|
|profile_url|varchar(255)|The URL of the contact's profile on the platform|
|created_at|datetime|Timestamp of when the social profile was created|
|updated_at|datetime|Timestamp of when the social profile was last updated|

### **Phone Numbers Table**
The phone_numbers table stores information about phone numbers associated with each contact.

|Column Name|Data Type|Description|
|---|---|---|
|phone_number_id|integer|Primary key that uniquely identifies the phone number|
|contact_id|integer|Foreign key that associates the phone number with the contact it belongs to|
|name|varchar(255)|The custom name for the phone number|
|number|varchar(20)|The phone number itself|
|created_at|datetime|Timestamp of when the phone number was created|
|updated_at|datetime|Timestamp of when the phone number was last updated|

### **NFC Cards Table**
The nfc_cards table stores information about NFC card associated with each contact.

|Column Name|Data Type|Description|
|---|---|---|
|nfc_card_id|integer|Primary key that uniquely identifies the NFC card|
|user_id|integer|Foreign key that associates the NFC card with the user who owns it|
|contact_id|integer|Foreign key that associates the NFC card with the contact it represents|
|nfc_tag_id|varchar(255)|The unique ID of the NFC tag|
|created_at|datetime|Timestamp of when the NFC card was created|
|updated_at|datetime|Timestamp of when the NFC card was last updated|

## **3. Conclusion**
ContactWave is a useful tool for individuals and businesses who want to easily share their contact information. By implementing the proposed design, the app will be able to securely store user data and efficiently retrieve it when needed. The app will also be flexible enough to accommodate future changes and enhancements.