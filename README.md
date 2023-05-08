# Relaible Kitchen



## Author:



- [Shvet Kantibhai Anaghan](shvetanaghan28@gmail.com)

## About:



- I created an application that can keep track of all the raw materials/ingredients available in the kitchen. Before accepting any orders online it should validate that sufficient ingredients are available in the kitchen and it should also keep track of the consumption of the raw materials in case the quantity reduces below a set level it should send an order to the retailers for the same.

## List of Features:



- This application has user Authentication and user Authorization features for security. Also, an ingredients module can track the number of ingredients available in the inventory. Admin can add new ingredients, modify the existing ingredients and change the number of availability, and set the threshold quantity for every ingredient. In the Food and Beverages section, there is a list of food and beverages along with the add new item option. Through the Order module, the admin can verify the order item's ingredients. If all the ingredients are available to make the order complete then the order will accept. And if the required ingredients are not available the order will reject along with a specific reason.

- There is a also cronjob feature for the ingredients shortfall. A cronjob will run at a configured schedule and trigger an event. This event will check for the shortfall in the quantity of the ingredients present in the kitchen. It will fetch all the ingredients whose available quantity is less than the desired minimum quantity. If there are such ingredients then the system will calculate the quantity for which the order needs to be placed to the distributor/retailer. The calculation will be done to identify the quantity which is the difference between the minimum desired quantity and the availability and additional ‘X’ percentage as configured in the system as buffer value. Each ingredient with the calculated quantity to be ordered will be pushed into the order list. Then this final list will be sent to the Distributor/Retailer for further processing.

## Folder Structure Used



- MVC or Model-View-Controller is a widely-used software design pattern that is often used in web application development. In a typical MVC architecture, the Model represents the data and the business logic, the View represents the user interface, and the Controller acts as an intermediary between the Model and the View. In your Spring Boot project, you have implemented the MVC architecture, where the Model would represent the data and the business logic related to my application, the View would represent the user interface, and the Controller would handle the user input and update the Model and View accordingly.

- By using the MVC architecture in my application, I can benefit from a number of advantages. Firstly, it helps to keep my code organized and maintainable by separating the different components of the application. Secondly, it makes it easier to test each component of the application separately. Thirdly, it allows for easier collaboration among team members working on different components of the application. Fourthly, it enables to reuse the components of the application in other projects with minimal modifications. Overall, implementing the MVC architecture in my Spring Boot project can help me to build a reliable and maintainable kitchen application.

## Prerequisites:


To run this application on your machine, You need to install git first. below is the link that will guide you to install Git on your machine.

- [Git Guides - Install Git](https://github.com/git-guides/install-git)

After Installing Git,

The first step is to clone the repo in your machine using the below command. Run the below command at the destination in cmd where you want to clone the repository.

```
git clone https://git.cs.dal.ca/snpatel/csci-5709-grp-02
```

Next, Change the directory to the client side of the project using:

```
cd .\csci-5709-grp-02\client
```

Next step is, run the below command to instal all the packages and dependencies that is required to run the Assignment.

```
npm install
```

You are all set and now just run the client side using following command.

```
npm start
```

Now, To run the server side of the Assignment, open the cmd with the path of the project's repo.

Next, Change the directory to the server side of the project using:

```
cd .\csci-5709-grp-02\server
```

Next step is, run the below command to instal all the packages and dependencies that is required to run the Assignment.

```
npm install
```

You are all set and now just run the server side using following command.

```
npm run dev
```

Both the server and client are now up and running.
