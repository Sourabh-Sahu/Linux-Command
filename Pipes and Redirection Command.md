# Pipes and Redirection 


-	command1 ; command2 ; command 3		:-		Multiples command at Once 
	
	```
	id ; date ; pwd 			 
	```

- 	command1 && command2 && command3		:-		Multiples command at Once 
	
	```
	id && date && pwd 
	```

- 	less		:-		View a file.(q key exit , space key next page , enter key next line , up key up line , down key down line )

	```
	less file.txt 
	```			

- 	more 		:-		View a file.(q key exit, space key next page , enter key next line)
			
	```
	more file.txt							
	```	

-  	ifconfig | wc   	:-		The wc command is used to count the number of lines, words, and characters in a file or	standard input.
		
	```	
	ifconfig | wc									
	```

- 	ifconfig | wc-l 	:-		The command ifconfig | wc -l is used to count the number of lines in the output of the ifconfig command. 
			
	```
	ifconfig | wc-l 
	```

- 	ifconfig | wc-w 	:-		The command ifconfig | wc -w is used to count the number of words in the output of the ifconfig command. 
			
	```
	ifconfig | wc -w		
	```
			
- 	ifconfig | wc -c		:-		The command ifconfig | wc -l is used to count the number of characters in the output of the ifconfig command. 

	```
	ifconfig | wc -c 
	``` 		

- 	ifconfig > newfile.txt		:-		The command ifconfig > newfile.txt is used to redirect the output of the ifconfig command to a new file named "newfile.txt".

	```
	ifconfig > newfile.txt						
	```

- 	ifconfig >> newfile.txt		:-		The command ifconfig >> newfile.txt is used to append the output of the ifconfig command to an existing file named "newfile.txt". 
		
	```
	ifconfig >> newfile.txt
	```		

- 	wc < filename.txt		:-		The command wc < filename.txt is used to redirect the contents of a file, filename.txt, as input to the wc command. 
		  	
	```
	wc < filename.txt
	```		
