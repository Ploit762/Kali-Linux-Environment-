# Using PhoneInfoga to Scan Phone Numbers

PhoneInfoga is an OSINT that is used to scan international phone numbers. This is a great tool to gather information on a specific phone number that you are needing to investigate in.
#
There is multiple ways to download this tool for Docker and UNIX systems, and it work well with the install. Click the link below to see the different options on installing this tool.
https://sundowndev.github.io/phoneinfoga/getting-started/install/

* I will be using Kali Linux to run this tool, you would first want to run this command in kali so it can download to Kali.
  * `bash <( curl -sSL https://raw.githubusercontent.com/sundowndev/phoneinfoga/master/support/scripts/install )`
    
* Next, you will install the tool onto Kali by running this command.
  * `sudo install ./phoneinfoga /usr/local/bin/phoneinfoga`
    
* PhoneInfoga is now installed and can be used on Kali, to check the version of the tool, run this command.
  * `./phoneinfoga version`
#
Here is how to use PhoneInfoga on Kali and also use the GUI version of the tool as well.
  * In Kali, run this command to see results of the phone numbers country, what type of line it is (landline or mobile), and Google searches that mention the phone number.
    *  `phoneinfoga scan -n (target phone number that you are wanting to search info for)`

* To get the GUI version with in a browser, you can enter this command.
  * `phoneinfoga serve -p (5000 or 8080)`
* The port by default is `5000`, but port `8080` will work as well. Once that command is running, you can then go to any browser and enter `http://localhost:(port number)`. From there you will be able to enter the phone number and get clear text results. 
