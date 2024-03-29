# Visit via hostname from another intranet device

**Example**: In computer A (HOSTNAME:computerA), I can visit my website via http://localhost:8088/. Then I need to access this website as http://computerA:8088/ via any computer in the intranet.

## Ping hostname instead of IP address
Modify your settings:
> https://superuser.com/questions/1068448/cant-access-pc-by-name-but-can-by-ip-address

To *Turn on net discovery*
> https://support.microsoft.com/en-us/help/2722035/you-cannot-turn-on-network-discovery-in-network-and-sharing-center-in

## Settings the *Windows Defender Firewall*
Open the port connection: its own website port

## Binding the hostname with the website
IIS Manager ***Bindings***

## Problems about binding IP address and Hostname 
**(use *nslookup* command to check)**
- Join the existing intranet domain
  - **Control Panel** > **System and Security** > **System**
  - *Change settings* of *WORKGROUP*/*Domain* as long as you have administrator permission

- Set up a new domain and allocate user account and password
  - Create a new domain and add another user (aside from administrator): **https://win10faq.com/create-domain-windows-server/**
  - Change this new user's permission into administrator so it can be connected remotely.
  - Change local machine's DNS settings to server's IP address.   
    **Control Panel > Network and Internet > Network and Sharing Center > *Connections* > Properties > Internet Protocol Version 4 *Properties* > *Use the Following DNS Server Address***
  - Local machine joins Domain.
  - Complete!
    

Building: https://www.businessnewsdaily.com/11019-set-up-configure-dns-on-windows-server-2016.html

Setting Server Properties: **Forwarders** & **Root Hints** (Domain name)

We can now nslookup, but it's *Non-authoritative answer*.


