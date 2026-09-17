# DirBuster

 This security tool is a simple yet very affective tool to use when wanting to brute-force directories and file names on a website and its server. All though there are more advance tools like GoBuster, DirBuster still holds up well and it is a great tool to use due to it being pre-installed on Kali, and a GUI to interact with easily. Going to go through how to use the tool and get the most out of it when needed.
 *<p align="center"> It is consider illegal to scan any public website without permission, I will only go through the tool and what it can provide to you. No website is being scanned or brute-forced here.   </p>*
 #
* You first want to open a terminal in Kali, and type `dirbuster`. see picture below..
   *  <img width="500" height="350" alt="Screenshot 2026-09-16 233421" src="https://github.com/user-attachments/assets/4547876c-2de7-418a-8567-157a6a4aa41d" />

* After you ran that command, you will then be prompted with a "OWASP" Window that looks like this..
  * <img width="500" height="350" alt="Screenshot 2026-09-16 234226" src="https://github.com/user-attachments/assets/bf445e9c-f006-4718-ae9d-8c6545631799" />

* Here is where you can enter the target URL of the website you are wanting to target and scan.
* The options that you see can make your scan very easy and can get you the directories and files that you are searching for.
* "Number of Threads" is the speed in which the scan will scan. Adjust this to your liking.
* You can keep the "List based brute force" checked for the list of directories that you will add.
* DirBuster does come with list of different directory name for you to scan and brute-force a website. See picture below for details...
  *   <img width="500" height="350" alt="Screenshot 2026-09-16 233623" src="https://github.com/user-attachments/assets/4bf9a11f-8af5-43d1-ad98-852a5291bca5" />
* The directory for the list provided by DirBuster is `/usr/share/dirbuster/wordlists`. From there you can pick out a list and use it to scan and brute-force the website, you can add and remove the directory names within the list as well to be more specific about directories you are wanting to find.
* DirBuster can also scan for files. In the "File extension" section you can put any file extension that coudl be found during the scan that is connected with directory names within the wordlists. "Ex: .php, .txt, .zip"
* Another option is the "Be Recursive" option, which is a option that has you find a directory, and then scan within that directory for more files or directories.
#
After you completed all the settings that fit what you need for scan, you can then push "Start". Once the scan is complete you can look within the directories that DirBuster came back with for that website, right click on them, and open them in a browser to look through them.


