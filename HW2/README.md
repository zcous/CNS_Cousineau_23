# 1/c Zoe Cousineau - HW2 - 07Sep - CNS

## Lab Process
  Overall, this lab was the smoothest yet! I had a lot of catching up to do because I started doing the CNS
  Labs and Homeworks on the NUCs in the Capstone lab (bad idea, would never do that again). However, putting
  a little more time into doing it right paid off when coming to this lab.

  First, I copied the docker compoase file over to my new HW2 folder, this allowed me to start off with a 
  template and hit the ground running. I did not rename the file, I just put it in the new HW2 file so that I  
  did not have to rename it and give myself more hastle than needed. 

  Second, I configured the Docker File to add the attacker host, see below:
  ![Attacker Configuration in Docker File](https://github.com/zcous/CNS_Cousineau_23/blob/main/HW2/HW2_pic1.png)

  Lastly, it was time to ping. Yes, you can ping the hosts on the netwrok. Pinging is just seeing if anything has     
  connectivity. Pining is not getting into the system, rather just saying hello from the outside. You can use
  docksh into the other container. 

## 2 Containers

### Container 1 - redis
  I chose this container because I initially thought it said REGIS and I thought that was funny. 
  This container is maintained by the Docker Community and has a large GitHub respository with more information on it.
  Redis has a plethora of options, even in the initial look up of this image, their example code shows options like 
  --name, --help, --save --rm
  This container is unique because it is so well developed. This page has a lot of information on it and can do alot.
  It is also written in ANSI C, giving it some durability other container do not have. 

### Container 2 - traefik
  I chose this container because the penguin or beaver looking animal on the front was very cute!
  This container is maintained by the Traefik Project, and also has a GitHub repository with additional information.
  Traefik has --help and --providers options. This is better than the last container, but there are still limited options.
  This container is interesting because it seamlessly integrates with existing infrastructure and configures itself 
  automatically and dynamically. This is especially compelling for cadets with not a lot of time and the hope to
  do well in this class. 


## My Container of Choice: Busybox
  I chose this container because I thought the name was funny (just like all the other things I have picked so far).
  This container is maintained by the Docker Community, and has a GitHub Repo with more information on it.
  There are not many options in BusyBox, it does have a --help option, but nothing further than than. Other options
  are currently under development.
  This box is 1-5 Mb in on-disk size, making it very space efficient. It usually has less options than full GNUs,
  but it provides a good environment for small systems. It is called the "Swiss Army Knife of Embedded Linux".

  ![Busybox Container](https://github.com/zcous/CNS_Cousineau_23/blob/main/HW2/Hw2scrn5.png)
