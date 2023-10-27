# 1/c Zoe Cousineau - CNS - 26Oct

## Research a Vunlerable Service
My group decided that we all wanted to use a Linux based vulnerability so we could all help trouble shoot and get our exploits set up. The service I chose was Think PHP, a Chinese PHP framework that uses Apache2.
![ThinkPHPLogo](https://github.com/zcous/CNS_Cousineau_23/blob/main/HW7/OIP.jpg)
This service aims to simplify enterprise application development with MVC structure. Think PHP is currently at version 8.1. Think PHP has a big open source github directory that everyone can see and add to. I also chose this service because it is open source, allowing me to download it easily and prepare to exploit it. The tough thing about Think PHP is that it is a Chinese product, meaning all of the diagrams and information I found are in Chinese and I do not know Chinese. This diagram of their frame work has some Chinese, but is still readable. 
![Framework](https://github.com/zcous/CNS_Cousineau_23/blob/main/HW7/ThinkFrame.png)
Someone would chose Think PHP if they are a beginner learning how to use PHP. Think PHP is a little bit sketchy in my opinion. It's website ends in .cn. However, if you trust it (or are using a virtual machine that you cna destroy if anything goes wrong) this might be the tool for you. 

## Vulnerability Information
The exploit that I am using leverages Metasploit and RCE injections. The CVEs for this exploit are CVE-2018-20062 and CVE-2019-9082. The interesting thing about this exploit is that it needs Think PHP 5.0.23 or worse for this to work and to be on Linux. This vulnerability is from a remote attack that allows arbitrary PHP code to be executed, and the code is given on Exploit Database's website. It's a very long document of code, showing that using Metasploit, executing as a user they are not. Additionally, these CVEs are labeled as critical and high for severity. 
