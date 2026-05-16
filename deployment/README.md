# To deploy the app
- We push the repository on our github
- Create a virtual machine on Azure with the required specs to run the webapp
![VM Deployment ](/deployment/screenshots/vm_deployment.png)
![VM Deployment ](/deployment/screenshots/vm_deployment2.png)
- Save the ssh file or PEM 
- SSH into the site using the public key IP, if using linux, chmod the PEM so that you can SSH into it, we get the public ip and the user
[ssh -i \<pem file> \<vm username>@\<public ip>]
- Then we git clone the app
- CD into the app
- Create a virtual environment using python
- pip install -r requirements.txt to install the necessary libraries
- We run the app using [flet run main.py --web --host 0.0.0.0 --port 8080]
- We got to the network settings and add a inbound rule of 8080
- Then we can access the website by seaching \<public ip>:\<port>


# Done