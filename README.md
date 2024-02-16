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
<br><b>Regression tests</b>

<b>3.1 Search Engine<br>

| Test Steps: | Test Data: | Expected Results: | Actual Results: | Status: |
| --- | --- | --- | --- | --- |
| 1. Go to the website glovoapp.com <br> 2. Navigate to 'Get Started' button <br> 3. Choose 'Email' login option <br> 4. Enter email <br> 5. Enter password <br> 6. Enter address <br> 7. Press on the search bar and type what you want to search <br> 8. Press on 'Show more' | - svvttest360@outlook.com <br> -svvttest123 <br> -Aleja Lipa 66, 71000 Sarajevo <br> -'pizza' | Load the website without any issues. Login to your account. Search opens a new page where it shows all the stores and products that have ‘pizza’ in their name or in their menu. Shows all of the options for specific search | Website is loaded without any issues. Search engine does actions correctly, it opened new window with pizzas. | PASS |


 
