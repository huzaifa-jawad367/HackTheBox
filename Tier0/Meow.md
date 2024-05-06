# Meow

## Task 0 - Download and Initialise VPN

The download link is given on the website. Upon clicking that link a .ovpn file is downloaded.

![image](https://github.com/huzaifa-jawad367/HackTheBox/assets/103884662/61f5147c-8181-4f5e-b851-6e1a5915733b)

After the VPN file is downloaded we use the following command to initialize the model:

```
sudo openvpn starting_point_HuzaifaJawad367.ovpn
```

If you see the following output your VPN has been setup successfully.
We then refresh the webpage to continue to our tasks and press the `spawn machine` button.

![image](https://github.com/huzaifa-jawad367/HackTheBox/assets/103884662/9e476417-697d-465e-8a0c-a8a0950a93ee)

## Task 1
**What does the acronym VM stand for?** \
Ans: Virtual Machine

## Task 2
**What tool do we use to interact with the operating system in order to issue commands via the command line, such as the one to start our VPN connection? It's also known as a console or shell.** \
Ans: Terminal

## Task 3
**What service do we use to form our VPN connection into HTB labs?** \
Ans: OpenVPN

## Task 4
**What tool do we use to test our connection to the target with an ICMP echo request?** \
Ans: ping

## Task 5
**What is the name of the most common tool for finding open ports on a target?** \
Ans: nmap

## Tasks 6
**What service do we identify on port 23/tcp during our scans?** \
Ans: Telnet

Explaination: The telnet command is used to establish a connection with a remote host via the Telnet protocol. 

## Task 7
**What username is able to log into the target over telnet with a blank password?** \
Ans: root

# Task 8
**Submit root flag** \
Ans: 
Check for open ports at the spawned device using the nmap command: 
```
nmap -v <ip-address of spawned machine>
```
![image](https://github.com/huzaifa-jawad367/HackTheBox/assets/103884662/07f5a0ca-ac58-48ee-a350-bd37d95e3a80)

Use telnet to access the spawned machine:
```
telnet <ip-address of spawned machine>
```

it will ask for credentials. We can enter `root`. There is no need for a password if we login with root.

Enter the `ls` comand to look at the available directories. There will be a file `flag.txt` available.
Read the content of the file using the following command:
```
cat flag.txt
```

here is the result:

![image](https://github.com/huzaifa-jawad367/HackTheBox/assets/103884662/41485c15-a27f-4227-9e69-659213a6d9b7)
