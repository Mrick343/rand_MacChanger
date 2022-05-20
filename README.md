# rand_MacChanger
A Project in which a valid Mac address generates.
In normal macchnager they gives you a ivalid MAC Address which can be detectable. But using this tool it give a valid MAC address which will not be detectable.

for example: 


![Screenshot at 2022-05-20 12-47-22](https://user-images.githubusercontent.com/85066116/169476937-17f05c04-7f3a-4afe-9a28-1061263b2146.png)


See It shown 'Unknown'.

When we use rand_MacChanger it gives us this:

![Screenshot at 2022-05-20 13-05-24](https://user-images.githubusercontent.com/85066116/169477845-c08873e4-3434-4407-bcb4-ca47f3722200.png)


A valid and Legit MAC Address.


**Installation steps:**

**Step 1:** git clone https://github.com/mdey786/rand_MacChanger.git

**Step 2:** cd rand_MacChanger/Macchanger/

**Step 3:** sudo nano sudo nano randmacgen.sh

**Step 4:** Change the Interface name in the last Line which you want and save it.

![InkedScreenshot at 2022-05-20 13-11-49_LI](https://user-images.githubusercontent.com/85066116/169480278-39e2a91f-cb50-4d76-9bfc-3713e4234625.jpg)


**Step 5:** First give permissions by **"chmod +x randmacgen.sh"** and Check if its changing MAC Address perfectly or not by running **"sudo ./randmacgen.sh"**

**Step 6:** Run **"sudo nano /etc/systemd/system/randmacgen.service"**, Once the file is created Paste the code below;

[Unit]
Description=Random MAC Address Generator

[Service]
Type=simpl
ExecStart=/bin bash **/directory of the random mac generator**

[Install]
WantedBy=multi-user.target

save this.

**Step 7:** Run **"sudo chmod 644 /etc/systemd/system/randmacgen.service"**

**Step 8:** Run **"sudo service randmacgen start"**

**Step 9:** Run **"sudo systemctl enable randmacgen"**

**Now Reboot your system**


Thank You..!
