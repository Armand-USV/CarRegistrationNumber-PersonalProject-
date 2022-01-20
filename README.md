# CarRegistrationNumber -PersonalProject- -DEMOVERSION-

Application made on Android Oreo 8.1 version (API 27).

This application takes a registration number entered in a PlainText and checks if it is in the database (Obs: Currently "Database" is a list of objects of the type "CarRegistrationNumber"). The "CarRegistrationNumber" class contains two string variables (registration number and expiration date) and one boolean (insurance) variable.
The verification is done by pressing a button, and the results (indicated by an AlertDialog message) can be the following:
- "Registration number is wrong". The registration number of a car, from Romania, consists of 7 characters (5 letters and 2 numbers). Therefore, if that number of characters is exceeded, we will receive that error message.
- "Please enter the registration number". This message will appear when we do not enter anything in PlainText.
- "The car with registration number XX00XXX does not exist in the database! Do you want to enter it in the database?" . As I said above, the database is a list of "CarRegistrationNumber" objects, the list being populated with several registration numbers. This message will appear when the registration number entered does not exist in that list. If it does not exist, we can add that registration number.
- "The car with registration number XX00XXX does not have insurance! Do you want to create an insurance?" . This message will appear when the value assigned to the registration number is "false". In this case we can enter the expiration date.
- "The car with registration number XX00XXX has insurance". This message will appear when the registration number is in the "database" and its value is "true". For cars with insurance, the expiration date can be viewed.

The project is just beginning, with some issues, such as when the expiration date is entered. We did not specify a specific format or the ability to retrieve the entered value as a calendar date.

The future development of the project represents:
- Use of databases
- The possibility to create an insurance, much more detailed.
