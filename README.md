# Test_cases for booking application
Below there are some Test Case samples that I wrote while working on my graduation project at Wantsome applying the techniques and testing types learned, on booking application for the register page.

TC01 
Description: Landing Page - Register button
Precondition: For unregistered users 

Steps to reproduce:
1. Open the site : http://138.68.69.185
2. Find the "Register" button on the top of the right side of the page.
3. Click on "Register" button.

Expected results: Being redirected on the register page.

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

TC02
Description: Register Page -Verify elements
Precondition: For unregistered users 

Steps to reproduce:
1. Open the site : http://138.68.69.185/register
2. Check the elements of the page: There are two sections : ''Login information'' (Top of the page) & '' Personal information'' (Bottom of the page) and there are two buttons ''Register'' & ''Cancel''.
3. [Login information] Check if every field is mandatory or optional
4. [Login information] Check if the following field is displayed : First Name.
5. [Login information] Check if the following field is displayed under the First Name : Last Name.
6. [Login information] Check if the following field is displayed under the Last Name : Email.
7. [Login information] Check if the following field is displayed under the Email : Password.
8. [Login information] Check if the following field is displayed under the Password : Confirm Password.
9. [Personal information] Check if every field is mandatory or optional.
10. [Personal information] Check if the following field is a dropdown : Country.
11. [Personal information] Check if the following field is a text field : City.
12. [Personal information] Check if the following field is a text field : Address 1.
13. [Personal information] Check if the following field is a text field : Address 2.
14. [Personal information] Check if the following field is a date picker field : Date of Birth.
15. [Personal information] Check if the following field is a dropdown : Gender.
16. [Personal information] Check if the following is a text field: Nationality.
17. Check if under the register form, two buttons appear: "Register" above and "Cancel" under.

Expected results: All the fields are displayed.

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

TC03
Description: Check if the account is not created if at least one mandatory field from Login information is not completed.
Precondition: The Register page is open.

Steps to reproduce:
1. Leave empty one of the mandatory fields.
2. Complete the rest of the mandatory fields.
3. Click on the Register button.

Expected results: An error message is displayed. 
The error message is: “[Name of the field] should not be empty”. Where [Name of the field] is related to each empty mandatory field.

Test Data:
First name : Test
Last name: Name
Email: TestEmail@test.com
Password: TestPassword123!
Confirm Password: TestPassword123!

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

TC04
Description: Check if the account is created if the field 'Date of birth' in Personal information section is not completed.
Precondition: The Register page is open. All the mandatory fields in the Login information section are completed.

Steps to reproduce:
1. Leave empty 'Date of birth' field.
2. Click on Register button.

Expected results: An error message is displayed. 
The error message is: "You must complete this mandatory field."

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

TC05
Description: Check if the account is created if the email doesn't have a validation of type {text}@{text}.{text}
Precondition: The Register page is open. All the mandatory fields are completed except the email field.

Steps to reproduce:
1. Enter an invalid email address in the email field.
2. Click on Register button.

Expected results: An error message is displayed. 
The error message is: "You must provide a valid email address."

Test Data: TestNametest.com

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

TC06
Description: Check if the account is created when the password doesn't meet one of the validations required.
Precondition: The Register page is open. All the mandatory fields are completed except the password field.

Steps to reproduce:
1. Complete the password field with the following test data.
2. Click on Register button

Expected results: An error message is displayed.
The error message is: "Your password must contain at least 8 characters, one 
uppercase letter, one lowercase letter, one number and one special character."

Test Data:
at least 7 characters;
no uppercase letter;
no one lowercase letter; 
no number;
no special character.

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

TC07
Description: Check if the user can create the account if is under 18 years old.
Precondition: The Register page is open. All the mandatory fields are correctly completed ( First Name, Last Name, Email, Password and Confirm Password) except 'Date of birth' field.

Steps to reproduce:
1. Pick a date of birth under 18 years old.
2. Click on Register button.

Expected results: A message will appear.
The message is: “You have to be over 18 
years in order to create an account”.

Test Data:
12.05.2007
10.01.2002

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

TC08
Description: Check if the account is created when the confirm password doesn't match with the password
Precondition: The Register page is open. All the mandatory fields are completed except the password and re-type password field.

Steps to reproduce:
1. Complete the password field with test data.
2. Complete the re-type password field with test data
3. Click on Register button

Expected results: An error message is displayed.
The error message is: "Your passwords must match"

Test Data:
TestPassword123!
TestPassword123

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

TC09
Description: Check if the account is created when all mandatory fields are completed
Precondition: The Register page is open. 

Steps to reproduce:
1. Complete "First name" field with test data.
2. Complete "Last name" field with test data.
3. Complete "E-mail" field with test data.
4. Complete "Password" field with test data.
5. Complete "Confirm password" field with test data.
6. Pick a date from the "Date of birth" picker using test data.
7. Click on "Register" button form the bottom of the page.
8. The user is redirected to the ‘Login’ page.

Expected results: The account is created. The "Login" page is open.

Test Data:
First name : Test
Last name: Name
Email: TestEmail@test.com
Password: TestPassword123!
Confirm Password: TestPassword123!
Date of birth: 12.01.2000

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

TC10
Description: Check if 'Cancel' button works by redirecting the user to the page they navigated from
Precondition: The Register page is open. 

Steps to reproduce:
1. Complete all the mandatory fields with valid data.
2. Complete some of the optional fields.
3. Click on 'Cancel' button under the Register form.

Expected results: The user is redirected to the page they navigated from.

Test Data:
First Name: Test
Last Name: Name
Email: TestEmail@test.com
Password: TestPassword123!
Re-type password: TestPassword123!
Date of birth: 12.05.2000
Country: Romania
City: Bacau
Gender: I prefer not to tell


















