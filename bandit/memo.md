# Bandit  

## level0  
ssh bandit0@bandit.labs.overthewire.org -p 2220  
bandit0  
```
cat readme
```

## level1  
ssh bandit1@bandit.labs.overthewire.org -p 2220  
boJ9jbbUNNfktd78OOpsqOltutMc3MY1  
```
cat < -
```
## level2 
ssh bandit2@bandit.labs.overthewire.org -p 2220  
CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9  
```
cat < "spaces in this filename"
```
## level3 
ssh bandit3@bandit.labs.overthewire.org -p 2220  
UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK  
```
cat inhere/.hidden
```
## level4 
ssh bandit4@bandit.labs.overthewire.org -p 2220  
pIwrPrtPN36QITSp3EQaw936yaFoFgAB
```
cat < -file07
```
## level5 
ssh bandit5@bandit.labs.overthewire.org -p 2220  
koReBOKuIDDepwhWk7jZC0RTdopnAYKh  
```
find /home/bandit5/inhere/ -size 1033c -exec cat {} \;
```
## level6
ssh bandit6@bandit.labs.overthewire.org -p 2220  
DXjZPULLxYr17uwoI01bNLQbtFemEgo7  
```
find / -size 33c -user bandit7 -group bandit6 -print 2> /dev/null | while read -r f; do cat $f; done
```
## level7
ssh bandit7@bandit.labs.overthewire.org -p 2220  
HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs  
```
cat data.txt | grep millionth | awk -F'\t' '{print $2}'
```
## level8
ssh bandit8@bandit.labs.overthewire.org -p 2220  
cvX2JJa4CFALtqS87jk27qwqGhBM9plV  
```
cat data.txt | sort | uniq -c | sort | tail -1 | awk -F' ' '{print $2}'
```
## level9
ssh bandit9@bandit.labs.overthewire.org -p 2220  
UsvVyFSfZZWbi6wgC7dAFyFuR6jQQUhR  
```
strings data.txt | grep -G "=" | grep -E '^=+'
```
## level10
ssh bandit10@bandit.labs.overthewire.org -p 2220  
truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk  
```
cat data.txt | base64 -d
```
## level11
ssh bandit11@bandit.labs.overthewire.org -p 2220  
IFukwKGsFW8MOq3IRFqrxE1hxTNEbUPR  
```
cat data.txt | tr A-Z N-ZA-M | tr a-z n-za-m
```
## level12
ssh bandit12@bandit.labs.overthewire.org -p 2220  
5Te8Y4drgCRfCx8ugdwuEX8KFC6k2EUu  
```
mkdir /tmp/silky
cp -p data.txt /tmp/silky/data.txt
cd /tmp/silky
xxd -r data.txt > data
file data
mv data data.gz
gzip -d data.gz
file data
bzip2 -d data
file data.out
mv data.out data.gz
gzip -d data.gz
file data
tar -xf data
ls
file data5.bin
tar -xf data5.bin
ls
file data6.bin
bzip2 -d data6.bin
ls
file data6.bin.out
tar -xf data6.bin.out
ls
file data8.bin
mv data8.bin data8.bin.gz
gzip -d data8.bin.gz
file data8.bin
cat data8.bin
```
## level13
ssh bandit13@bandit.labs.overthewire.org -p 2220  
8ZjyCRiBWFYkneahHwxCv3wb2a1ORpYL  
```
ssh -i sshkey.private bandit14@127.0.0.1
cat /etc/bandit_pass/bandit14
```
## level14
ssh bandit14@bandit.labs.overthewire.org -p 2220  
4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e  
```
echo '4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e' | netcat 127.0.0.1 30000
```
## level15
ssh bandit15@bandit.labs.overthewire.org -p 2220  
BfMYroe26WYalil77FoDi9qh59eK5xNr  
```
echo 'BfMYroe26WYalil77FoDi9qh59eK5xNr' |openssl s_client -ign_eof -connect 127.0.0.1:30001
```
## level16
ssh bandit16@bandit.labs.overthewire.org -p 2220  
cluFn7wTiGryunymYOu4RcffSxQluehd  
```
nmap 127.0.0.1 -sT -p 31000-32000
echo 'cluFn7wTiGryunymYOu4RcffSxQluehd' |openssl s_client -ign_eof -connect 127.0.0.1:31790
```
vim 17_sshkey  
chmod 600 17_sshkey  
ssh -i 17_sshkey bandit17@bandit.labs.overthewire.org -p 2220
```
cat /etc/bandit_pass/bandit17
```
## level17
ssh bandit17@bandit.labs.overthewire.org -p 2220  
xLYVMN9WE5zQ5vHacb0sZEVqbrp7nBTn  
```
diff passwords.old passwords.new
```
## level18
ssh bandit18@bandit.labs.overthewire.org -p 2220 cat readme  
kfBf3eYk5BPBRzwjqutbbfE887SVc5Yd  

## level19
ssh bandit19@bandit.labs.overthewire.org -p 2220  
IueksS7Ubh8G3DCwVzrTd8rAVOwq3M5x 
```
```
## level20
ssh bandit20@bandit.labs.overthewire.org -p 2220  

## level21
ssh bandit21@bandit.labs.overthewire.org -p 2220  

## level22
ssh bandit22@bandit.labs.overthewire.org -p 2220  

## level23
ssh bandit23@bandit.labs.overthewire.org -p 2220  

## level24
ssh bandit24@bandit.labs.overthewire.org -p 2220  

## level25
ssh bandit25@bandit.labs.overthewire.org -p 2220  

## level26
ssh bandit26@bandit.labs.overthewire.org -p 2220  

## level27
ssh bandit27@bandit.labs.overthewire.org -p 2220  

## level28
ssh bandit28@bandit.labs.overthewire.org -p 2220  

## level29
ssh bandit29@bandit.labs.overthewire.org -p 2220  

## level30
ssh bandit30@bandit.labs.overthewire.org -p 2220  
