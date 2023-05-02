# Bandit
Report on attempt to solve bandit wargame by OverTheWire
### **Level 0-password-bandit0**
Pretty straightforward had to ssh into use bandit0@bandit.labs.overthewire.org on port 2220
Command used -> ssh bandit0@bandit.labs.overthewire.org -p 2220
password bandit0
on logging into user bandit0 and listing all the files using “ls” command a readme file is found
on opening the readme file using cat readme it gives the password for the next level
### **Level 1-password-NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL**
On sshing into user bandit1 and running the ls command met with a file named –
Access the file using the command cat ./-
The file gives the password for the next level
### **Level 2-password-rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi**
On running the ls command met with a file named “spaces in this filename”
Access the file using the command cat ‘spaces in this filename’
The file gives the password for the next level
### **Level 3-password-aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG**
The command ls reveals a directory inhere
On cding into the directory ls reveals nothing
On running, ls with the -a parameter reveals a hidden file .hidden
On opening the file using cat .hidden gives the password for the next level
### **Level 4-password-2EW7BBsr6aMMoJ2HjW067dm8EgX26xNe**	
We are met with the same directory inhere
On cding we are met with a few files named file01-file09
Clue says the password is contained in human-readable files among them
 Using the “file” command reveals that file07 is the only ASCII text file 
Opening it gives the password for the next level
### **Level 5- password-lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR**
Met with the same directory inhere
Cding into it shows numerous directories named maybehere00-maybehere19
Cding into I shows more files
The properties of the file are given in the clue as human-readable 1033 bytes in size and non-executable
after running man find and looking for possibly useful tags cding back into the inhere directory and searching for the specified file using the command find -type f -size 1033c ! –executable returns the file ./maybehere07/.file2
opening it gives the password for the next level
