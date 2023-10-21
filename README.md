![image](https://github.com/EdwinLamarWalker/Virtual-private-network/assets/147763790/d449ee6a-e7b4-4d30-8052-97dd91470024)


</p>

<h1>Azure - Vpn setup and usage</h1>
This tutorial observes Ip address differences and demonstrates how to successfully deploy a vpn in azure virtual machines.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Proctor Vpn

<h2>Operating Systems Used </h2>

- Windows 10</b> (22H2)

<h2>List of Prerequisites</h2>

- Look Up and record your ip address.
- Create a virtual machine in a different region with Azure.
- Item 3
- Item 4
- Item 5

<h2>Installation Steps</h2>

![image](https://github.com/EdwinLamarWalker/Virtual-private-network/assets/147763790/50067b13-12e2-4728-bf5a-98296758f62d)

</p>
<p>
The first thing you want to do is to look up your Ip address (whatismyipaddress.com) and jot it down in your notes (71.228.240.53, Tennessee), this will be important for later observation when using the virtual machine and vpn, so that we can view the differences when used.</p>
<br />


![image](https://github.com/EdwinLamarWalker/Virtual-private-network/assets/147763790/b6c20fd4-e29e-4996-b634-4db34aae9bd3)


<p>
Now when creating your virtual machine, you want to do 2 things differently. The first is to change your region, so that we can observe the differences.(Also be sure that the region has a language you can semi understand.) The second is to pick a size* with at least 2 vcpu's so that your virtual machine wont run slowly or lag up in the process. Then complete all the steps as normal and connect into remote desktop for your next steps.
</p>
<br />


![image](https://github.com/EdwinLamarWalker/Virtual-private-network/assets/147763790/d9f4d658-11d1-4c38-a18f-b1533dde3587)

</p>
<p>
In remote desktop look up your virtual machine's ip address (20.199.64.29, France) note it down and observe it. As you can see our ip address changed to france because of our vm's region. If you look up any site ( google, youtube) you will see it adjust to french language which is interesting even without a vpn its kind of like we have a vpn acting as our vm.
</p>
<br />

![image](https://github.com/EdwinLamarWalker/Virtual-private-network/assets/147763790/15e5adfa-2491-459c-b1d9-81d475ec28f8)

![image](https://github.com/EdwinLamarWalker/Virtual-private-network/assets/147763790/04562791-f15e-4f97-ab68-36c6c93906ad)


Now Close ( do not shut down) your vm in azure and search a vpn app of your choice on your computer, I will be using proton vpn. The reason we arent creating an account inside our vm is because of our language barrier due to our vm's region ( france i.e french.) Once finished downloading and creating an acc, Copy The link and paste it inside your Azure browser, then proceed to download and sign in from there.
