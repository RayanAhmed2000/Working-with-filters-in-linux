# AWK
- file = alicebob.txt
```
Alice 23 Female Engineer
Bob 30 Male Doctor
Charlie 25 Male Lawyer
Eve 28 Female Teacher
```
- Print columns
```
cat alicebob.txt | awk '{print $1 $3}'
```
- Print colums with custom delimeter
```
cat alicebob.txt | awk -F ',' '{print $2}'
```
- Search for a pattern (works like grep)
```
cat alicebob.txt | awk '/30/'
```
- List out all the rows having age more than 25
```
cat alicebob.txt | awk '25<$2 {print $0}'
```
- Calculate and print sum of all ages
```
cat alicebob.txt | awk '{sum+=$2} END  {print "Total=", sum} '
```
