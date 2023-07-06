# cp command 

cp 		:-		The cp command in Linux is used to copy files and directories. It allows you to duplicate files and directories, either within the same directory or to a different location.
																	
- 	cp source_file destination	:-	Copy a single file to a destination.
			
```
cp source_file destination		
```

- 	cp source_file1 source_file2 destination	:-	Copy multiple files to a destination:

```
cp source_file1 source_file2 destination			
```

### cp command switch 

- 	-r	:-	Copies directories and their contents recursively. This option is necessary when copying directories.
			
```
cp -r source_directory destination_directory
```

- 	-i	:-	Prompts for confirmation before overwriting an existing file.
			
```
cp -i file_name destination_directory
```
- 	-v	:-	Displays detailed output, including the names of files being copied.

```
cp -v file_name destination_directory
```			
- 	--help	:-	cp command help
			
```
cp --help
```			
