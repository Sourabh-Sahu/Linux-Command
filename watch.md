# watch command 

watch 	:-	The watch command is a utility available in Unix and Unix-like operating systems that allows you to
																	execute a command periodically and display the output in real-time. It repeatedly runs the specified
																	command and updates the display at a specified interval.

### watch command switch 

-	-n	:-	The watch -n command is used to specify the interval, in seconds, at which the watch command executes the specified command and updates the display. 			

```
watch -n 5 ls -l
```

- 	-d								:-					The -d option is used with the watch command to highlight differences between successive updates. It
																	enables the display of changes in the output of the monitored command between each execution.
			
```
watch -d ls -l 
```

- 	-t									:-					The watch -t command is used to disable the display of the title header when using the watch command. 
																	By default, the watch command shows a header that includes the current time and interval.
```
watch -t ls -l
```
			