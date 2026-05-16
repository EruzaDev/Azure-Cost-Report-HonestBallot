# Deployment Guide

## To Deploy the Application

- Push the repository to GitHub.
- Create a Virtual Machine in Azure with the required specifications to run the web application.

![VM Deployment](/deployment/screenshots/vm_deployment.png)
![VM Deployment](/deployment/screenshots/vm_deployment2.png)

- Save the SSH key file or PEM file.
- SSH into the virtual machine using the public IP address.  
  If using Linux, change the permissions of the PEM file before connecting.

```bash
chmod 400 <pem file>
ssh -i <pem file> <vm username>@<public ip>
```

- Clone the repository from GitHub.

```bash
git clone <repository link>
```

- Navigate into the project directory.

```bash
cd <project folder>
```

- Create a Python virtual environment.

```bash
python -m venv venv
```

- Activate the virtual environment.

```bash
source venv/bin/activate
```

- Install the required dependencies.

```bash
pip install -r requirements.txt
```

- Run the application using Flet.

```bash
flet run main.py --web --host 0.0.0.0 --port 8080
```

- Go to the Azure Network Settings and add an inbound security rule for port `8080`.
- Access the deployed application using:

```text
http://<public ip>:8080
```

# Done
