
# Linux File Permissions

```timestamp-url 
 https://www.youtube.com/watch?v=4e669hSjaX8
 ```

r - **Read**

w - **Write**

x - **Execute**
  - For a file, if x is set, then it can be executed
  - For a folder, if x bit is set, you can navigate inside the directory, but if it is not set you can not navigate inside the directory.


## Using the chmod for execution 

- To make a file executable use the below command.
	- ```chmod +x new.py```
	
- The problem with this command is it adds the executable bit to user, group and the others
- To add the executable bit only to the user ``chmod u+x new.py``
- To add the executable bit only to the group ``chmod g+x new.py``
- To add the executable bit only to the other ``chmod o+x new.py``
- Similarly to remove executable permission ``chmod u-x new.py``

  **chmod can be used not only with x, but also with r and w**

    ```
    chmod g+rw new.py
    ```


## Advanced chmod

Each bit has a value associated with it.

  **r=4**
  
  **w=2**
  
  **x=1**

  Examples :
  
  1. To provide all permissions only to the file owner.

         chmod 700 script.py
  2. To provide read and write permissions to the owner and its group.
     
         chmod 660 script.py

  3. To provide all permissions to all users.
     
         chmod 777 script.py
