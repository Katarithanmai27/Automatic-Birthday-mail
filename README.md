Importing Necessary Libraries

Begin by importing the following libraries:

pandas for handling Excel data,
datetime for date manipulation,
smtplib for sending emails,
time for managing time-related tasks,
requests for sending HTTP requests,
win10toast for displaying desktop notifications.
Step 2: Creating an Excel File

Create an Excel file named birthdays.xlsx containing the following columns: Name, Email, Contact, Birthday, and Year. Populate this file with relevant data.

Step 3: Defining the Email Sending Function

Define a function named sendEmail that will:

Start an SMTP session with Gmail,
Send an email to the specified recipient with a subject and message,
Quit the SMTP session after sending the email.
Step 4: Defining the SMS Sending Function

Define a function named sendsms that will:

Use the Fast2SMS API to send SMS,
Accept the API key, message, and contact number as parameters,
Send the message using an HTTP POST request.
Step 5: Reading Data and Matching Birthdays

Read the data from the birthdays.xlsx file. For each record, compare today's date with the birthday listed in the file:

If a match is found, call the sendEmail function to send an email,
Call the sendsms function to send an SMS,
Update the Year column in the Excel file to the current year,
Use the ToastNotifier to display a desktop notification confirming that the email and SMS were sent.
Step 6: Saving the Updated Excel File

After processing all records, save the updated data back to the birthdays.xlsx file to ensure the Year column reflects the current year.# Automatic-Birthday-mail
