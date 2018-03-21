# Rails Developer Admission Test

The candidate should implement  and deploy the application as defined below

The code should be available on a github open repository

The application must be running on a free heroku&#39;s account

The candidate must provide the github&#39;s url and heroku&#39;s url for our evaluation

A Readme should be available in the source code with instructions for usage, deploy and development of the application

# App Definition

I want to manage my deals and estimate the probability to achieve my sales goals.

Functional Requirements:

- I want to be able to sign in/sign up by email/password;
- I want to be able to create/replace/update/delete deals;
- I want to be able to search deals by any information;
- I want to be able to order deals by any information;
- I want to be able to define a expected closing date for a deal;
- I want to be able to mark a deal as &#39;won&#39; or &#39;lost&#39;;
- I want to import deals from a Pipedrive Account

Create a free trial account for this test:

[https://www.pipedrive.com/](https://www.pipedrive.com/)

[https://developers.pipedrive.com/docs/api/v1/](https://developers.pipedrive.com/docs/api/v1/)

# Technical Requirements

- It should be a WEB application:
- For the client side, use HTML5, CSS3, Bootstrap, JavaScript, and jQuery;
- For the server side, use Ruby on Rails.
- It should have client side and server side validation;
- It should work like a single-page WEB application and should use AJAX technology (load and submit data without reloading a page);
- It should have a user authentication solution. The user should only have access to his/her own deals (Devise, Cancancan);
- It should have automated tests for all functionality (models - RSpec, controllers - RSpec, acceptance/functional tests - RSpec + Capybara);

# Use Cases and Suggested Screens

The result should be similar to the screens and use cases below

## Main Screen:

## Use Case:

- User login on App
- Go to Main Screen and list user deals
- On this screen user can CRUD Deals
- User can Import Deals from a Pipedrive Account

## Screen:

**+ Deals:**

   Customer: [\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_]

   Description: [\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_]

   Value: [\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_]

   [Add Deal]

   [Import Deals From Pipedrive]

**Current Deals: US$2,5B       **

[\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_] [Search]

| Customer | Description | Status | Closing Date/ Probability | Value | Actions |
| --- | --- | --- | --- | --- | --- |
| Acme | Multi Billion Dollars Sale | Won | 03/03/18 | US$ 2,5 B | Edit | Destroy | Won | Lost |
| W&amp;B | Multi Million Dollars Sale | Pending | In 25 days70% | US$ 2,5 M | Edit | Destroy | Won | Lost |
| Acme | Multi thousand Dollars Sale | Lost | 03/02/18 | US$ 2,5 K | Edit | Destroy | Won | Lost |

|&lt; &lt; Page: n of nn &gt; &gt;|

## Pipedrive Import Screen

## Use Case:

- From main screen select [Import Deals from Pipedrive]
- Open a Popup Window
- Inform Pipedrive token and connect (Save token on session for future imports)
- Select Pipeline and update Owner Combo with Ajax (Save selected queue on session for future imports)
- Select salesman and update Deals list with Ajax (Save Selected Salesman on session for future imports)
- Select Deals to Import, Import Deals and go back to main Screen.

## Screen:

**Import Deals from Pipedrive**

Pipedrive Token: [\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_]

[Connect]

Pipeline: [\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_-][&gt;]

Owner: [\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_-][&gt;]

Deals (For the Salesman Above):

[\_] Customer - Deal ….. - Value

[\_] Customer - Deal ….. - Value

[\_] Customer - Deal ….. - Value

[\_] Customer - Deal ….. - Value

[\_] Customer - Deal ….. - Value

[Import All Selected Deals]

<u>Cancel</u>

# Screen Legend:


[\_] : Check Box

[\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_-][&gt;]  : Combo Box

[\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_]  : Text Box

[Connect]  : Button

Cancel    : Link
