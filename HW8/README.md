# 1/c Zoe Cousineau - CNS - HW8 - 16Nov2023

## Research a Tool
The tool I am researching is gobuster, a kali linux tool! Gobuster is described as a "noisy, aggressive scan that is noticed". They warn that you should only scan websites that you have permission to scan because the scan will be noticed. Gobuster is written in "Go Lnaguage" on Ubuntu 20.04. Gobuster's github page can be found here: [https://github.com/OJ/gobuster]. This github page shows the changed gobuster has had over the years and shows all the docuentation. Gobuster is able to brute force URIs on websites, DNS subdomains, Virtual hosts on web servers, open Amazon S3 buckets, Open Google cloud buckets, and TFTP servers. Gobuster was originally created in 2015, and has grown since to be up to version 3.6 today. Gobuster is perfect for capture the flag challenges because you can brute force webserve data, however, it is a slower tool to use. Wordlists are commonly used in Gobuster because it is a list of commonly used terms. They have provided multiple word lists, but you can also add your own. Wordlists include common username lists and password lists that you can brute force on a admin login website. Additionally, directory mode allows you to look for hidden files and URL paths that you would not normally see otherwise. Using the wordlists to look up common phrases and the directory mode searching, you can use gobuster to be dangerous. 

## Demonstrate the Tool

I will be using gobuster, which can help hack into websites and get into directories on websites that you shouldn't usually see. First, I needed to install go buster using the command 
(gobuster)
and it's installed!

The next command I used was:
(gobuster dir -u http://testphp.vulweb.com -w /usr/share/wordlists/dirbuster/directory-list-2.3-medium.txt -x .php,.txt)

gobuster: to call the tool
U: denotes that you want to scan a URL that will follow
testphp.vulweb.com: the URL we want to scan, it is a website set up that we know is vulnerable
-w: denotes that we will be using a word list that will follow
/user/share/wordlists... : the word list we will use, this is pre-installed on kali linux. There are multiple in this folder to choose from! There is small and large as well. 
-x: extensions that we want to use
.php,.txt: the type of file extensions you want to look for

After running that, the program tool FOREVER to run, about 30 minutes (I may have watched the full charlie Brown Thanksgiving before it finished)

![CharlieB](https://github.com/zcous/CNS_Cousineau_23/blob/main/HW8/charlieBREAL.png)
^^Me chowing down during this Thanksgiving Break

![Running](https://github.com/zcous/CNS_Cousineau_23/blob/main/HW8/HW8_run1.png)
The statuses next to each one have different meanings. Seeing statuses is good news!
- 200: it is ok, request has succeeded and we can find this
- 300: page has been redirected
- 403: Forbidden, we will still not be able to access!
Here, you can see all the directories that are now accessable and we can even see the admin section, below

![Admin](https://github.com/zcous/CNS_Cousineau_23/blob/main/HW8/HW8_indexadm.png)

Through all these directories, you can access the Admin folder and look for usernames or passwords that we could then use hydra for. Since this is an open website that is used for many cyber excersises, there was not much in these directories. However, there was an SQL database that you could download and study to see their vulnerabilities. 

## Closing
Kali Linux is a super useful tool because you can do so many different things with it! There are so many tools and resources online to really embrace your inner hactivist. Although these tools are not the strongest ever and you definetly would need more skill to hack into bigger companies, these are good tools for a beginner who is hoping to learn more. 

