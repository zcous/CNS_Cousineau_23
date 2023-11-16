# 1/c Zoe Cousineau - CNS - HW8 - 16Nov2023

## Research a Tool


## Demonstrate the Tool

I will be using gobuster, which can help hack into websites and get into directories on websites that you shouldn't usually see. First, I needed to install go buster using the command 
!(gobuster)
and it's installed!

The next command I used was:
!(gobuster dir -u http://testphp.vulweb.com -w /usr/share/wordlists/dirbuster/directory-list-2.3-medium.txt -x .php,.txt)

gobuster: to call the tool
U: denotes that you want to scan a URL that will follow
testphp.vulweb.com: the URL we want to scan, it is a website set up that we know is vulnerable
-w: denotes that we will be using a word list that will follow
/user/share/wordlists... : the word list we will use, this is pre-installed on kali linux. There are multiple in this folder to choose from! There is small and large as well. 
-x: extensions that we want to use
.php,.txt: the type of file extensions you want to look for

After running that, the program tool FOREVER to run, about 30 minutes (I may have watched the full charlie Brown Thanksgiving before it finished)
