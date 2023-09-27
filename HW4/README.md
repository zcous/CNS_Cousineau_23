# CNS - HW4 - 1/c Zoe Cousineau - 28Sep2023

## Creating AD Users and Logging in with the User Account
First, I logged in with the IP, 172.25.1.60, and my user name zoecousineau. We had previously made the accounts last lab. The way we did this was using the cadetadm user, we added a new user with our information. In our scheme, my computer is puppy4, the naming scheme is off of our domain, SNARKYPUPPY. My username for this account is zoecousineau.

My account properties are as follows:
![My Account Properties](HW4/ZCousineauProperties.png)

You can also see all of the users we've added:
![User List](HW4/Users.png)

In the picture below, you will see that we are on the AD with our domain. 
![My Account Set Up](HW4/userHW4_1.png)

## Automated AD Administration

### Powershell Permissions
As a default, powershell had all the policies set to "Undefined". To run a shell script, these policies had to be changed. To change the policy, I used the following command and got the following output as a result:

![Policy Change](HW4/executionpolicychangeHW4.png)

The command was picked because it allows unsigned scripts to be run. None of the scripts we will write with be signed, that's kind of a hastle and a lot of work for no reason. We changed the scope of Current User because we only want to change our own computers! 


### Powershells Script Execution
Now I can finally run a powershell script with my new powers! The script I wrote was one that echos "this is hw4" (I know, very original) and shows processes that start with "wu". I originally wanted to find a process ID that was 2024 or something that started with "zo", but nothing came up. But from the screen shot below, searching "wu" output two findings. 

![Powershell Script](HW4/powershellHW4_real.png)


###Creat More AD Objects
Badblood, at first I thought we were doing something with Taylor Swift...
![Taylor Swift's Hit Single: Bad Blood](HW4/Taylor_Swift_Feat._Kendrick_Lamar_-_Bad_Blood_(Official_Single_Cover).png)

But we are actually doing something cooler, messing with our VM! Downloading Badblood was kind of scary, it kept warning us not to do it, but we went for it. The program said it was adding 2500 new users and 500 groups!! WOW!
![BadBlood working](HW4/thumbnail_image.png)

And oh my gosh did it add some users... Who is Angela Booker?! She sounds fake. Who is Adam Smith?! They couldn't have been less creative in their naming scheme. I'll give them come credit for Dwight. That was moderately original. 

The thing I find most interesting about BadBlood is it adds THOUSANDS of objects really quickly, it maybe took 7 minutes to fully run the program and start searching the platform. It's amazing how it's different every single time too! Imagine the course code for that, they must have a huge data base of random names and they just pull from that everytime. Badblood is a really cool tool to learn more abour permissions!
