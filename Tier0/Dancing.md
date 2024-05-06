# Dancing

## Task 0 - Setup OpenVPN
look at the Meow.md

## Task 1
**What does the 3-letter acronym SMB stand for?** \
Ans: server message block

**Explaination:** Server Message Block (SMB) is a network communication protocol used primarily by Microsoft Windows systems for sharing access to files, printers, and other resources between nodes on a network. SMB operates as an application-layer network protocol and provides the basis for networked file and print sharing services.

## Task 2
**What port does SMB use to operate at?** \
Ans: 445 (Found in nmap scan)

## Task 3
**What is the service name for port 445 that came up in our Nmap scan?** \

microsoft-ds (Found in nmap scan)

![image](https://github.com/huzaifa-jawad367/HackTheBox/assets/103884662/4f00db6e-dcc0-412e-8370-d35cf479f652)


## Task 4
**What is the 'flag' or 'switch' that we can use with the smbclient utility to 'list' the available shares on Dancing?** \
Ans: -L

## Task 5
**How many shares are there on Dancing?** \
Ans: 4

## Task 6
**What is the name of the share we are able to access in the end with a blank password?** \
Ans: WorkShares

## Task 7
**What is the command we can use within the SMB shell to download the files we find?** \
Ans: get

## Task 8
**Submit root flag** \
Ans: 
```
sudo apt install smbclient
smbclient -L 10.129.52.3
smbclient \\\\10.129.52.3\\WorkShares
```

![image](https://github.com/huzaifa-jawad367/HackTheBox/assets/103884662/beff9274-2730-49ee-acd4-6e39a4fd1db0)
![image](https://github.com/huzaifa-jawad367/HackTheBox/assets/103884662/e9499f58-f08a-48b5-80da-f4f0ad33e69c)
![image](https://github.com/huzaifa-jawad367/HackTheBox/assets/103884662/a5a25918-0c12-43e6-afa3-c8356730a432)

