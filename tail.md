# tail command 

tail :-	The tail command is a utility used in Unix and Unix-like operating systems to display the ending lines of a file or input. It is commonly used to view the last few lines of a file or to continuously monitor the contents of a file as it grows.
			
- 	tail filename.txt	:- Display the last 10 lines of a file.
	
	```
    tail filename.txt		
	```

### tail command switch 

- 	-n 									:-					Display the last 10 lines of a file.
			
    ```
    tail -n filename.txt
	```		
- 	-c 									:-					Display the last 100 bytes of a file.
	
    ```
    tail -c 100 filename.txt
	```		
- 	-f										:-					Continuously monitor a file for appended data.
	
    ```
    tail -f filename.txt
	```		
- 	-q 									:-					Display the last 5 lines of multiple files without file name headers.
	
    ```
    tail -n 5 -q file1.txt file2.txt file3.txt
    ```
- 	-v 									:-					The tail -v command is used to display the file name header when using the tail command.
	
    ```
    tail -v filename.txt
	```		
- 	--help 							:-					tail command help 
	
    ```
    tail --help 
    ```


			
