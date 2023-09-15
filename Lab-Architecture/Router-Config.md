# Configuring our router 

Let's start off with configuring our router. This will be vitale in ensuring we are able to run our virtual network to begin with. I do have 3 interfaces, and thanks to this diagram from Michael Taggart, you can get an idea
of what my network design will look like when we're done. I utilized the document listed in my [read me file](README.md) to help configure this network. 

![image](https://github.com/96Hydra/DevOps-Lab/assets/97918012/0a25d247-b795-4f3b-bad6-05eddf29fbae)


After you wrestle through some prompts, you should be presented with your 3 interfaces in a similar fashion as below:
![Router Config](https://github.com/96Hydra/DevOps-Lab/assets/97918012/10611543-8f5c-4a37-8087-13ab7eb746ec)

You will also have a sign in screen that is asking you to sign in. We will use 'root' for the username and the super secure password of 'opnsense' to continue our static IP set up.

Once you are signed in, you will be met with a screen that looks similar to this: 

![image](https://github.com/96Hydra/DevOps-Lab/assets/97918012/ed09c2a3-0219-4e7d-8f70-e3ba426c0c1b)

We are going to use option 1 to configure our interfaces as follows. I decided to stick with the configuration presented within the documentation, just so it was easier for me to follow, but feel free to use what works best with you.

![image](https://github.com/96Hydra/DevOps-Lab/assets/97918012/6b0a7cf1-eca1-4cf9-8e06-4d49aa00c9d9)


We're going to ensure IPv6 is disabled, but _do_ ensure DHCP is selected. 

For the malware lab/lab where we want things isolated, I would start with a new schema, either 172.x.x.x, or 10.x.x.x to ensure you do not get confused with the infastructure side. 

Once this is complete, we're ready to get to the next screen. 


# OPNSense Installer

Once you wrap up your config of your IP addresses, you can sign out by pressing '0' and then signing into the 'installer' user utilizing the same 'opnsense' password. Very secure.

![image](https://github.com/96Hydra/DevOps-Lab/assets/97918012/268857b0-9555-42e4-a096-d589a8635505)

We're going to stick with the default install and ignore any memory/storage warnings.

![image](https://github.com/96Hydra/DevOps-Lab/assets/97918012/5be552f5-f054-4064-9c9a-b1feb650f097)

Ensure you have hard disk selected for your installation: 

![image](https://github.com/96Hydra/DevOps-Lab/assets/97918012/d5c06c1c-7734-4e4f-a3f3-97a0c58f0662)

After this, just answer yes to everything and anything that comes up. Even if it means having to give up your first born. I unfortunately do not make the rules here.

While the install process is running, feel free to go grab something to snack on, a drink, etc. It may take a bit

![image](https://github.com/96Hydra/DevOps-Lab/assets/97918012/8b4cc0e0-c95a-471d-8dec-2a68e682fb47)


Before you continue, please update your root password. You do not want to leave it as the super secure password opnsense provided us.

Now that this is complete, for now, let's move on to the next part.
