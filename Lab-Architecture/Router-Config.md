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
