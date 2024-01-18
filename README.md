# linuxlesson1


'''
ssh -l pi 192.168.1.70

cd dev
mkdir user2
cd user2
cp ../user1/t*.py .
cp ../user1/*.csv .

Edit script:
vi t*.py

To run script:
t*.py *.csv

t*.py *.csv |grep -v debug

Pipe to awk to print total:
t*.py *.csv | grep i_rent | awk -F, '{ print $4; tot+=$4; }END {print "Total:",tot}'
'''
