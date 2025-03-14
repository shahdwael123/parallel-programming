https://github.com/shahdwael123/parallel-programming/settings# parallel-programming
Idea : Sending Emails Through a Spring Boot Application
Email through spring boot app to send emails through the spring application we use JavaMailSender
Spring** **Boot provides the ability to send emails via SMTP using the [﻿JavaMail](https://docs.spring.io...) Library. You may send an email with Gmail transport layer security by utilizing the spring boot restful web API
Steps :- 
Step 1: Add Required Dependencies
To enable email functionality in your Spring Boot application, you first need to add the necessary dependencies.

Step 2: Add Required Configuration Properties
Next, configure the email properties. Open your application.properties or application.yml file and add the following settings for Gmail's SMTP server

Important: If you have two-factor authentication enabled, you will need to generate an App Password. Follow these steps to generate an App Password for your Gmail account:
Visit your Google Account settings.
Navigate to the "Security" section.
Under "Signing in to Google," select "App passwords."
Follow the prompts to generate a password tailored for your application.

Step 3: Generate the Email Service Layer
Create a service class to encapsulate the email-sending logic. This service will handle both simple emails and emails with attachments

Step 4: Generate the Controller Layer
Create a REST controller to provide endpoints for sending emails. This controller will expose two endpoints: one for sending simple emails and another for sending emails with attachments.

Step 5: Create Data Transfer Objects (DTOs)
Define data transfer object (DTO) classes for encapsulating email request data. One DTO will be used for simple emails, and another for emails with attachments.
