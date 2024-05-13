# ZTA

Enhancing Network Security: Exploring Zero Trust Architecture with Penetration Testing and Real-Time Threat Detection


As per the ZTA we are going to check our Wazuh tool for identifying the attacks occuring in our system

So 1st we need to Open a ssh service in our targeted host, here i am use the windows 10
1. Go to settings--manage optiontal features--add new feature--ssh server install
2. Open our wazuh server from virtualbox/vmware
3. Open our web client using the wazuh server ip   (eg  https:// wazuh ip)
4. Default username and password is admin and admin 
5. Add Agent in Wazuh  ( click the add agent icon and add your correspond os agent)
6. Open kali Linux 
7. Start attack through hydra tool (our target is SSH in our windows 10)
8. hydra -L username list -P Password list target ip ssh
   -L for username list that we are created for bruteforce attack
   -P for password list that we are created for bruteforce attack
   target ip = our windows ip 

10. Open wazuh and go through the Security Events
11. We can see the alerts of our attacks is created
