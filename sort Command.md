# sort command 

sort :-	The sort command is a utility used in Unix and Unix-like operating systems to sort the lines of a file or input in either ascending or descending order. It takes input from a file or standard input, sorts it, and outputs the sorted result.
																	
-   sort filename.txt		:-					Sort the lines of a file using a specific field as the key.

    ```
    sort filename.txt		
    ```

### sort command switch

-   -r										:-					Sort the lines of a file in reverse order.
			
    ```
    sort -r filename.txt
	```		
-   -n 									:-					Sort the lines of a file numerically.
			
    ```
    sort -n filename.txt
	```		
-	-b 									:-					Sort the lines of a file ignoring leading blanks.
			
    ```
    sort -b filename.txt
	```		
-   -k 									:-					Sort the lines of a file using a specific field as the key.
	
    ```
    sort -k 2,2 filename.txt
    ```
-   -t										:-					Sort the lines of a file using a custom field separator.
			
    ```
    sort -t ':' -k 3,3 filename.txt
	```		
-	-f										:-					Sort the lines of a file in a case-insensitive manner.
	
    ```
    sort -f filename.txt
	```		
-	--help							:-					Sort command help
			
    ```
    sort --help filename.txt
	```		

			
			




			
