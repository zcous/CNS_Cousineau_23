# HW 1 - CNS - 1/c Zoe Cousineau
## 31Aug 2023

### Automate Webserver Creation
  First, I made a new folder called html, then pasted the HW file given into the folder. by adding the following lines, we can configure the webserver to use shell. 
  bootstrap.sh is the name of the file in the directory. 
    _config.vm.provision :shell, path: "bootstrap.sh"_

  Then, I SSH'd into Vagrant, using the command 'vagrant ssh', so that I could confirm that the file was created during provisioning. This was done by the command:
    _wget -qO- 127.0.0.1/Homework_1.html._ 
    At first, I just typed "wget -qO- 127.0.0.1, but that did not give the output wanted. 

    !(https://github.com/zcous/CNS_Cousineau_23/blob/main/HW1/vagrantpicsHW1.png)

### Configure the Network
  After privisioning, I had to configure the network by adding the following line in my VagrantFile:
    _config.vm.network :forwarded_port, guest: 80, host: 4567_
 For these change to come into effect, then I ran "vagrant reload".

### Vagrant Privisioners
  The Vagrant Privisioner I chose was Chef Solo, continuing on the food theme from my box, bentobox. Chef Solo is a continuuation of Chef, 
  and allows you to provision the guest using Chef. Chef is an open source system integration framework that can automate tasks through
  their "cookbooks". You can also make recipies through their long list of options for how to use the provisioner. The objects in
  these cookbooks use JSON format, and are considered the node objects of paths. Additionally, the recipies use URL format to achieve 
  these cookbooks. 


  

