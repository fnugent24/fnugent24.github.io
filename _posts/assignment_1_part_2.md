# Assignment 1 part 2

### Description of the implementation and instructions on how to execute the code

An empty dictionary is created called "phone_book" which is used to
store the entries in.

Dictionary called "phone_book" will be coded as: 
phone_book = {}

The application will start running by associating a variable
("phone_book") with the Boolean value set to True (Drake, 2001, Python
3.11.2). This opens the loop and enables the application to keep running
until the Boolean value becomes False. The user is provided with the
main menu of the application in which they are given 4 options to
choose. Each option can be accessed by entering the designated number.
The main menu will be declared using the while loop (Drake, 2001, Python
3.11.2: 8.2) to allow the user to access the menu multiple times. On the
menu screen, the user will also be prompted to input a number. This is
created with a variable called "choice".

code would run as: 
while True: 
	print("Menu options") 
	print(" 1 - Add Contact") 
	print(" 2 - Search Contact") 
	print(" 3 - Delete Contact")
	print(" 4 - Quit Application") 
	choice = input("Enter an option: ")

Choosing one of the four options will be declared using if statements
(Drake, 2001, Python 3.11.2: 8.1). This will be so that the user can
choose any option they wish and do so in any order they wish. Inputting
"1" will prompt the user to input a person's contact details (name, age
and phone number) into the application. The application stores the age
of the contact using the built-in function called int. This is so that
the user must enter an integer rather than inputting characters. If they
do so, they will be met with the following error: 
ValueError: invalid literal for int() with base 10: ''

After entering these details, they will be stored on the application (in
the dictionary called "phone_book").

code would run as: 
	if choice == '1': 
		name = str(input('Name:'))
		age = int(input('Age:')) 
		phone_number = input('Telephone Number:')
		book[name] = age, phone_number

For example, the user would enter: 
Name: Michael Flower 
Age: 27
Telephone Number: 07324236457

User will have to enter "1" again on the main menu to add a further
contact. If they did, they would do the same as before:

Name: Henry Yates 
Age: 44 
Telephone Number: 094534563453

Name: John Mann 
Age: 52 
Telephone Number: 0943536346

Name: Jennie Wates 
Age: 37 
Telephone Number: 09346365363

Name: Peter Mill 
Age: 17 
Telephone Number: 0943636436

Entering number 2 on the main menu will allow the user to search for a
person's contact details stored in the application, including their age
and phone number. This option will be implemented by prompting the user
to input the name of the contact that they wish to search for. The
application would then output the age and number associated with that
contact. The application does this by searching for the name entries
stored in the dictionary "phone_number", and outputting the age and
phone number also associated with that name.

code would run as: 
elif choice == '2':
	name = str(input('Name of contact:'))
	print("Their age and phone number is:",phone_book[name])

For example, the user would enter: 
Name of contact: Michael Flower 
The application would output: 
Their age and phone number is: 27, 07324236457

The user would have to choose option 2 again in the main menu to search
for a different contact. Again, as an example, the code would run as:

Name of contact: Henry Yates 
The application would output: 
Their age and phone number is: 44, 094534563453

Entering number 3 will give the option to delete a person's contact details that are stored in the application. The "delete contact" option (number 3) will be implemented using the del statement, which will delete all the data associated with that specific contact - name, age and phone number.

code would run as: 
elif choice == '3': 
	name = input('Name:') 
	del phone_book[name]

For example, the user would enter: 
Name: Michael Flower

The application would delete the information associated with this
contact stored in the dictionary "phone_book" and the user would be
taken back to main menu. If the user searches for this name again
without adding it as a new contact, they will be met with an error
saying KeyError with the name of that now-deleted contact. For example:
KeyError: 'Michael Flower'

Entering number 4 will force the user to quit the application. This
option will be implemented by using the in-built "break" statement
(Drake, 2001, Python 3.11.2: 4.4). This will terminate the while loop
that is used to run the application.

code would run as: 
elif choice == '4': 
	break

The application will also prompt the user to click on a number between
1-4 if they enter a different number or input letters while in the main
menu. The application will remain running even if the user enters the
wrong number.

code would run as: 
	else: 
		print("click on a number 1-4")
