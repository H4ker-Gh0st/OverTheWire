#Bandit 
## Level Goal

The password for the next level is stored in the file **data.txt**, which is a hexdump of a file that has been repeatedly compressed. For this level it may be useful to create a directory under /tmp in which you can work. Use mkdir with a hard to guess directory name. Or better, use the command “mktemp -d”. Then copy the datafile using cp, and rename it using mv (read the manpages!)

## Commands you may need to solve this level

grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd, mkdir, cp, mv, file

## Helpful Reading Material

- [Hex dump on Wikipedia](https://en.wikipedia.org/wiki/Hex_dump)

## RASPUNSUL

mkdir /tmp/xyz
cd /tmp/xyz
cp ~/data.txt .
mv data.txt data
xxd -r data > binary
mv binary binary.gz
gunzip binary.gz
gunzip2 binary
mv binary.out binary.gz
gunzip binary.gz
tar -xf binary
rm binary data
tar -xf data5.bin
rm data5.bin
bunzip2 data6.bin
tar -xf data6.bin.out
rm data6.bin.out
mv data8.bin data8.gz
cat data 8

KEY : FO5dwFsc0cbaIiH0h8J2eUks2vdTDwAn