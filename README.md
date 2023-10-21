![image](https://github.com/EdwinLamarWalker/Virtual-private-network/assets/147763790/ef483fa9-49db-43ca-bc09-18a60140e5a1)



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


Now Close ( do not shut down) your vm in azure and search a vpn app of your choice on your computer, I will be using proton vpn. The reason we arent creating an account inside our vm is because of our language barrier due to our vm's region ( france i.e french.) Once finished downloading and creating an acc, Copy The link and paste it inside your Azure browser, then proceed to download and sign in through the app from there.


![image](https://github.com/EdwinLamarWalker/Virtual-private-network/assets/147763790/efe499d8-ae9b-4053-8667-a8231c576a5e)

Notice our ip address is still based in france inside the vpn, now when we connect to a vpn it connects us to a proton private network server in that area, in our case it would be japan. when that happens our ip address will change. 



![image](https://github.com/EdwinLamarWalker/Virtual-private-network/assets/147763790/3686b78e-4df3-4bf8-908c-74aa902d8e0e)

Durring this process its building us a tunnel into a japanese server, If your connection to your vpn falters (which it will) thats normal it should comeback online shortly.


![image](https://github.com/EdwinLamarWalker/Virtual-private-network/assets/147763790/59318491-1fba-4645-864b-cf90f6f4dbf4)


We've installed a vpn and connected it into a server in japan. Now all of Our browsing traffic in the vpn, instead of where its been going, will be routed through our vpn servers, making it look as though we are in japan.


![image](https://github.com/EdwinLamarWalker/Virtual-private-network/assets/147763790/7d4141f7-5a60-4175-a837-d06069d5815b)

![image](https://github.com/EdwinLamarWalker/Virtual-private-network/assets/147763790/9c43dd47-ef65-48bf-8442-2d98dd831529)


To Verify, refresh your ip address site we looked up earlier and it should give you a tokyo, japan ip address. Additionally any website you search will be brought up in japanese format, and that is creating and observing vpn's in microsoft azure.


