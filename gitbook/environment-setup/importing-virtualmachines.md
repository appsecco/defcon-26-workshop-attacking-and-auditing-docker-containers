# Importing virtual machines

* Download the virtual machines from [https://sourceforge.net/projects/defcon-26-container-security/](https://sourceforge.net/projects/defcon-26-container-security/)

## student machine (docker-student.ova)

* Open VirtualBox, and select `File` -> `Import Appliance` from the top menu

![Importing student ova](images/import-ova.png)

* Select `docker-student.ova` file from the `workshop-content` folder

![selecting student ova](images/select-student-ova.png)

* Check the "Reinitialize the MAC address of all network cards" checkbox, and click on Next to import the ova file

![student ova settings](images/student-ova-settings.png)

* Now we can see that ova file is importing

![processing](images/processing.png)

* Use following credentials for `student` VM login

```bash
username: student
password: Docker@321
```

![student vm login](images/student-vm-login.png)

* Your IP address may differ from what is visible in the screenshot. Please note down this IP address for later use

## ctf machine (docker-ctf.ova)


* Open VirtualBox, and select `File` -> `Import Appliance` from the top menu

![Importing ctf ova](images/import-ova.png)

* Select `docker-ctf.ova` file from the `workshop-content` folder

![selecting ctf ova](images/select-ctf-ova.png)

* Check the "Reinitialize the MAC address of all network cards" checkbox, and click on Next to import the ova file

![ctf ova settings](images/ctf-ova-settings.png)

* Use following credentials for `ctf` VM login

```bash
username: ctf
password: Dockerctf@321
```

![ctf vm login](images/ctf-vm-login.png)

* Your IP address may differ from what is visible in the screenshot. Please note down this IP address for later use
