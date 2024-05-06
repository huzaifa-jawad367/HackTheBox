# Fawn

## Task 0 - Setup OpenVPN
look at the Meow.md

## Task 1 
**What does the 3-letter acronym FTP stand for?** \
Ans: File Transfer Protocol

## Task 2
**Which port does the FTP service listen on usually?** \
Ans: 21

## Task 3
**What acronym is used for the secure version of FTP?** \
Ans: sftp

## Task 4
**What is the command we can use to send an ICMP echo request to test our connection to the target?** \
Ans: ping

## Task 5
**From your scans, what version is FTP running on the target?** \

run the following command to check:
```
nmap -sV 10.129.159.243
```

the output is as follows:
![image](https://github.com/huzaifa-jawad367/HackTheBox/assets/103884662/59af1387-7ae2-4fb5-b21c-0c17d95896ad)


Ans: vsftpd 3.0.3

## Task 6
**From your scans, what OS type is running on the target?** \
Ans: Unix (displayed in the above image)

## Task 7
**What is the command we need to run in order to display the 'ftp' client help menu?** \
Ans: `ftp -h`

## Task 8
**What is username that is used over FTP when you want to log in without having an account?** \
Ans: anonymous

## Task 9
**What is the response code we get for the FTP message 'Login successful'?** \
Ans: 230

## Task 10
**There are a couple of commands we can use to list the files and directories available on the FTP server. One is dir. What is the other that is a common way to list files on a Linux system.** \
Ans: `ls`

## Task 11
**What is the command used to download the file we found on the FTP server?** \
Ans: `get`

## Task 12
**Submit root flag** \
Ans:
```
ftp -v <target-ip>
```

![image](https://github.com/huzaifa-jawad367/HackTheBox/assets/103884662/c6f5881a-e6df-4510-bb74-bd5d9d63177a)

```
get flag.txt
```



