# awk command 

awk 	    :-		The awk command is a versatile text processing tool used in Unix-like operating systems. It allows you to manipulate and analyze text files by applying pattern matching and performing actions based on the matched patterns. Here's the basic syntax of the awk command.
																
-   awk '/pattern/ { print }' file.txt 				:-						Print lines containing a specific pattern.
	
    ```
    awk '/pattern/ { print }' file.txt
    ```
-   awk '{ print $1, $3 }' file.txt			:-			Print specific fields from a file (fields are separated by a delimiter, often space or tab).
			
    ```
    awk '{ print $1, $3 }' file.txt
	```
-   awk '{ sum += $2 } END { print sum }' file.txt			:-					Calculate and print the sum of values in a specific column.
	
    ```
    awk '{ sum += $2 } END { print sum }' file.txt
    ```
-   awk 'length > 80' file.txt							:-						Print lines longer than a certain length.
			
    ```
    awk 'length > 80' file.txt
	```		

### awk command switch 

-   -F	:-	The command you provided is an awk command that uses a colon (:) as the field separator (-F) and prints the first field followed by a hyphen and a space ($1, " - "), and then prints the second field ($2). However, there is a typographical error in your command. The closing double quotation mark after the hyphen is a curly closing quotation mark (“) instead of a regular double quotation mark (").
		
    ```
    awk -F: '{print $1," - ",$2'} file.txt
    ```			
-   -f 	:-	The awk command provides the -f option to specify a file containing the awk program. This allows you to write your awk script in a separate file and reference it using the -f option. Here's the syntax:
			
    ```
    awk -f script.awk file.txt
    ```
-   --help 							:-						awk command help 
    ```
    awk --help 
    ```

**Example :**


-	```
	awk '{print $0}' /etc/passwd
	```		
-	```
	awk '{print $1}' /etc/passwd 	
	```		
-	```
	awk '{print $1,$2,$3}' /etc/passwd
	```
-	```		
	awk '{print $1,"local",$2}' /var/log/messages
	```
-	```		
	ifconfig | awk '/inet/{print $2}'	
	```
-	```		
	awk -F: '{print $1,$2,$3}' /etc/passwd
	```
-	```		
	awk -F: '{print $1," - ",$2'} /etc/passwd 
	```		
			
### Basic Structure
			
- 	awk 'progaram_you_will_write' input-file1 input-file2

- 	awk 'BEGIN( code_in_BEGIN_section ) (code_in_main_body_section) END( code_in_END_section)' input-file1 input-file2

-	```
			BEGIN {

        	print "Start line"

        	}

	{
        	print $1, "home at" ,$6

        	}

	END {

        	print "End line"
        	}
	
**Example :**	


	'BEGIN{ print "Start line"}
			
	{print "home at"}
			
	'END { print "End line"}	

			
-	```
	echo "one two three four" | awk 'BEGIN{print "Start line"} {print $0} END{print "End line"}'
	```		
-	```
	echo "one two three four" | awk '{print $1 "," $2}'
	```		
-	```
	ifconfig | awk 'BEGIN{ print " IP Add "} /inet /{print $2}'	
	```		
-	```
	ifconfig | awk 'BEGIN{ print “ IP Add “} /inet /{print $2}' END {print "===="}'
	```		
-	```
	cat /etc/passwd | awk -F: '{print $1 $6}'		
	```		
-	```
	echo one two | awk '{$1="ONE";print $1}'		
	```
-	```
	ifconfig | awk '$1=="inet" {print $0}'										
	```
-	```
	cat /etc/passwd | awk -F: '$1=="root"{print $0}'
	```	
-	```
	cat /etc/passwd | awk -F: '/root/ {print $0}'			
	```	
-	```
	awk -F: '$3>=1000 {print $0}' /etc/passwd
	```		
-	```
	awk -F: '$3>=0 {print $0}' /etc/passwd 									 
	```	
-	```
	awk -F: '$3<=0 {print $0}' /etc/passwd 										 
	```
-	```
	awk -F: '$3==0 {print $0}' /etc/passwd 				
	```
-	```
	cat /etc/passwd | awk -F: 'BEGIN{print "Start line"} {print $1, "home at" ,$6} END {print "End line"}'
	```		
-	```
	awk "(print $1 - $2)"							 
	```
-	```
	awk "(print $1 * $2)"							 		
	```
-	```
	awk "(print $1 / $2)"							 
	```
-	```
	awk '/\troot/{print $0}' user.txt		
	```
-	```
	awk '!/root/{print $0}' user.txt 		 
	```
-	```
	awk '/^root/{print $0}' user.txt
	```
-	```
	awk '/root$/{print $0}' user.txt 
	```
-	```
	awk '{print NF}' /etc/passwd 			 
	```
-	```
	echo "one two three four" | awk '{print $NF}'		
	```
-	```
	ifconfig | awk '{print NR}'					
	```



 	
	