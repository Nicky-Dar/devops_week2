# devops_week2

# devops_week2

# install ubuntu with WSL
#### Enabling WSL in Windows 10
Before you can install Ubuntu on WSL, WSL has to be enabled in one of the following ways:

Using the GUI for enabling Windows features :
1. Open the Start Menu and search Turn Windows features on or off
2. Select Windows Subsystem for Linux
3. Click OK
4. Restart your computer when prompted

#### Install your Linux distribution of choice
1. Open the Microsoft Store and select your favorite Linux distribution. 
    * Ubuntu 18.04 LTS
    * Ubuntu 20.04 LTS
    * openSUSE Leap 15.1
    * SUSE Linux Enterprise Server 12 SP5
    * SUSE Linux Enterprise Server 15 SP1
    * Kali Linux
    * Debian GNU/Linux
    * Fedora Remix for WSL
    * Pengwin
    * Pengwin Enterprise
    * Alpine WSL

        or download oprating system from
https://ubuntu.com/wsl
2. Starting Ubuntu on WSL

    The Ubuntu on WSL terminal can be started via:

    * The app tile in the Windows Start menu (or pinned to your taskbar)
    * WSL - Remote extension for Visual Studio Code.

    * The wsl command on the Windows command prompt or PowerShell

    * By running ubuntu1804.exe, etc. on the Windows command prompt or PowerShell

2. next after installation we can check for updates:

 >   sudo apt update
 
 
 ![image](https://user-images.githubusercontent.com/88620315/134180356-be5b8e30-46d3-4221-9b4d-834c3ba4f49c.png)

>   sudo apt upgrade

![image](https://user-images.githubusercontent.com/88620315/134180682-fb48730b-5100-461a-a445-7d943379f562.png)

 
# Node.js Installation & Config
1. Open your terminal
![image](https://user-images.githubusercontent.com/88620315/134169567-6a9ad8bd-189a-413e-b391-888d34619f03.png)

2. To install node.js use the following command:

    1. Download the package
> curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.38.0/install.sh | bash

![image](https://user-images.githubusercontent.com/88620315/134170175-c689fc46-b90e-497a-8602-8e89d5e08336.png)

if nvm can not found, we can input :
 
* if use Bourne Again SHell
> exec bash 

or

* if use Z shell
> exec zsh  

3. Install NVM version 13
> nvm install 13.7.0

![image](https://user-images.githubusercontent.com/88620315/134178204-568c19e0-b36f-4a7a-b55e-66eb65a7999f.png)

4. Use the nvm version 13
> nvm use 13

![image](https://user-images.githubusercontent.com/88620315/134178843-8eeab725-eeb7-4481-8698-7135b473e4a0.png)


5. Once installed, verify it by checking the installed version using the following command:

> node -v 

![image](https://user-images.githubusercontent.com/88620315/134179077-80fb2e25-e88e-4636-92cc-ca17913ee505.png)

> npm -v

![image](https://user-images.githubusercontent.com/88620315/134179245-167cc4d7-34ac-4393-ad00-b773fbe49108.png)

6. To collect all node.js files we can create a folder named myapp-nodejs. Go to the directory. 

> mkdir myapp-nodejs

> cd myapp-nodejs

7. Create a .json package file.

> npm init-y

8. Install the node.js framework. There are several node.js open source frameworks such as Express.js, Socket.io, Meteor.JS, Koa.js, and Sail.js.

    In here we use express.js package

> npm install express --save

![image](https://user-images.githubusercontent.com/88620315/134793654-ad7cbcfd-ac0d-4828-9454-fa3b12b43bec.png)

9. make and config file named index.js:

> nano index.js

![image](https://user-images.githubusercontent.com/88620315/134794688-c142761b-cdd9-46f9-a89d-96056753401f.png)

To save and overwrite index.js you can enter command ctrl+O.

To exit index.js you can enter command ctrl+X

After index.js is configured.
Next index.js can be run with the following command

> node index.js

![image](https://user-images.githubusercontent.com/88620315/134794744-51eeefc0-d71a-44f7-a4af-b485588a7897.png)

open localhost:3000 in a web browser: http://localhost:3000/

![image](https://user-images.githubusercontent.com/88620315/134794804-80c714fc-d4f4-4440-b025-eb5163a8b812.png)

# Python Installation & Config

Python installation steps, enter the following command:
1. Perform system updates:
> sudo apt update

![image](https://user-images.githubusercontent.com/88620315/134803624-d8c5dbac-1d9b-4da7-9885-9ffd6dc9d3c7.png)

2. Perform a system upgrade:
> sudo apt upgrade

![image](https://user-images.githubusercontent.com/88620315/134803667-e1c899c8-e247-4680-ae69-04dc42ea5a44.png)

3. Python already exists by default. To check the version
> python3 -v

![image](https://user-images.githubusercontent.com/88620315/134803984-0ec9ee75-dd70-4cd0-9bb0-f74863e71632.png)
.

.

.

![image](https://user-images.githubusercontent.com/88620315/134804027-5924a201-0acb-43b4-a2ec-2f70a410d770.png)

4. Install the python package manager:
> sudo apt install python3-pip

![image](https://user-images.githubusercontent.com/88620315/134804691-857c7c6b-caeb-4dfa-9fca-7b6bb6814821.png)

5. Install Python framework.
> pip install flask

![image](https://user-images.githubusercontent.com/88620315/134804927-e0a7f1b0-3c68-4b76-a61c-149a21e469bb.png)

6. To collect all python files we can create a folder named python. Go to the directory. 

> mkdir python

> cd python

7. Create and configure index.py

> nano index.py

![image](https://user-images.githubusercontent.com/88620315/134808041-b3ec66d1-9366-441f-9974-d2844e6b8cf6.png)


To save and overwrite index.py you can enter command ctrl+O.

To exit index.py you can enter command ctrl+X

After index.py is configured.
Next index.py can be run with the following command
> python3 index.py

![image](https://user-images.githubusercontent.com/88620315/134807638-9410c668-2d0e-4bcd-8a81-06fbd0bd1c37.png)

open localhost:5000 in a web browser: http://localhost:5000/

![image](https://user-images.githubusercontent.com/88620315/134808070-648dbc5d-586c-4922-b7cb-a769f70567c4.png)

# Go Installation & Config

1. Download go package:
>wget -c https://dl.google.com/go/go1.16.5.linux-amd64.tar.gz && sudo su

![image](https://user-images.githubusercontent.com/88620315/134811589-119b8f73-9fe6-446c-86d1-2514a493b79c.png)

2. extract and copy data
>rm -rf /usr/local/go && tar -C /usr/local -xfz go1.16.5.linux-amd64.tar.gz && exit



3. Enter path go in bashrc
> export PATH=$PATH:/usr/local/go/bin


4. Installation verification:
> go version

![image](https://user-images.githubusercontent.com/88620315/134811629-15211b84-f9d2-40b5-b002-1a19322b9d6b.png)

5. Collect all go files we can create a folder named myapp-golang. Go to the directory.
>mkdir myapp-golang

>cd myapp-golang

6. Create and configure index.go
> nano index.go

![image](https://user-images.githubusercontent.com/88620315/134811749-225580ca-29e4-4edd-821b-5c0ebb071a34.png)

run golang application:
>go run index.go

if you want to build:
>go build index.go

to run the already built app:
>./index.go

![image](https://user-images.githubusercontent.com/88620315/134811674-bf8d686d-c7c6-4d77-8886-d839b8c40dfd.png)

