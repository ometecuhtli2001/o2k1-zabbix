# o2k1-zabbix
Stuff for Zabbix including templates

## TMO-G5AR template.yaml
Useful for monitoring signal of a (T-Mobile) cellular gateway. Create a host, set the IP address of the agent to 127.0.0.1 and add the template. Then set the macro {$G5AR_ADDRESS} to the IP address of the gateway.
![image](https://github.com/user-attachments/assets/5a8df42e-9e2b-4804-8264-7b794e181854)

## Enphase
If you have an Enphase solar system, you can use this template and config file to get some interesting information on status and performance. The template was developed against an Enphase X-IQ-AM1-240-4 gateway. 

Create a virtual host in Zabbix like this:
![image](https://github.com/user-attachments/assets/806f4b04-95f2-481a-bc92-8c5605717741)
Set the {$ENPHASE.HOST} and {$ENPHASE.TOKEN} values as needed. To get the token, start the Enphase app on your tablet/phone, go to Account, then My Access Control. At the bottom of the screen is a section named API Settings. Note the user ID there.  The steps beyond that are clouded in mystery....and were not written down because it was not intuitive....once I reconstruct how the API token was obtained, this will be updated!
