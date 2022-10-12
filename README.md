# Lab 3 - Installing Nessus
Before attempting this lab, please complete the steps below:

 

1. Register for a personal Nessus activation code by visiting 
https://www.tenable.com/tenable-for-educationLinks to an external site.
2. Download a copy of Nessus from https://www.tenable.com/downloads/nessusLinks to an external site. ( do this from the firefox browser in kali)

Once you have the registration code and the Nessus install file has been downloaded, please proceed to the next steps

 

# Nessus Installation Lab!

1. Change directory to wherever the Nessus install file is located (Default is usually /home/kali/Downloads)
2. Type "dkpg -i ./ /Nessus-10.1.1-debian6_amd64.deb"  (Note the version number may be different than what is here)
3. Once the install is complete start the nessus service by typing the following command:
               ```sudo systemctl start nessusd```

4. Access Nessus via Firefox by going to https://localhost:8834Links to an external site.
5. Accept the self-signed certificate warning
6. Select a username, password and enter activation code (please make sure you have chosen the correct product version as well)
7. Wait while Nessus compiles all the plugins (This may take a long time to complete, and it is normal)
8. Login with the user account you previously created
9. Go to Scans -> New Scan
10. On the Scan Templates page under Vulnerabilities, choose the "Advanced Scan" type
	1. Provide a name for your scan configuration (e.g. "External Scan")
	2. Provide the target IP address (in this case, the IP address of the Metasploitable2 VM)
	3. Save the scan template
11. Press the "Play" button on the My Scans page to launch the scan you just created

Once the scanning is complete, please export the report in PDF format and submit it. To export the list of vulnerabilities, go to Report/Complete List Of Vulnerabilities by Host.
