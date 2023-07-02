# cat command 
		
cat     :-	The cat command in Linux is used to concatenate and display the contents of one or more files on the standard output (usually the terminal). 		
		
- 	cat file.txt    :-	Read file 
			
    ```
    cat file.txt	
  	```

- 	cat file1.txt file2.txt			:-			Multiple files read 
			
    ```
    cat file1.txt file2.txt
	  ```

- 	cat file1.txt file2.txt > combined.txt		:-		Multiple files into a single file.
			
    ```
    cat file1.txt file2.txt > combined.txt
    ```


### cat command switch



- 	-n 	:- 	Displays line numbers for all the lines in the output.
		
    ```
    cat -n file.txt
    ```

- 	-b	:-	Display the contents of a file with line numbers only for non-empty lines.
	
    ```
    cat -b file.txt
	  ```

- 	-s 	:-	Squeeze multiple adjacent blank lines into a single blank line.
		
    ```
    cat -s file.txt
	  ```

- 	-E	:-	Display the contents of a file with a $ symbol at the end of each line.
	
    ```
	cat -E file.txt
  	```

- 	-T	:-	Display the contents of a file with tab characters represented as ^I .
		
    ```
    cat -T file.txt
    ```
