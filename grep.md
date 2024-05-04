# grep command 

grep :-	The grep command is a powerful text search utility commonly found in Unix-like operating systems.It allows you to search for specific patterns or regular expressions within files or input streams and print the matching lines.

-   grep 								:-						Search for a specific word in a file.
	
    ```
    grep "apple" file.txt
    ```

### grep command switch 

-   -i 									:-						Search for a pattern case-insensitively and display line numbers.
    
    ```
    grep -i "apple" file.txt
    ```
-	-v									:-						Invert the match. Display lines that do not match the pattern.
	```
    grep -v "apple" file.txt
	```		
-   -E									:-						let's use the grep -E command to search for lines that contain words starting with either "ap" or "gr.
			
    ```
    grep -E "(ap|gr)" data.txt
    ```
-   -r										:-						Search for a pattern recursively in a directory.
	
    ```
    grep -r "pattern" directory/
    ```
-	-l										:-						Only list the names of files that contain the pattern.
	
    ```
    grep -l "apple" directory/
    ```
-   -n									:-						Print line numbers along with the matching lines.
	```
    grep -n "apple" file.txt
    ```
-   -w									:-						Match whole words only.
	
    ```
    grep -w "apple" file.txt
    ```


**Examples :** 

	
-   ```
    grep “pattern search” file.txt 
	```		
-   ```   
    grep -i “pattern search”  file.txt
    ```
-	```
    grep -E “( pattern1 | pattern2 )” file.txt			
    ```
-   ```
	grep -E “( pattern search1 | pattern search2 )” file.txt
    ```
-   ```
    grep -E "( localhost journal | localhost kernel )" messages  			
	```
-   ```		
	grep -E "( localhost journal | localhost kernel )" messages | grep failed
	```
-   ```		
	grep -v “localhost kernel” messages 	
    ```
-   ```
	grep root. messages 	
	```
-   ```		
	grep "root\." messages 
    ```
-   ```
	grep root\. messages
	```
-   ```		
	grep root\.$ messages 	
	```
-   ```		
	grep “^Jun 1 ” messages 	
	```
-   ```		
	grep -E "( localhost journal | localhost kernel )" messages | grep -E "( OK | failed )"
	```
-   ```		
	grep -E "( localhost journal | localhost kernel )" messages | grep -vE "( OK | failed )"
    ```
-   ```
	grep "^#" sshd_config
	```
-   ```	
	grep -v "^#" sshd_config
	```
-   ```		
	grep -vE "( ^# | ^$ )" etc/ssh/sshd_config
	```
-   ```		
	grep -E "( ^# | ^$ )" etc/ssh/sshd_config
	```
-   ```		
	grep “^$” etc/ssh/sshd_config 		
	```
-   ```		
	grep -v “^$” etc/ssh/sshd_config 			
	```
-   ```			
	grep -vE "( ^# | ^$ )" etc/yum.conf | grep s.
	```
-   ```	
	grep -vE "( ^# | ^$ )" etc/yum.conf | grep s.*	
	```
-   ```		
	grep -vE "( ^# | ^$ )" etc/yum.conf | grep [sa]		
	```
-   ```		
	grep -vE "( ^# | ^$ )" etc/yum.conf | grep [0-9]
	```
-   ```
	grep -vE "( ^# | ^$ )" etc/yum.conf | grep [a-z]	
    ```
-   ```
	grep [0-9] user.txt		 
	```
-   ```		
	grep [123] user.txt		 
	```
-   ```
	grep “123” user.txt		 
	```
-   ```
	grep [0123456789] user.txt			 
	```
-   ```
	grep [0-9] [0-9] user.txt				 
    ```
-   ```
	grep [0-9] [0-9] [0-9] user.txt	 
    ```
-   ```
	grep [A-Z] user.txt							 
    ```
-   ```
	grep -o "localhost" messages 	 	
    ```
-   ```
	grep root *											 
    ```
-   ```
	grep -Rn root /etc 								 
    ```
-   ```
	grep -l root /etc 									 
    ```
-   ```
	grep "^./Desktop" file.txt	
    ```
	
	