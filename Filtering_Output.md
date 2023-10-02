
# Filtering Output
```timestamp-url 
 https://www.youtube.com/watch?v=-Z5tCri-QlI&list=PLtK75qxsQaMLZSo7KL-PmiRarU7hrpnwK&index=9
 ```


`03:48`
Cut Command 
```
cat <file_name> | cur -d: -f2
```
_________________________________________________________________________


## Video 2 Log Analysis
```timestamp-url 
 https://www.youtube.com/watch?v=L2BFDyYknIg
 ```

Topics Covered :
- cut
- sort
- uniq
- grep
- negative grep
	```grep -v "not needed"```
	- Removes the lines with the word **not needed**
- wc -l


_______________________________________________________________________

## Video 3 Mastering GREP
```timestamp-url 
 https://www.youtube.com/watch?v=DEgErzyUR2Q
 ```
- #### Excluding special characters in Grep using `-F`
  `07:54`
  
  ```
  grep -F "!@#$this is a text not special characters"
  ```



`-E is the enhanced regex which gives grep extra power to filter.`



- #### Using Enhanced regex with negative regex
  `16:13`

  **Exercise 1 : Removing lines with empty spaces and commented lines**
    
    ```
    grep -Ev "^($|#)" /etc/services
    ```

- #### ?
  `19:38`

  **Exercise 2 : Using the ?**

  ```
  echo color > test.txt
  echo colour >> test.txt
  ```
  
  ```
  grep -E 'colou?r' test.txt
  ```


  `24:27`
- #### How to search for a complete word ?
  **Exercise 3 : Using the -w**

  ```
  grep -w 'root' /etc/passwd
  ```


  `27:34`
- #### Searching with case sensitive

  ```
  grep -wi root /etc/passwd
  ```

  `29:35`
- #### Printing the lines 5 lines before and after and both after getting the match
  
  ```
  grep -w root -A5 /etc/passwd
  grep -w root -B5 /etc/passwd
  grep -w root -C5 /etc/passwd
  ```

  `31:33`
  
- #### Dealing with number

	- Searching for ports  with minimum 5 digits
		```grep -E [0-9]{5,} /etc/services```
		
	- Searching for port with only 3 digits
		```grep -E [0-9]{3,3} /etc/services```
		

- #### White Spaces

  ```
  grep -E "\s*" filename.txt
  ```

  \s* will search for matches with 0 or n number of white spaces !!

