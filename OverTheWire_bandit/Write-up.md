# To start with:
## What is OverTheWire ?
**OverTheWire is a wargames online website that offers some interesting challenges, the wargames offered by the OverTheWire community can help you to learn and practice security concepts in the form of fun-filled games.**





So this paragraph is from their official website
This game, like most other games, is organised in levels. You start at Level 0 and try to “beat” or “finish” it. Finishing a level results in information on how to start the next level. The pages on this website for “Level <X>” contain information on how to start level X from the previous level. E.g. The page for Level 1 has information on how to gain access from Level 0 to Level 1. All levels in this game have a page on this website, and they are all linked to from the sidemenu on the left of this page.

## Why this challenge ?
- Perfect for new linux users.
- Great to begin with.

>  **Usefull links:** ***https://overthewire.org/wargames/***

# Let's begin with the write-ups now:

- bandit0 : bandit0
- bandit1 : cmds:  ls >>>> cd

  boJ9jbbUNNfktd78OOpsqOltutMc3MY1
- bandit2 : cmds:  ls >>>> cat ./-

  CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9
- bandit3 : cmds: ls  >>>>> cat + TAB

  UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK
- bandit4 : cmds: ls >>>> cd + TAB >>>> ls -a >>>> cat .hidden

  pIwrPrtPN36QITSp3EQaw936yaFoFgAB
- bandit5 : cmds: ls >>>> file ./-file* >>>> cd file07 //because in file07 is Ascii file

  koReBOKuIDDepwhWk7jZC0RTdopnAYKh
- bandit6: cmds: find -size 1033c >>>> cat {This file}

  DXjZPULLxYr17uwoI01bNLQbtFemEgo7 
- bandit7: cmds: find -size 33c -user bandit7 -group bandit6 >>>> cat ./var/lib/dpkg/info/bandit7.password 

  HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs
- bandit8: cmds: grep millionth data.txt

  cvX2JJa4CFALtqS87jk27qwqGhBM9plV
- bandit9: cmds: sort data.txt | uniq -u

  UsvVyFSfZZWbi6wgC7dAFyFuR6jQQUhR
- bandit10: cmds: grep -a "=========" data.txt

  truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk
- bandit11: cmds: base64 -d data.txt | strings

  IFukwKGsFW8MOq3IRFqrxE1hxTNEbUPR
- bandit12: cmds: cat data.txt >>>> Then go here https://www.dcode.fr/chiffre-rot and Decode the content of data.txt

  5Te8Y4drgCRfCx8ugdwuEX8KFC6k2EUu
- bandit13: cmds: a little bit complicated but the idea is to use xxd and put it in a file at /tmp/{NameThisFileAsYouWant}
                  then use file and change the extention of the file to the one you've found while applying file
                  extract it untill you will find yourself with an ASCII text file 

  8ZjyCRiBWFYkneahHwxCv3wb2a1ORpYL
- bandit14: cmds: ssh -i sshkey.private bandit14@localhost

  4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e
- bandit15: cmds: nc localhost 30000 >>> 4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e 

  BfMYroe26WYalil77FoDi9qh59eK5xNr
- bandit16: cmds: bandit15@bandit:~$ ncat -C --ssl localhost 30001 >>> BfMYroe26WYalil77FoDi9qh59eK5xNr

  cluFn7wTiGryunymYOu4RcffSxQluehd
- bandit17: cmds: nmap -p 31000-32000 -A -v localhost
  ssh private key and create an authentification file
- bandit18: cmds: diff password.old password.new
  
  kfBf3eYk5BPBRzwjqutbbfE887SVc5Yd
- bandit19: cmds: ssh -t bandit18@localhost
  
  IueksS7Ubh8G3DCwVzrTd8rAVOwq3M5x
- bandit20: cmds: ./bandit20-do cat /etc/bandit_pass/bandit20
  
  GbKksEFF4yrVs6il55v6gwY5aVje5f0j
- bandit21: cmds: nc -l -p 1234 < /etc/bandit_pass/bandit20 THEN ./suconnect 1234
  
  gE269g2h3mw3pwgrj0Ha9Uoqen1c9DGr
- bandit22: cmds: cat /etc/cron.d/cronjob_bandit22 >>>> cd /usr/bin/ >>>> cat cronjob_bandit22.sh >>> cat /tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv
  
  Yk7owGAcWjwMVRwrTesJEwB7WVOiILLI
- bandit23: cmds: echo I am user $myname | md5sum | cut -d ' ' -f 1
  
  jc1udXuA1tiHqjIsL8yaapX5XIAI6i0n

 > \>>>> is a separation used to separate the used. 
 
 > **cmds** stands for the commands executed to find the flag.