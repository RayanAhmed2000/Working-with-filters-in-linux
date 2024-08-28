# GREP
- grep -v (search opposite)
- grep -i (ignore case)
- grep -n (also print line no in which pattern is found)
- grep -H (also print the filename in starting where the pattern is found)
```
# EXAMPLE USING THE ABOVE THREE IN COMBO
grep -Hin "the " *.txt

#OUTPUT (line no and filename is printed in the begining)
2para.txt:1:Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum
para.txt:9:As in other professional wrestling promotions, WWE shows are not true contests but entertainment-based performance theater, featuring storyline-driven, scripted, and partially choreographed matches; however, matches often include moves that can put performers at risk of injury, even death, if not performed correctly. The pre-determined aspect of professional wrestling was publicly acknowledged by WWE's then-owner Vince McMahon in 1989 in order to avoid taxes from athletic commissions. WWE markets its product as sports entertainment, acknowledging professional wrestling's roots in competitive sport and dramatic theater.
```

- grep -r (recursively search for pattern withing sub directories)
```
grep -r "rayan" /home/rayan/grep

#OUTPUT
/home/rayan/grep/hello.txt:hello this is Rayan
/home/rayan/grep/test/hello.txt:hello this is test file inside test folder and my name is Rayan
```
- grep -l (Print names of all files containing pattern in pwd)
```
grep -l "rayan" *.txt
# it print the NAMES of all .txt files in the pwd which contain "rayan"
```
- grep -L (opposite of the above : Print the files not conatining the pattern)
- grep -o (print only the matching word not the whole line)
- grep -c (count and print the number of lines having the pattern : output in numbers)
- grep -w (match pattern as whole word : this can alternatively be achieved by adding leading or trailing spaces in patterns and putting this in inverted commas)
```
grep the file1.txt #it will also match 'others' because it contains 'the' in between

grep -w the file1.txt
Alternatively
grep " the " file1.txt

```
