# LORI's Grocer

## Master login info:
ID: 1
Password: x

## Statement of Problem: 
Tasked to make a database python program that can do CRUD using sqlite. There are 3 tables, inventory, employee and sales.
We were tasked with Lori's grocer, so we made our tables and the database relevant to a grocery store.
There are 3 positions for the employees, owner, supervisor and cashier. Owner has access to every function and menu, while
supervisors and cashiers have limited access.

## How it works:
There are functions for every menu, and certain functions are stored in different files for superior organization.
Each menu either calls another sub menu, or a function from the functions.py file, that will run one of the CRUD functions.
Before you can access the menu, there is a sign in(file: encryption.py) where the program knows what position you have in 
order to restrict certain functions.
There is error checking functions for inputs to ensure the program doesn't crash, and the user input is correct.
For a more in depth user manual, check README.md

## Known errors and limiations:
The item name in inventories have to be lower case, when doing accessing, modifying, and removing.
The user cannot quit the program or go back once they've entered a non-menu function when they 
don't know the correct input.
Commas can possibly create problems in certain string inputs when doing a sqlite execution. This is extremely rare.

## Response to testing:
Allow the user to quit when they don't know a response.
Error check strings for commas.
The while loops would probably be done differently, since we require an abudance of breaks.
We would keep the functions.py and error.py files, since they are very modular and versatile.
