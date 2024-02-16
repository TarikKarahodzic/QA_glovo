# Quality Assurance of Glovo website

## 1. Introduction
<b>1.1 About the project</b><br>
<b>Glovo</b> is an on-demand delivery service platform that connects users with local couriers to deliver a wide range of items, including food and groceries, to their doorsteps quickly and conveniently. It's known for its user-friendly app and website, making everyday deliveries easy and efficient. Glovo operates in multiple countries and urban areas worldwide. <br>
[Link to Glovo app](glovoapp.com)

## 2. Test Plan
<b>2.1 Scope</b><br>
Firstly, we're going to look into how you log in or sign up on the website. Then, we'll test if the address input works well and finds the right address. It's also important to check that you can edit your profile info. Another big thing we'll check is how payments work and if you can order stuff smoothly. Plus, we'll explore features for people who want to become Glovo couriers or partners.

<br><b>2.2 Testing Environment and Tools<br>
Tools that have been used in this project are mostly TypeScript and JavaScript. Also, Chrome Driver enabled automated testing in Chrome browser.

## 3. Test Execution
In this section there are test scenarios and test cases. Section has ten test cases for regression tests and one for smoke test.

<b>Regression tests</b>

<b>3.1 User Authentication<br>

| Test Steps: | Test Data: | Expected Results: | Actual Results: | Status: |
| --- | --- | --- | --- | --- |
| 1. Go to the website glovoapp.com <br> 2. Close cookies popup <br> 3. Navigate to 'Get Started' button <br> 4. Choose 'Email' login option <br> 5. Enter email <br> 6. Enter password <br> 7. Enter address <br> 8. Enter your location/address | - svvttest360@outlook.com <br> -svvttest123 <br> -Tester <br> -Aleja Lipa 66, 71000 Sarajevo | Load website without any issues. Open a signup/login window. Email and password work successfully. Input location is successful. User is signed up. | Website is loaded without any issues. Email and password fields are correct. Input of location is successful, and the user is signed up. | PASS |

<b>3.2 Edit profile<br>

| Test Steps: | Test Data: | Expected Results: | Actual Results: | Status: |
| --- | --- | --- | --- | --- |
| 1. Go to the website glovoapp.com <br> 2. Close cookies popup <br> 3. Navigate to 'Get Started' button <br> 4. Choose 'Email' login option <br> 5. Enter email <br> 6. Enter password <br> 7. Enter your location/address <br> 8. Navigate to and press on a profile drop down menu button <br> 9. Press on 'Edit profile name' <br> 10. Clear old name <br> 11. Enter new name and press 'Save' | - svvttest360@outlook.com <br> -svvttest123 <br> -Aleja Lipa 66, 71000 Sarajevo <br> -'Testing' | Load website without any issues. Open a signup/login window. Email and password work successfully. Input location is successful. User is logged in. Profile and edit profile name buttons are clickable. Save a new name. | Website is loaded without any issues. Email and password fields are correct. Input of location is successful, and the user is logged in. Both buttons are clickable and it saves a new name. | PASS | 

<b>3.3 Search Engine<br>

| Test Steps: | Test Data: | Expected Results: | Actual Results: | Status: |
| --- | --- | --- | --- | --- |
| 1. Go to the website glovoapp.com <br> 2. Navigate to 'Get Started' button <br> 3. Choose 'Email' login option <br> 4. Enter email <br> 5. Enter password <br> 6. Enter address <br> 7. Press on the search bar and type what you want to search <br> 8. Press on 'Show more' | - svvttest360@outlook.com <br> -svvttest123 <br> -Aleja Lipa 66, 71000 Sarajevo <br> -'pizza' | Load the website without any issues. Login to your account. Search opens a new page where it shows all the stores and products that have ‘pizza’ in their name or in their menu. Shows all of the options for specific search | Website is loaded without any issues. Search engine does actions correctly, it opened new window with pizzas. | PASS |

<b>3.4 Payment methods<br>

