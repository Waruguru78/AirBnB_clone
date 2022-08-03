AirBnB Clone Project
Description
An airbnb clone project built with the aim to learn and apply the concepts of high level programming. It specifies classes for user, place, state, city, amenity and review that inherit from the BaseModel class. Instances are serialized and saved to a JSON file then reloaded and deserialized back into instances. Additionally, there is a simple command line interface or console that abstracts the process used to create these instances.

Requirements
Python 3

Installing
To clone this repository;

git clone git@github.com:Waruguru78/AirBnB_clone.git
cd AirBnB_clone./console.py

Usage
A console can run in two modes ie: interactive and non-interactive to manipulate your models.
Interactive mode;
To run the console type ;
	./console.py
Non-interactive mode;
To run the console type;
	echo “all” | ./console.py
Other commands supported include;
To create an instance of a specified class; 
	create [class_name]  Example: create BaseModel
To show the string of an instance;
	show [class_name][id]  Example: show BaseModel 1234-5678-4321
To delete an instance;
	destroy [class_name][id]  Example: destroy BaseModel 1234-5678-4321
To add or modify attributes of an instance
 	update [class_name][id][attribute][value] Example: update BaseModel 234-5678-4321 
To display help information for a command 
	help [command]  Example: help all
To exit the program
	quit

Tests
Testing is imperative to building any robust program thus the project uses the python unit test model for automated tests.
To run the entire unittest, use the command;

	python3 -m unittest discover tests

To run individual tests , use the command;

	python3 -m unittest tests/test_models/test_base_model.py
