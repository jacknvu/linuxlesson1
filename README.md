# linuxlesson1



1. ssh -l pi 192.168.1.70

2. cd dev
3. mkdir user2
4. cd user2
5. cp ../user1/t*.py .
6. cp ../user1/*.csv .

7. Edit script:
```
vi t*.py
```

9. To run script:
```
t*.py *.csv

t*.py *.csv |grep -v debug
```

10. Pipe to awk to print total:
```
t*.py *.csv | grep i_rent | awk -F, '{ print $4; tot+=$4; }END {print "Total:",tot}'
```

