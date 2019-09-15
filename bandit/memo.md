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
./bandit20-do cat /etc/bandit_pass/bandit20
```
## level20
ssh bandit20@bandit.labs.overthewire.org -p 2220  
GbKksEFF4yrVs6il55v6gwY5aVje5f0j  
```
echo 'GbKksEFF4yrVs6il55v6gwY5aVje5f0j' | nc -l -p 25002 &
./suconnect 25002
```
## level21
ssh bandit21@bandit.labs.overthewire.org -p 2220  
gE269g2h3mw3pwgrj0Ha9Uoqen1c9DGr  
```
cd /etc/cron.d/
ls
cat cronjob_bandit22
cat /usr/bin/cronjob_bandit22.sh
cat /tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv
```
## level22
ssh bandit22@bandit.labs.overthewire.org -p 2220  
Yk7owGAcWjwMVRwrTesJEwB7WVOiILLI  
```
cd /etc/cron.d/
ls
cat cronjob_bandit23
cat /usr/bin/cronjob_bandit23.sh
file=$(echo I am user bandit23 | md5sum | cut -d ' ' -f 1)
cat /tmp/$file
```
## level23
ssh bandit23@bandit.labs.overthewire.org -p 2220  
jc1udXuA1tiHqjIsL8yaapX5XIAI6i0n  
```
cd /etc/cron.d/
ls
cat cronjob_bandit24
cat /usr/bin/cronjob_bandit24.sh
echo 'cat /etc/bandit_pass/bandit24 > /tmp/bandit24/pass' > cat_pass.sh; chmod 777 cat_pass.sh
# wait a minute...
cat /tmp/bandit24/pass
```
## level24
ssh bandit24@bandit.labs.overthewire.org -p 2220  
UoMYTrfrBFHyQXmg6gzctqAwOmw1IohZ  
```
cd /tmp/bandit24
echo '#!/bin/bash' > brute_pin.sh
echo 'for i in {0000..9999}; do echo "UoMYTrfrBFHyQXmg6gzctqAwOmw1IohZ $i"; done | nc 127.0.0.1 30002' >> brute_pin.sh
chmod 777 brute_pin.sh
./brute_pin.sh | grep pass 
```
## level25
ssh bandit25@bandit.labs.overthewire.org -p 2220  
uNG9O58gUE7snukf3bvZ0rxhtnjzSGzG  
```
cat /etc/passwd | grep bandit26
cat /usr/bin/showtext
```
**Change terminal to 5 lines**  
```
v
e: /etc/bandit_pass/bandit26
```
## level26
**Change terminal to 5 lines**   
ssh bandit26@bandit.labs.overthewire.org -p 2220  
5czgV9L3Xx8JPOyRbXh6lQbmIOWvPT6Z  
```
v
:set shell=/bin/bash
:shell
./bandit27-do cat /etc/bandit_pass/bandit27
```
## level27
ssh bandit27@bandit.labs.overthewire.org -p 2220  
3ba3118a22e93127a4ed485be72ef5ea  
```
mkdir /tmp/bandit27/tmp27; cd $_
git clone ssh://bandit27-git@localhost/home/bandit27-git/repo
yes
3ba3118a22e93127a4ed485be72ef5ea
cat /repo/README
```
## level28
ssh bandit28@bandit.labs.overthewire.org -p 2220  
0ef186ac70e04ea33b4c1853d2526fa2  
```
mkdir /tmp/bandit28/tmp28; cd $_
git clone ssh://bandit28-git@localhost/home/bandit28-git/repo
yes
0ef186ac70e04ea33b4c1853d2526fa2
git log
git reset --hard 186a1038cc54d1358d42d468cdc8e3cc28a93fcb
cat README.md
```
## level29
ssh bandit29@bandit.labs.overthewire.org -p 2220  
bbc96594b4e001778eee9975372716b2  
```
mkdir /tmp/bandit29/tmp29; cd $_
git clone ssh://bandit29-git@localhost/home/bandit29-git/repo
yes
bbc96594b4e001778eee9975372716b2
git branch -a
git checkout remotes/origin/dev
cat README.md
```
## level30
ssh bandit30@bandit.labs.overthewire.org -p 2220   
5b90576bedb2cc04c86a9e924ce42faf  
```
mkdir /tmp/bandit30/tmp30; cd $_
git clone ssh://bandit30-git@localhost/home/bandit30-git/repo
yes
5b90576bedb2cc04c86a9e924ce42faf
cd repo
cat .git/packed-refs
git show --name-only secret
``` 
## level31
ssh bandit31@bandit.labs.overthewire.org -p 2220  
47e603bb428404d265f59c42920d81e5  
```
mkdir /tmp/bandit31/tmp31; cd $_
git clone ssh://bandit31-git@localhost/home/bandit31-git/repo
yes
47e603bb428404d265f59c42920d81e5
cd repo
cat README.md
echo 'May I come in?' > key.txt
rm .gitignore
git add key.txt
git commit -m add
git push origin master
yes
47e603bb428404d265f59c42920d81e5
```
## level32
ssh bandit32@bandit.labs.overthewire.org -p 2220  
56a9bf19c63d650ce78e6ec0354ee45e  
```
$0
cat /etc/bandit_pass/bandit33
```
## level33
ssh bandit33@bandit.labs.overthewire.org -p 2220  
c9c3199ddf4121b10cf581a98d51caee  
```
```
