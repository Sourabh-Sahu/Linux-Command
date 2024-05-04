# sed command 

sed :-	The sed command is a powerful text-processing tool available in Unix-like operating systems. It stands for "stream editor" and is primarily used for performing text transformations on input streams or files.
			
### sed command switch 

-   -n 	:-	This command uses the -n switch to suppress automatic printing. It searches for lines in "input.txt" that contain the specified pattern and only prints those lines.
			
    ```
    sed -n '/pattern/p' input.txt
    ```
-   -e									:-							This command uses the -e switch to specify multiple script commands inline. It first replaces "foo"
																				with "bar" in each line and then deletes lines that match the specified pattern in "input.txt".
	```
    sed -e 's/foo/bar/' -e '/pattern/d' input.txt
    ```
-   -f										:-							This command uses the -f switch to provide a file (script.sed) containing sed script commands. It 
																				applies the commands from the script file to each line in "input.txt".
    ```
    sed -f script.sed input.txt
    ```
-   -i										:-							This command uses the -i switch to edit the file "input.txt" in place, replacing "foo" with "bar" in 
																				each line. It also creates a backup file with the extension ".bak" containing the original contents.
    ```
    sed -i.bak 's/foo/bar/' input.txt
	```
-   -r										:-							This command uses the -r switch to enable extended regular expressions. It matches any sequence 
																				of digits and replaces it with the same sequence followed by " is a number" in each line of 
																				"input.txt".
    ```
    sed -r 's/(\d+)/\1 is a number/' input.txt
    ```
-   -s									:-							This command uses the -s switch to treat each file (file1.txt and file2.txt) separately. It performs the 
																				search and replace operation independently on each file.
	```
    sed -s 's/foo/bar/' file1.txt file2.txt
    ```


**sed command Structure** 
		
- 	sed OPTIONS [SCRIPT] [INPUTFILE]
		
-	sed -n ‘1,5p’ user.txt
			
- 	cat [INPUTFILE] | sed OPTIONS [SCRIPT]
			
		SCRIPT :
			
				[addr]x[options]				
				
				[addr] can be a single line number, a regular expression, or a range of line. If [addr] is specified, the command x will be 
				expression only on the matched lines. 
				
				x is a single-letter sed command.
												
				Additional [options] are used for some sed command.
				
		Example :-  sed ‘20.25d’ user.txt
				
				    20,25 is an address range 
						
					d is the delete command 
						
*SED command* :
		
	    a text 	        -	    append text after a line 
				
		d 			    -	    delete the pattern space 
				
    	i text		    -		insert text before a line 
				
		p 			    -		print the pattren space 
				
		q [exit-code]	-	    (quit) Exit sed without processing any more command to input 
				
		s/range/replacement/[flags]		-	(substitude) Match th erregular expression the content of the parttern space. If found,
																							replace matched string with replacment.
				
_Command line options:_
				
		-n  			-		disable automatic printing sed only produces output when explicitly told to the p command.
				
		-e script 		-		add script 
				
		-r 				-		use extended regular expression rather than basic regular expression.
				

**Example :**

-   ```
	sed -n '/^$/p' passwd 						 
	```
-   ```	
	sed '/^$/p' passwd 	 
    ```
-   ```
	sed '/^$/d' passwd 	
    ```
-   ```
	sed '1p' passwd 	 
    ```
-   ```
	sed -n '1p' passwd	 
    ```
-   ```
	sed -n '2,5!p' passwd  
    ```
-   ```
	sed '1,5d' passwd				 
    ```
-   ```
	sed -n '/root/p' passwd 	 
    ```
-   ```
	sed '/root/p' passwd 			 
    ```
-   ```
	sed -n '/root/,+3p' passwd 
    ```
-   ```
	sed -n 's/root/ROOT/p' passwd 
	```
-   ```
	sed 's/root/ROOT/p' passwd 		 
    ```
-   ```
	sed 's/root/ROOT/g'	 passwd 				 
    ```
-   ```
	sed -n 's/root/ROOT/gp' passwd 
    ```
-   ```
	sed '/user/a name  ' user.txt  
    ```
-   ```
	sed '/user/i	 name' user.txt	 
    ```
-   ```
	sed '2a name'	user.txt			 
    ```
-   ```
	sed '2i name'	user.txt 			 
    ```
-   ```
	sed '1,2a ----------------' user.txt	 
    ```
-   ```
	sed '1,$a ----------------' user.txt		  
    ```
-   ```
	sed '/\troot/d' user.txt								 
    ```
-   ```
	sed '/[[:digit:]]/d' user.txt							 
    ```
-   ```
	sed '/[[:space:]]/d' user.txt 						
    ```
-   ```
	sed '/[a-z]/d' user.txt							 		 
    ```
-   ```
	sed '/[a-zA-Z]/d' user.txt							  		
    ```
-   ```
	sed '/[0-9]/d' user.txt 								 
    ```
-   ```
	sed '/old name /c new name' passwd				
    ```
-   ```
	sed '1c name' passwd	 						 
    ```
-   ```
	sed '1e date' user.txt 									
    ```
-   ```
	sed '/root/e date' user.txt						 
    ```
-   ```
	sed '/root/e echo "one two three"' user.txt 
    ```
-   ```
	sed '1,$e echo "=============="' user.txt	
    ```
-   ```
	echo "one five three" | sed 's/five/two/' 			
    ```
-   ```
	echo "name 1000" | sed 's/[[:digit:]]\+/***/'	
    ```
-   ```
	echo "name 1895" | sed 's/[[:digit:]]/*****/'	
    ```
-   ```
	echo "name 1000" | sed 's/[0-9]\+/***/'		
    ```
-   ```
	sed 's /armour/ARMOUR &/g' user.txt						
    ```
-   ```	
	sed 's/.*/admin:&/' user.txt			 
	```
-   ```	
	sed -ne '/armour/p' -ne '/root/p' user.txt					    
    ```
-   ```
	sed -i -e '/root/a ROOT user' -e '/root/'i "-----------" user.txt
    ```
	 
