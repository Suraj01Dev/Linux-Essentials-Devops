# Managing Groups
```timestamp-url 
 https://www.youtube.com/watch?v=GnlgAD8-GhE
 ```



- #### Group Config File Location
      /etc/group
 
- #### Creating Groups
  ```
  sudo groupadd <groupname>
  ```

- #### Deleting a Group
  ```
  sudo groupdel <groupname>
  ```


- #### Adding a user to a group

  ```
  sudo usermod -aG <group name> <username>
  ```

- #### How to remove a user to a group
  ```
  sudo gpasswd -d <username> <groupname>
  ```
