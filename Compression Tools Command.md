 # Compression Tools
	
	A compression tool is a software program that is used to reduce the size of files or folders by compressing them. Compression is achieved by using
	algorithms that remove redundant or unnecessary data, resulting in a smaller file size.
	
	There are several commonly used compression tools available, including : 
	
1. bzip2 :- The bzip2 command is a compression tool used to compress and decompress files using the Burrows-Wheele block sorting text compression algorithm and the Huffman coding algorithm. It offers higher compression ratios compared to some other compression tools.
																	
    - 	bzip2 filename.txt		:-		Compressing a file.
			
    ```
    bzip2 filename.txt
    ```

    - 	bzip2 -d filename.bz2	:-	    Decompressing a file.
			
    ```
    bzip2 -d filename.bz2		
    ```	
    - 	bzip2 -v filename		:-	    Viewing compression statistics.
	
    ```
    bzip2 -v filename
    ```

2. gzip :-  The gzip command is a compression tool used to compress and decompress files using the gzip algorithm. It commonly used in Unix and Linux systems.
															
    - 	gzip filename.txt	:-  Compressing a file.
	
    ```
    gzip filename.txt
    ```

    -  	gzip -d filename.gz     :-	    Decompressing a file.

    ```
    gzip -d filename.gz		
    ```

    - 	gzip -v filename       :-	   Viewing compression statistics.

    ```
    gzip -v filename
    ```

    - 	gzip file1 file2 directory	    :-	    Compressing multiple files or directories.
	
    ```
    gzip file1 file2 directory	
    ```

3.  zip		:-	    The zip command is a compression tool used to create, manage, and extract ZIP archives. It is commonly used in various operating systems, including Windows, Linux, and macOS.
						
    - 	zip archive.zip file1 file2 directory	    :-      Creating a ZIP archive.
			
    ```
    zip archive.zip file1 file2 directory				
    ```

    - 	zip archive.zip additionalfile	    :-		Adding files to an existing ZIP archive.

    ```
    zip archive.zip additionalfile				
    ```

    -	zip -u archive.zip file1 file2		:-		Updating an existing ZIP archive.

    ```
    zip -u archive.zip file1 file2
    ```

    - 	unzip archive.zip       :-	    Extracting files from a ZIP archive.
	
    ```
    unzip archive.zip
    ```

    - 	unzip archive.zip file1 file2	    :-		Extracting specific files from a ZIP archive.
    
    ```
    unzip archive.zip file1 file2
    ```	
		
4. 7za	:- The 7za command is a command-line tool used to create, extract, and modify archives using the 7z compression format. The 7z format is known for its high compression ratio and supports various compression algorithms, including LZMA, LZMA2, and BZIP2.

    - 	7za a archive.7z file1 file2 directory		:-		Creating a 7z archive.
    
    ```
    7za a archive.7z file1 file2 directory
    ```

    - 	7za x archive.7z file1 file2	    :-		Extracting files from a 7z archive.
	
    ```
    7za x archive.7z file1 file2
    ```

    - 	7za x archive.7z file1 file2        :-		Extracting specific files from a 7z archive.
	
    ```
    7za x archive.7z file1 file2
    ```

    - 	7za u archive.7z additionalfile		:-		Adding files to an existing 7z archive.
	
    ```
    7za u archive.7z additionalfile
    ```

5. tar 	:- The tar command is a utility used in Unix-like operating systems to create, list, extract, and manipulate files within tar archives. Tar archives are commonly used for bundling multiple files and directories into a single file.

    - 	tar -cf archive.tar file1 file2 directory	    :-	    tar -cf archive.tar file1 file2 directory.	
	
    ```
    tar -cf archive.tar file1 file2 directory
    ```
    - 	tar -xf archive.tar		:-      Extracting files from a tar archive.
	
    ```
    tar -xf archive.tar
    ```

    - 	tar -xf archive.tar file1 file2		:-		Extracting specific files from a tar archive.
	
    ```
    tar -xf archive.tar file1 file2
    ```

    - 	tar -rf archive.tar additionalfile		:-		Adding files to an existing tar archive.
	
    ```
    tar -rf archive.tar additionalfile
    ```

    - 	tar -tf archive.tar		:-		Listing files in a tar archive.
	
    ```
    tar -tf archive.tar
    ```














																
			
				
		
				
																			
