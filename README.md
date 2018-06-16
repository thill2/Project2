# ScaleUp!
## Project 2

## Background
This app is called ScaleUp and it was done as a project for the February 2018 UNC Coding Boot Camp.

## How to get started with the app
The application is online at https://scale-up20182.herokuapp.com/. You will more than likely have to wait a little while after visiting this url before Heroku spins up the virtual machine which hosts the project.

Please install Git Bash, MySQL, and Node.js if you want to use the app locally. 

After all of these are installed, you can download the GitHub Repo.

In the project's root directory:
  Install the database from the command line by by entering:

      mysql -u root -p < schema.sql
      Enter password: <enter password here>

      mysql -u root -p < seeds.sql
      Enter password: <enter password here>

  Next install the project dependencies by entering:

      npm install

The project is now ready to run!

Start the server by typing in:

    node server.js

Open a browser and navigate to:

  http://localhost:8080/ 

in the address line.


You can enter utilities for Building 1, Zones 1-3, & Building 2, Zones 1-3

Navigate over to the results page, and you'll see the percent utilization for each of the zones in each building.  You can click on any of the zones aboe the chart to temporarily remove them from the chart.

## Authors
This app was built by Jeannie Rose, Walheed Hamza, & Tony Hill.

## Issues we encountered
The charts on the results page are not generated dynamically, and expecting data to be entered exactly as explained above.  Given more time we could have added this functionality. 

The foreign keys in mySql are not operating as intended.  Because they are based off of primary keys which are autoincrementing, each time a building or zone is entered, a new primary key and thus new foreign key is created.  This could have been resolved by generating foreign keys based on building or zone names as opposed to primary keys.
