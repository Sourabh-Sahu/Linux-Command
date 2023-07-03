
# rm Command 

rm	:-  The rm command in Linux is used to remove/delete files and directories. It allows you to delete single files, multiple files, or entire directories and their contents.
		
- 	rm 	file.txt	:-	Remove a single file.
			
    ```
    rm file.txt	
  	```

- 	rm file1.txt file2.txt file3.txt    :-	Remove multiple files.
		
    ```
    rm file1.txt file2.txt file3.txt
    ```


### rm command switch 
		
- 	-r	:-		Remove a directory and its contents recursively.
			
    ```
    rm -r file.txt				
	  ```

- 	-i	:-	Prompt for confirmation before deleting each file.
			
    ```
    rm -i file.txt					
    ```

- 	-f 	:-	Force removal without prompting for confirmation.
			
    ```
    rm -f file.txt					
  	```

-	-v	:-	Remove files and display verbose output.
	
    ```
    rm -v file.txt
  	```

- 	-d 	:-	Remove empty directories only.
	  	
  	```
    rm -d foldername 	
    ```

- 	-rf	:-	Remove a directory and its contents recursively without prompting for confirmation.
	
    ```
    rm -rf foldername 	
    ```

- 	*.txt :-	Remove files matching a specific pattern using wildcard.
			
    ```
    rm *.txt							
	  ```

- 	--help	:-	rm command help 
	
    ```
    rm --help  										
  	```		
