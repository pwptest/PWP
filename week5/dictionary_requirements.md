Menu Based Database application

Requirements:

1) Menu items (Add, Remove, Update, Delete, Quit)
1b) Use 'insert','lookup','update','delete' as function names, in accordance with the respective database terms

2) Menu doesn't cascade, meaning that each time an option is pressed, a new menu or display replaces the old one
3) The program should take our input as text and store it in a file
4) The program acts sanely.  For example, if the word is already in the file, it asks us whether we want to add an alternate
   definition, or overwrite what is there.
5) we treat an entry in the database as a 'transaction', meaning that we MUST close the file once we've written to it.

Improvements:
0) add option to enter words via file
1) lookup word by definition by matching some sub section of the definition stored
2) The program acts a little more sanely if the word is already in the file. We can add an alternate definition, overwrite one definition, or all of them
3) find a better method of ensuring files are closed properly
4) implement some sort of rudimentary 'did you mean X?' algorithm.
5) make it look nicer
6) Add a Quiz Menu Item etc for vocab
