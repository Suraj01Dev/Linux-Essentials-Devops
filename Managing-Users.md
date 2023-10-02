# Managing Users
```timestamp-url 
 https://www.youtube.com/watch?v=19WOD84JFxA
 ```

- #### Understanding Users in Linux

- How to actually check the users present ?
     - ``cat /etc/passwd``

- #### How to add a user ?

  ```
  sudo useradd <username>
  ```

  `User Id used by humans for interactive purposes are given user-id above 1000, and user-id below 1000 are system used by system accounts.`

- #### How to remove/ delete a user ?

  ```
  sudo userdel <username>
  ```


- #### Creating a home directory along with user creation

  ```
  sudo useradd -m <username>
  ```


- #### Removing the user with the home directory

  ```
  sudo userdel -r <username>
  ```

- #### How to add a password?

  ```
  sudo passwd <username>
  ```

- #### How to create a sys user?

  ```
  sudo useradd -r <username>
  ```


- #### How to change the default user shell?
  ```https://serverfault.com/questions/99787/tab-autocomplete-for-new-user```

  ```
  chsh -s /bin/bash <username>
   ```
