A MAC Changer is a script written in python that changes the MAC address of a machine.

MAC/Physical Address of a machine is assigned by the manufacturer and it remains the same. So, in order to increase anonymity while surfing the net or carrying out some specific tasks anonymously, changing the MAC address of a machine is can be preffered.

Changing a MAC address does not only helps to become anonymous but it can also help to impersonate another machine by changing MAC to the other machine's MAC address. So, the machine with a changed MAC address similar to the other machine's can get easily authenticated by a service.

Now, this script uses three standard libraries that are subprocess, optparse and re (regular expressions).

Subprocess module helps executing system commands.
Commands depends upon the OS which executes the script.
For syntax and more usage functionality, you can visit official documentation.

https://docs.python.org/2/library/subprocess.html

Optparse allows to get arguments from the user.
It parse them and use them in our code.
For syntax and more usage functionality, you can visit official documentation.

https://docs.python.org/2/library/optparse.html

re (regular expressions) have been used in order to search for specific patterns in a string.
Here I have used it to search for the MAC address from ifconfig command output and print it and do other operations.
For syntax and more usage functionality, you can visit official documentation.

https://docs.python.org/2/library/re.html
Usage:

This will work for Linux based systems because in the code I have written "ifconfig" to get the output of the network configurations. In Windows the same is done using "ipconfig".
For Windows ifconfig must be replaced with ipconfig.
This requires python to be installed in the system.
Use python2 to run the script.
To run the script just enter:

python mac_changer.py -i [interface] -m [preffered mac address]

In place of -i and -m, --interface and --mac can also be used.
After executing the script, the MAC address will get changed according to user input.



