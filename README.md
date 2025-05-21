# EX 05: METASPLOIT-FOR-RECONNAISSANCE:
# Metasploit
Metasploit for reconnaissance in pentesting

## AIM:

To get introduced to Metasploit Framework and to  perform reconnaissance  in pentesting .

## DESIGN STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode

### Step 2:

Investigate on the various categories of tools as follows:

### Step 3:

Open terminal and try execute some kali linux commands

## EXECUTION STEPS AND ITS OUTPUT:

Find out the ip address of the attackers system
### OUTPUT:
![alt text](image.png)


## Invoke msfconsole
### OUTPUT:
![alt text](image1.png)


Type help or a question mark "?" to see the list of all available commands you can use inside msfconsole.
![alt text](image2.png)

## Port scanning:
### msf > nmap -sT 192.168.1810/24-p1-1000
![alt text](image3.png)

### msf > db_nmap 192.168.181.0/24
![alt text](image4.png)

### kali > ls-l
![alt text](image5.png)

### search 
![alt text](image6.png)

### info
![alt text](image7.png)

## MYSQL ENUMERATION
### db_nmap -sV -sC -p 3306 <metasploitable_ip_address>
![alt text](image8.png)

### search
![alt text](<Screenshot 2024-10-09 080509.png>)

###  use 11 Or: use auxiliary/scanner/mysql/mysql_version
![alt text](<Screenshot 2024-10-09 080520.png>)

### Use the set rhosts command to set the parameter and run the module, as follows:
![alt text](<Screenshot 2024-10-09 080536.png>)

### After scanning, you can also brute force MySQL root account via Metasploit's auxiliary(scanner/mysql/mysql_login) module.
![alt text](<Screenshot 2024-10-09 080550.png>)

### /usr/share/wordlists: set PASS_FILE /usr/share/wordlistss/rockyou.txt 
![alt text](<Screenshot 2024-10-09 080614.png>)

![alt text](<Screenshot 2024-10-09 080629.png>)

## RESULT:
The Metasploit framework for reconnaissance is  examined successfully
