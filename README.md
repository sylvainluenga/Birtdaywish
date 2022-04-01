# Birtdaywish using python script by Alex Sylvain Luenga
Realm Digital Simple Practical Assessment Intermediate Developer  
The first thing we do is import six libraries: 
1.pandas
2.datetime
3.smtplib
4.time
5.requests
6.win10toast

Also create an Excel sheet for containing records like this: Name, Email, Contact, Birthday, and Year.

# Approach:

For the sending email part, We define a sendEmail() function which will start a Gmail session, send the email, and quit the session.
For the SMS part, we must have an account on www.fast2sms.com 
from where we will get an API key. This API key is used to send SMS over mobile numbers using your account on fast2sms then We create a sendsms() function which will verify the API key and send SMS. (This was just one plus )

But here we have been given an API link: https://interview-assessment-1.realmdigital.co.za/employees  

In the driver code section, 
we read the data from Excel sheet and match today’s date with any of the birthdays. 
If there is a match, we call the sendEmail() and sendsms() functions and also we add the current year in the Excel sheet. Also, we have used ToastNotifier from win10toast library to show desktop notifications once the e-mail and SMS has been sent successfully.
