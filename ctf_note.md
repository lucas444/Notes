# CTF Note :

## THM Rick and morty 

- sudo nmap 10.10.10.10 -A -T 4 -v -oN scan_results

- gobuster dir -u 10.10.10.10 -x php,html,css,js,txt,pdf -w /wordlist



## Whiterose

https://eslam.io/posts/ejs-server-side-template-injection-rce/?source=post_page-----288b3019f87f--------------------------------

https://www.jasonturley.xyz/how-to-stabilize-a-reverse-shell/


sudo nmap 10.10.157.248 -A -T 4 -v

10.10.157.248


gobuster dir -u 10.10.157.248 -x php,html,css,js,txt,pdf -w /wordlist


Olivia Cortez:olivi8




PORT   STATE SERVICE VERSION
22/tcp open  ssh     OpenSSH 7.6p1 Ubuntu 4ubuntu0.7 (Ubuntu Linux; protocol 2.0)
| ssh-hostkey: 
|   2048 b9:07:96:0d:c4:b6:0c:d6:22:1a:e4:6c:8e:ac:6f:7d (RSA)
|   256 ba:ff:92:3e:0f:03:7e:da:30:ca:e3:52:8d:47:d9:6c (ECDSA)
|_  256 5d:e4:14:39:ca:06:17:47:93:53:86:de:2b:77:09:7d (ED25519)
80/tcp open  http    nginx 1.14.0 (Ubuntu)
| http-methods: 
|_  Supported Methods: GET HEAD
|_http-server-header: nginx/1.14.0 (Ubuntu)
|_http-title: Site doesn't have a title (text/html).
MAC Address: 02:2A:2B:4E:93:FD (Unknown)




ffuf -u http://cyprusbank.thm -H "Host: FUZZ.cyprusbank.thm"


ffuf -u http://cyprusbank.thm/ -w /root/cc/n0kovo_subdomains/n0kovo_subdomains_medium.txt  -H "Host: FUZZ.cyprusbank.thm" -ac



Gayle Bev: Of course! My password is 'p~]P@5!6;rs558:q'



/home/web/app/views/settings.ejs:
