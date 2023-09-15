 # What is being used? 
The most important part to any home lab is the equipment. Without the proper equipment, things may not run properly. I am not of the group that thinks you need to spend an exorbitant amount of money to have a functioning lab. 9/10 an old laptop you forgot about in your closet will get the job done. 

I am not running this on an old laptop. I do have a dedicated server I picked up off of eBay for about $200. I am running a Dell PowerEdge T320 with an Intel Xeon E5-2450 stocked with 96 GB of RAM and over 12 TB of storage. I picked up this guy after I attempted to run most of my labs from my local computer, and unfortunately it did not have the power to run what I needed it to. 

# Hypervisor Install
Since I am running this on a server and not my personal PC, I have the opportunity to run this server as a type 1 hypervisor which allows me to have access to all of it's hardware. With some different options as to what hypervisor I wanted to run, I decided to use Proxmox, which is an open-source software server for virtualization management. Unfortunately, I have already installed Proxmox on this server so I do not have any photos to walk you through this install, however, I will leave [this video](https://www.youtube.com/watch?v=6NfZ1R6jrXQ) that shows you how to make ProxMox on a bootable USB and then how to install it onto your laptop, desktop, etc. 
