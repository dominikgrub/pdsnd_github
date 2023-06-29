## Bikeshare Project

### Date Created
The bikeshare project was created 2nd of May 2023.

### Description
In this project, the goal is to **explore data related to bike share systems for three major cities** in the United States: Chicago, New York City, and Washington.
It includes computing a variety of **descriptive statistics** about popular times of travel, popular stations and trips, trip durations and user info. 
The user should be able to run through the program by answering which data they want to see (for examplefor which city, month, weekday).
After filtering the dataset, users will see different statistical result of the selected data, and choose to start again or exit.
The script also prompts the user whether they would like want to see the raw data at the end. If the user answers 'yes,' then the script should print 5 rows of the data at a time, then ask the user if they would like to see 5 more rows of the data. If not, they can end or restart the program.

### Coding Language Used
This project is based on Python.

### Hadnling Unexpected Input by user 
The project code is set up so that it can handle unexpected input well without failing. Below is an example of how to make sure that the _month_ comes in correctly.

`def month_input_validation(month_input):`

`        while True:`
        
`            month_user_entered = input(month_input).lower()`

`            try:`
            
`                if month_user_entered in ['january', 'february', 'march', 'april', 'may', 'june', 'all']:`
                
`                   break`
                   
`                else:`
                
`                   print('\nSorry, that was an invalid enter.')`
                   
`            except ValueError:`
            
`                   print('Your input is wrong.')`
                   
`        return month_user_entered`

`    month = month_input_validation('\nWould you like to see statistics for January, February, March, April,\nMay or June?\nPlease type month here (for all months type "all"): ')`

### Files Used
The main file containing the Python script is the following:

- _bikeshare.py_

There are 3 datasets, one per city each:

- _chicago.csv_

- _new_york_city.csv_

- _washington.csv_

### Credits
Udacity provided lots of useful hints on how to go through this project - **kuddos**!
