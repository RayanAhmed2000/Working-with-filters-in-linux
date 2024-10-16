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
- Now lets remove unique values
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
- notice how hello is still repeated 2 times because as told earlier only works on consecutive duplicate lines.
- so To make it useful, the input needs to be sorted or have duplicate lines grouped together.
```
sort abc.txt | uniq

?
are
are 
hello
hi
how
you
```





