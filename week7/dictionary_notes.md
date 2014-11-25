*** DICTONARY ***

[copy PWP/week5/dictionaryINPROGRESS.py into TextWrangler] 

Testing it Out

	Test the app out for a few minutes and see what works, what doesn't

	What is Nonfunctional?
	What can be improved?
	Looking at the code, what can be improved?


Add a FindAll Function

	1) open file for reading
	2) readlines into list
	3) split lines into word,def
	4) print word,def

Deleting Words from the Dictionary

	1) finding word in file and updating it is hazardous

	2) finding word in a list constructed from the file is fine,
	but deleting it is tricky

	3) take the list constructed from file and copy it into a new list,
	but filter what you don't want

Updating Words in the Dictionary
	
	1) read file into list called lines
	
	2) use enumerate too loop through lines
	
	3) if a line.split(',')[0] matches the word to update
		+ show current word and def
		+ get user input for revision
		+ if that is > 0 in length, modify lines[num] with new string
		+ use ''.join(i for i in [word,' , ',new_definition,'\n']) to match format

Writing a Database Object

	1) create separate file called database.py (lowercase d)

	2) Functionality?
		initialize variables
		display which file it's using
		find a word
		find all words
		delete a word
		update a word
		(same funcs from our previous program, but bound to the db obj)

	3) class Database:
	(notice Database is capitalized, per convention

	2) define your database class and give it an init method that takes in a filename
	and stores it as self.db_file
	
	3) write a getDbName() function that prints self.db_file

	3) go to main and create the database object, call it db.

	4) review: 
		database.py file is 'database'
		Database is the class
		db = Database('default.db') -> db is object
