# About
- The uniq command in Linux is used to remove duplicate lines from a file or input, but it only works on consecutive duplicate lines.
```
cat abc.txt
hello
hello
hi
hello
hello
how
are 
are
are
you
?
?
?
```
Now lets remove unique values
```
cat abc.txt | uniq
hello
hi
hello
how
are 
are
you
?
```





