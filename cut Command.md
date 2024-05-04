# cut command

    cut 		:-			The cut command is a Unix/Linux command-line utility that is used to extract specific sections (columns) from lines of input or files.     It allows you to cut out fields or characters based on delimiter or byte positions.

			
### cut command switch 

-   -f 						:-					Specify fields or columns to extract.
	
    ```
    cut -f 2,4 file.txt
	```		
-   -d 						:-					Extracting fields using a comma as the delimiter.
			
    ```
    cut -d ',' -f 1,3 file.txt
    ```


**Example :**

-   ```
    cut -f1 -d " " file.txt				 
	```
-   ```	
	cut -f1,4 -d " " file.txt 		 
    ```
-   ```
	ifconfig | grep "inet " 		 
    ```
-   ```
	ifconfig | grep "inet" | cut -f9 -d " " 	
    ```
-   ```
	cut -f1 -d "/" file.txt		
    ```
-   ```
	cut -f1,2 -d "/" file.txt	
    ```
-   ```
	cut -f1,2 -d "/" file.txt | uniq 			
    ```
-   ```
	cut -f1,2 -d "/" file.txt | uniq -c 																				  
    ```
-   ```
	cut -f1,2,3 -d "/" file.txt	| uniq 	
    ```
-   ```
	cut -f1,2,3 -d "/" file.txt | grep "^./Desktop" 		
    ```
-   ```
	cut -f1,2,3,4 -d "/" file.txt | grep "^./Desktop/kf" 	
	```
