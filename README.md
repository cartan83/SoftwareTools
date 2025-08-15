OpenVPN Instructions
https://redhat.service-now.com/help?id=kb_article_view&sys_kb_id=26f368443b12ae102800053a85e45a3a
Topic
OpenVPN Client Setup on non-Windows CSB
Setup OpenVPN client for Windows
VPN Setup for Windows non-CSB

Environment(s)
Windows
OpenVPN client
Solution
Download the OpenVPN client from here
Run the downloaded file. Click Install Now when prompted
After the client is installed, click Start> OpenVPN> OpenVPN Configuration File Directory
Download the OpenVPN configuration files to a location you will remember
Note: In order to download the configuration files, you need to either have set up two-factor authentication or received a temporary token from your Manager, and you must log in to Red Hat SSO via the browser
Unzip the config file downloaded in step 4 by right-clicking it and select Extract All... > Extract
Copy the location folders that include the .ovpn files and ca certs into the OpenVPN Configuration File Directory(C:\Program Files\OpenVPN\config\)
Alternatively, configs can be placed in C:\Users\$username\OpenVPN\config\
On the Desktop, click the OpenVPN GUI icon
On the taskbar, by the system clock, a smaller icon similar to the network connection icon will open 
Right-click this icon
Hover the cursor over one of the connections listed
Click Connect
In the Username field, type your Red Hat Username
In the Password field, type your PIN+Token or the temporary token that has been sent to your Red Hat manager.
Note: If you didn't receive a temporary token or if it doesn't work, please request a new one via our emergency hotline: https://source.redhat.com/departments/it/itx/itglobalenterprisesupport/it_global_enterprise_support_wiki/global_it_support_emergency_voicemail_numbers_faq
Click OK. If successfully connected, you will see a prompt like this and the icon will be green

Additional Information
If you are having problems resolving DNS try this - https://www.petenetlive.com/KB/Article/0001402

If there are still "limited session" errors after completing the steps above and connecting to token.redhat.com follow KB0007987: Can't access token.redhat.com

If you are experiencing the multiple .ovpn file error when opening the program/failing to connect to the VPN, Go to settings -> advanced to see what directory it is reading the configuration files from. Delete files from OpenVPN Configuration File Directory and place them in the directory the application is reading from. Close then reopen the program and try connecting again.

For China users who can't access https://openvpn.net/community-downloads, you can click here to download the client.