| Test Steps: | Test Data: | Expected Results: | Actual Results: | Status: |
| --- | --- | --- | --- | --- |
| 1. Go to the website glovoapp.com <br> 2. Close cookies popup <br> 3. Navigate to 'Get Started' button <br> 4. Choose 'Email' login option <br> 5. Enter email <br> 6. Enter password <br> 7. Enter your location/address <br> 8. Navigate to and press on a profile drop down menu button <br> 9. Choose 'Add a new card' under Payment methods <br> 10. Enter Credit card details and press 'Save' | - svvttest360@outlook.com <br> -svvttest123 <br> -Aleja Lipa 66, 71000 Sarajevo <br> -'Tester Testing' <br> 1234567812345678 <br> 12/28 <br> 234 | Load website without any issues. Open a signup/login window. Email and password work successfully. Input location is successful. User is logged in. Profile drop down button works. New tab is opened with payment settings. Credit card successfully added. | Website is loaded without any issues. Email and password fields are correct. Input of location is successful, and the user is logged in. Drop down button works, and it opens a new website. No fields are accessed and no data is inserted. The card was not successfully. | FAIL |

<b>Notes: </b><i>None of the paths work, the program cannot find the path to insert the data. Tried with custom and full xpaths.</i>

<b>3.5 Sorting test<br>

| Test Steps: | Test Data: | Expected Results: | Actual Results: | Status: |
| --- | --- | --- | --- | --- |
|  1. Go to the website glovoapp.com <br> 2. Close cookies popup <br> 3. Navigate to 'Get Started' button <br> 4. Choose 'Email' login option <br> 5. Enter email <br> 6. Enter password <br> 7. Enter your location/address <br> 8. Navigate to a Food menu <br> 9. Choose 'Restaurants' <br> 10. Sort restaurants as 'Best Rated' | - svvttest360@outlook.com <br> -svvttest123 <br> -Aleja Lipa 66, 71000 Sarajevo | Load website without any issues. Open asignup/login window. Email and password work successfully. Input location is successful. User is logged in. Circular menu opens with options, and opens a new page with restaurants. Restaurants successfully sorted. | Website is loaded without any issues. Email and password fields are correct. Input of location is successful, and the user is logged in. Food menu opens, and it selects Restaurants. Opens a new window and successfully sorts the restaurants as Best rated. | PASS |

<b>3.6 Special deals and promotions<br>

| Test Steps: | Test Data: | Expected Results: | Actual Results: | Status: |
| --- | --- | --- | --- | --- |
| 1. Go to the website glovoapp.com <br> 2. Close cookies popup <br> 3. Navigate to 'Get Started' button <br> 4. Choose 'Email' login option <br> 5. Enter email <br> 6. Enter password <br> 7. Enter your location/address <br> 8. Navigate to and press a profile drop down menu button <br> 9. Toggle off 'Recieve special deals and promotions' option | - svvttest360@outlook.com <br> -svvttest123 <br> -Aleja Lipa 66, 71000 Sarajevo | Website is loaded without any issues. Email and password fields are correct. Input of location is successful, and the user is logged in. Open the profile section, toggle off the promotions option. | Website is loaded without any issues. Email and password fields are correct. Input of location is successful, and the user is logged in. Profile opens up and it successfully toggles off the promotions option | PASS |

<b>3.7 Search Engine<br>

| Test Steps: | Test Data: | Expected Results: | Actual Results: | Status: |
| --- | --- | --- | --- | --- |
| 1. Go to the website glovoapp.com <br> 2. Close cookies popup <br> 3. Navigate to 'Get Started' button <br> 4. Choose 'Email' login option <br> 5. Enter email <br> 6. Enter password <br> 7. Enter your location/address <br> 8. Navigate Food menu <br> 9. Choose 'Restaurants' <br> 10. Choose Taj Mahal restaurant <br> 11. Select the desirable food for order <br> 12. After finishing with the meals, press 'Add to Cart' | - svvttest360@outlook.com <br> -svvttest123 <br> -Aleja Lipa 66, 71000 Sarajevo | Load website without any issues. Open a signup/login window. Email and password work successfully. Input location is successful. User is logged in. Circular menu opens with options, and opens a new page with restaurants. Find a desirable restaurant. Select desirable food, add to cart. Order. | Website is loaded without any issues. Email and password fields are correct. Input of location is successful, and the user is logged in. Food menu opens, and it selects Restaurants. Opens a new window, opens desirable restaurant, in this case ‘Taj Mahal’ and orders desirable food. | PASS |

<b>3.8 Become a partner<br>

