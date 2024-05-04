# paste command 

paste 	        :-			The paste command is used to merge lines from multiple files or standard input and display them side by side. It is typically used for    combining data horizontally by joining corresponding lines. Here is a description of the paste command.
			
-   paste 							:-							Merging lines from two files side by side.
			
    ```
    paste file1.txt file2.txt
    ```

### paste command switch 

-	-d									:-							Merging lines from two files side by side with a custom delimiter.
	
    ```
    paste -d ',' file1.txt file2.txt
    ```
-   -s									:-							Concatenating lines from multiple files serially:
	
    ```
    paste -s file1.txt file2.txt
    ```
-   --help 							:-							paste command help 
		
    ```
    paste --help 
    ```