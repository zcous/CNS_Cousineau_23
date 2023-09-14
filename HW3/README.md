# Homework 3 - CNS - 14Sep2023 - 1/c Zoe Cousineau

## New Linux Installation
  For this lab, I installd the Oracle Linux 8.8 disc, and my first try did not go well. It ran into some error and suddenly I got a black screen in death and couldn't control any part of the computer screen. I destroyed the machine and tried again. On the second try, everything was going well! I had the VM up and was going to open terminal... then crash. Another black screen on death. One step forward, two steps back. On the third try, the installation process took forever, but I got in and started to be dangerous. But then I wasn't connected to any sort of wifi and couldn't firgure out how to even do so. Again, deleted it and tried again for a fourth time. 

## SCC
   After downloading the SCC file from the Cyber Exchange website, it was time to put the tool to work. By using the command [vagrant upload C:\Users\cousineauz\HW3\scc-5.7.2_rhel8_x86_64\scc 5.7.2_rhel8_x86_64.tar.gz], it put the files on my VM. 
   Then, used the command  [vagrant scp :/home/vagrant/SCC C:\Users\cousineauz\HW3] to take the data from the tests. 

## Conclusion
  Once the SCC ran, my overall score was 37.2% RED, 139 failed, 97 passed controls, and 141 not checked with 5 not chcked. This VM needs a lot of help!!
