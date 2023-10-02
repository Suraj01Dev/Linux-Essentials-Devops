# User Account and Password Expiration

```timestamp-url 
https://www.youtube.com/watch?v=UYBPpaWUT64
 ```
 
 
- #### How to check for password expiration?
  ```
  chage -l <username>
  ```

- #### Setting expiration for users 
  ```
  chage -E <date> <username>
  ```

- #### Password expiration
  ```
  chage -M <days> <username>
  ```

- #### Remove the password expiration
  ```
  chage -M -1 <username>
  ```

- #### How to lock the user account?
  ```
  sudo passwd -l <username>
  ```

- #### How to unlock a user account?

  ```
  sudo passwd -u <username>
  ```



### Full Process
#### Creating a user with an account expiry and password expiry

  ```
  useradd suraj
  passwd suraj
  chage -E 2023-10-22 suraj
  chage -M 30 suraj
  ```

#### Removing password expiry of a user

  ```
  chage -M -1 suraj
  ```

#### How to lock a user ?
  ```
  sudo passwd -l <username>
  ```

