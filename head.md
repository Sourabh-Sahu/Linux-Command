# head command 

	head :-	The head command is a utility used in Unix and Unix-like operating systems to display the beginning lines of a file or input. It is typically used to preview the contents of a file or extract a portion of a file.
			
- 	head filename.txt	:-	Display the first 10 lines of a file.
			
    ```
    head filename.txt	
	```

### head command switch 

- 	-n 	:-					Display the first 50 lines of a file.
	
    ```
    head -n 50 filename.txt		
	```	
- 	-c :-					Display the first 100 bytes of a file.

	```
    head -c 100 filename.txt		
	```	
- 	-q :-					Display the first 5 lines of multiple files, without file name headers.
	
    ```
    head -n 5 -q file1.txt file2.txt file3.txt
	```	
- 	-v 	:-					The head -v command is used to display the file name header when using the head command.

	```
    head -v filename.txt
	```	
- 	--help :-					head command help 

	```
    head --help
	```	

		



			
			
			
 