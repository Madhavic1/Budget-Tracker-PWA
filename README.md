# Budget-Tracker-PWA
 Online/Offline Budget Trackers

## User Story
AS a avid traveller
I WANT to be able to track my withdrawals and deposits with or without a data/internet connection
SO THAT my account balance is accurate when I am traveling

## Business Context
Giving users a fast and easy way to track their money is important, but allowing them to access that information anytime is even more important. Having offline functionality is paramount to our applications success.

## Desciption
This is a Budget Tracking application, which takes name of the Transaction, transaction amount as user inputs and adds or subtracts the amount from the total depending on the button click on Add Funds or Subtract Funds buttons respectively. Using this apllication, the user will be able to add expenses and deposits to their budget with or without a connection. When entering transactions offline, they will populate the total on backend when brought back online.

The Offline Functionality allows the user to perform the following operations in the app.
  * Enter deposits offline
  * Enter expenses offline
When brought back online:
  * Offline entries will be added to tracker.

To make this apllication as a PWA, Progressive Web Application, I used Service Worker and Cache APIs to cache assets and API responses to ensure this application works without an internet connection. I used indexedDB, a low-level API for client-side storage, to store the transactions the user make when he/she is offline, without internet connection. As and when the user gets the internet connection, the data stored in the indexedDb will be posted to the MongoDB, which serves as a main database for the apllication and the data in the indexedDB will be cleared for futher usage.

## Launching the application
After you get the source code of the application, execute the command "npm install" to install all the node modules needed by the application to perform all of its jobs mentioned in the application and then execute the command "npm start". Once the server is up and running, you can open this application by accessing the link "http://localhost:3000/" in your local machine.

## How to install this application as a native app?
Once the server is up and the application is running ion the localhost, you will find a little "+", plus, symbol at the end of the address bar, where you typed "http://localhost:3000/". After clicking the plus symbol and clicking on install button from the browser pop-up dialogue, the application will be installed on your local machine and you can use it as a native app.

### Technologies Used
* HTML
* CSS
* Javascript
* Node js
* Express js

### Link to the git repository
https://github.com/Madhavic1/Budget-Tracker-PWA.git

### Link to Deployed Application on heroku
https://glacial-peak-07886.herokuapp.com/
