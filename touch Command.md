# touch Command

 touch : The touch command in Linux is used to create new empty files.

- 	touch								:-				Creating a new file
	
    ```
    touch file.txt
    ```

- 	touch file1 file2			:-				Creating multiple files
	
    ```
    touch file1 file2 file3 file4
  	```

- 	touch path/file.txt		:-				Specifying the path
	
    ```
    touch /root/file.txt
	  ```
- 	touch "file name" 		:-				" " Space cover 
	
    ```
    touch "file name"		
    ```

_touch command switch_ 		
		
- 	-m											:-				change only the modification time.
		
        touch -m file.txt
		
- 	-c 											:-				Do not create a new file if it doesn't exist.
	
    	touch -c file.txt
		
- 	-r 											:-				Use the timestamp of the reference FILE instead of the current time.				
		
        touch -r reference.txt myfile.txt

- 	-d											:-				Use the specified STRING as the new timestamp value instead of the current time.
	
    	touch -d "2022-12-31 23:59:59" file.txt
		
- 	-t 											:-				Use [[CC]YY]MMDDhhmm[.ss] instead of current time change the specified time.

		touch -t 202106231530.45 file.txt

- 	--help									:-				touch command help 

		touch --help 			

		
		
