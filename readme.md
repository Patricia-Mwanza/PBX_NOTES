# Creating extensions on PBXs and calling each other using the extension created
### Dependencies 
- Zoiper 
### Log into the PBX with user credentials if you don’t have any account, one has to be created. 
- If you have a pbx account log in to the pbx and create extensions
### Create  extensions.
- Click applications once done a drop down menu will appear . go to extensions and click.
- Click on quik create extensions and enter the details required like the following;Display name,Caller id. Then click on next and finish.  Create Two extensions so that they can be used for establishing the connection.
### Testing the extension by calling each other using the same extensions created
- Downloaded zoiper and registered the extensions on zoiper with credentials such as user name, password and domain.
- After that was done , we called the extension created and they rang without audio.
### To enable audio after the calls were made.
- To enable audio, we created the sip-trunk which was used to establish communication between the two PBXs. 
- After creating the  trunk we got the trunk's credentials and used it in the second pbx as the second PBXs sip-trunk.
- Then created the inbound and outbound routes for making the calls between the pbxs using the registered extensions. Additional information includes the following; trunk name, dial pattern and the inbound route.
- Clicked on ```settings``` > ```asterisk sip settings``` ,then click on ```detect network settings under NAT settings``` then click ```submit``` and ```apply config```.
- Then click ```admin``` >```asterisk CLI```and a form appeared where we ```entered core restart now``` as a command and clicked on the ```send``` button. Wait for 10-20 minutes for it to execute the command and refresh the page.
- Then we did a test call and the audio worked.

