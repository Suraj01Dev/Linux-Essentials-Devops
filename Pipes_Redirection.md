

# Pipes and Redirection

```timestamp-url 
 https://www.youtube.com/watch?v=-Z5tCri-QlI&list=PLtK75qxsQaMLZSo7KL-PmiRarU7hrpnwK&index=9
 ```


 `03:59`
 
What are channels ?
Every process run by the linux kernel has 3 channels.
- STDIN       --->   0
- STDOUT   --->   1
- STDERR    --->   2


`06:44`
How to redirect a stdout to a file ?

```
echo "log this" > log.txt
```

`07:09`
How to redirect and append stdout to a file ?

```
echo "log this" >> log.txt
```

`08:05`

How to redirect a stderr to a file ?

```
ls wrong_file_name 2> error.txt
```


