# BBC Bitesize - Software Engineer Technical Test - Address Labels

## Introduction

This technical test is based around a simple JavaScript application that produces address labels. The application works and prints out address labels to the console.

The existing code is considered "legacy" as it has no tests. The technical test outlines two tasks which are focussed around 1) safely refactoring and testing critical parts of the codebase and 2) adding a new feature to support international address formats.

During the test we'll be looking for your approach to solving problems and working with a partner, rather than the solution itself.

> **Note:** _Please take some time before the interview to consider how you would approach the tasks below, but do not perform these tasks until the interview._

## Get set up

You'll be asked to use your machine during the interview. To help ensure you have the most time avilable for the test, please follow the instructions below to set up the application locally and make sure you can start the application and run the test suite. If you encounter any issues, please get in touch with your recruiter before the interview.

### Install the dependencies

`npm install`

### Run the application

`npm start`

### Run the tests

`npm test`

## Structure

- `/data` Contains json with raw address fields
- `/app` Contains the code that prints out the labels
- `/test` Contains an empty test file, pre-configured to run with Jest

# Task 1

The code currently has no tests associated with it, the project is pre-configured with a Jest configuration. Your task is to begin refactoring and testing the most critical part of the application.

- Do not change the data in the json file. Treat this as an external data system.
- Fix any bugs that you encounter.

# Task 2

Implement the ticket below on this project. The address data is already available in the json file.

## Ticket-130

- As an international user
- I want to recieve your product

### Background

Our business is growing and we now need to print off address information so that we can send our products around the world. It has come to the attention of the team that the UK format for address labels is not valid for all countries.

We want to start sending products to the US, Hong Kong, Italy, Switzerland, France, Germany and Japan.

We already have collected the address information but require a change to display the address in the correct format.

Update the application to provide support for printing address labels in the correct formats for all listed countries.

### Examples:

(taken from https://bitboost.com/ref/international-address-formats.html)

#### Italy:

CHRIS RUSSO  
VIA APPIA NUOVA 123/4  
00184 ROMA RM  
ITALY

#### US:

CHRIS NISWANDEE  
SMALLSYS INC  
795 E DRAGRAM  
TUCSON AZ 85705  
USA

#### Switzerland:

Frau  
Wilhemlina Waschbaer  
Hochbaumstrasse 123 A  
5678 Bern  
SWITZERLAND

#### Hong Kong:

Mr. CHAN Kwok-kwong  
Flat 25, 12/F, Acacia Building  
150 Kennedy Road  
WAN CHAI  
HONG KONG

#### France:

Madame Duval  
27 RUE PASTEUR  
14390 CABOURG  
FRANCE

#### Germany:

Herrn  
Eberhard Wellhausen  
Wittekindshof  
Schulstrasse 4  
32547 Bad Oyenhausen  
GERMANY

#### Japan:

see https://www.japan-guide.com/e/e2224.html

〒 106-0044  
東京都港区東麻布 1-8-1  
東麻布 IS ビル 4F

Yagita Asami  
Higashi Azabu IS Bldg 4F  
Higashi Azabu 1-8-1  
Minato-ku Tokyo 106-0044