| Test Steps: | Test Data: | Expected Results: | Actual Results: | Status: |
| --- | --- | --- | --- | --- |
| 1. Go to the website glovoapp.com <br> 2. Close cookies popup 3. Navigate to 'Get Started' button <br> 4. Choose 'Email' login option <br> 5. Enter email <br> 6. Enter password <br> 7. Enter address/location <br> 8. Find 'Become a partner' section and press 'Register here' button <br> 9. Choose which country your business is from <br> 10. Click on 'Postani partner' (Become a partner) | - svvttest360@outlook.com <br> -svvttest123 <br> -Aleja Lipa 66, 71000 Sarajevo <br> -'Sarajevo' <br> -'Test Company' <br> -'Test <br> -'Testing' <br> -'testtest111@outlook.com <br> -0610001111 | Load website without any issues. Open a signup/loginwindow. Email and password work successfully. Input location is successful. User is logged in. Open Become a partner, select Bosnia and Herzegovina. Click ‘Postani partner’, fill out information about your business. | Website is loaded without any issues. Email and password fields are correct. Input of location is successful, and the user is logged in. Opens the become a partner, selects country, fills out information successfully. | PASS |

<b>3.9 Become a rider<br>

| Test Steps: | Test Data: | Expected Results: | Actual Results: | Status: |
| --- | --- | --- | --- | --- |
| 1. Go to the website glovoapp.com <br> 2. Close cookies popup <br> 3. Navigate to 'Get Started' button <br> 4. Choose 'Email' login option <br> 5. Enter email <br> 6. Enter password <br> 7. Enter your location/address <br> 8. Find 'Become a partner' section and press 'Register here' button <br> 8. Find 'Become a rider' section and press 'Register here' | - svvttest360@outlook.com <br> -svvttest123 <br> -Aleja Lipa 66, 71000 Sarajevo | Load website without any issues. Open a signup/login window. Email and password work successfully. Input location is successful. User is logged in. Open Become a rider, and load the new website. | Website is loaded without any issues. Email and password fields are correct. Input of location is successful, and the user is logged in. Opens become a rider website. | PASS |

<b>3.10 Contact us<br>

| Test Steps: | Test Data: | Expected Results: | Actual Results: | Status: |
| --- | --- | --- | --- | --- |
| 1. Go to the website glovoapp.com <br> 2. Close cookies popup <br> 3. Navigate to 'Get Started' button <br> 4. Choose 'Email' login option <br> 5. Enter email <br> 6. Enter password <br> 7. Enter your location/address <br> 8. Find 'Become a partner' section and press 'Register here' button <br> 8. Navigate to the bottom of the page and press 'Contact us' <br> 9. Choose 'Not related to an order' (Because we haven't had any orders) <br> 10. Click on 'Account details' <br> 11. Press on 'Change email address' | - svvttest360@outlook.com <br> -svvttest123 <br> -Aleja Lipa 66, 71000 Sarajevo | Load website without any issues. Open a signup/login window. Email and password work successfully. Input location is successful. User is logged in. Find the Contact us button, choose Not Related, click on account details and press on change email address. | Website is loaded without any issues. Email and password fields are correct. Input of location is successful, and the user is logged in. Successfully finds the button, new window pop up is shown, new options have been given, new drop down menu is shown, new tab is open with a detailed information about Glovo’s FAQ. | PASS |

<b> Smoke test </b>

<b>3.1 Search Engine<br>

| Test Steps: | Test Data: | Expected Results: | Actual Results: | Status: |
| --- | --- | --- | --- | --- |
| 1. Go to the website glovoapp.com <br> 2. Navigate to 'Get Started' button <br> 3. Choose 'Email' login option <br> 4. Enter email <br> 5. Enter password <br> 6. Enter address <br> 7. Press on the search bar and type what you want to search <br> 8. Press on 'Show more' | - svvttest360@outlook.com <br> -svvttest123 <br> -Aleja Lipa 66, 71000 Sarajevo <br> -'pizza' | Load the website without any issues. Login to your account. Search opens a new page where it shows all the stores and products that have ‘pizza’ in their name or in their menu. Shows all of the options for specific search | Website is loaded without any issues. Search engine does actions correctly, it opened new window with pizzas. | PASS |


 
