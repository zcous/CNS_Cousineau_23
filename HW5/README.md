# 1/c Zoe Cousineau - HW5 - CNS - 05Oct2023

## Learning about ssh with RedHat
  Learning SSH with RedHat was actually really enjoyable! I enjoyed the layout of the lesson and the delivery of the material. To complete this lab, I SSH'd into the serverb and showed proof that I had successfully done so
  ![SSH6](https://github.com/zcous/CNS_Cousineau_23/blob/main/HW5/10.2_s6.png)
  After showing proof of logon, it was time to create the key fingerprint and show what hostname was attached
  ![SSH12](https://github.com/zcous/CNS_Cousineau_23/blob/main/HW5/10.2_step12.png)
  After, came the cool stuff, I thought it was really interesting how you could add the keys and ensure authenticity (and the Key thing looked cool). 
  ![SSH4](https://github.com/zcous/CNS_Cousineau_23/blob/main/HW5/10.4_setp4.png)
  Lastly, copying the key.
  ![SSH9](https://github.com/zcous/CNS_Cousineau_23/blob/main/HW5/10.4_step9.png)
  
## Applying Key Based Authentication
  First, I used the command ssh-keygen to make my key
  ![keygen](https://github.com/zcous/CNS_Cousineau_23/blob/main/HW5/keygen_HW5.png)
  Then, I copied my key to the cybernet jump box but searching and cat'ing the key to the host I wanted. Below is the copying and showing that I could get in!
  ![sharekey](https://github.com/zcous/CNS_Cousineau_23/blob/main/HW5/sharekey_HW5.png)
  
## Brute Force
I changed the password to killer using passwd command. I wanted to make it test, but test was too short... Honestly, I didn't get too far into this. However, I did change the password and learn about the brute force machines. 
![brute](https://github.com/zcous/CNS_Cousineau_23/blob/main/HW5/changepass_hw5.png)
I tried to install hydra on the jump box but it told me no (even with sudo) and said they'd report the issue. It really did not like sudo apt install hydra. 

But, if that had worked, I read up on how to possibly use the program. 
The command 
[hydra -L worst-passwords-2017-top100-slashdata.txt -P CousineauZ/Downloads/worst-passwords-2017-top100-slashdata.txt 10.233.103.51 ssh]
I believe would have worked. This is a dictionary attack where it tests the passwords on the users. Sad that I could not get it to work, but the research on this tool was fun and useful!


