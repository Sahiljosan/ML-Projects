## Students_Placement model deployment in EC2 Instance 

<img src ="[footprints-docomo](https://user-images.githubusercontent.com/106590141/209423488-9901d030-3fb4-4968-9067-9c76cecf73db.png)" width="100" height="100" />
### Steps ML Model Deployment!

- Build the model
- Export the model using pickle/joblib
- Build a Flask website to serve the model
- Deploy the website on AWS EC2
	- Create an AWS Account
	- Create an EC2 instance
	- Edit security group
	- Download keygen(pem file)
	- Download and install Putty and WinSCP
	- Upload Flask Website to EC2 using WinSCP
	- Install packages on EC2 using Putty

WinSCP: To upload project files to server

Reference Video-[campusX](https://youtu.be/_rwNTY5Mn40)

### Command to be written in putty

```
sudo apt install python3
```

```
sudo apt-get update && sudo apt-get install python3-pip
```

```
pip3 install -r requirements.txt
```
To lock the display screen
```
screen -R deploy python3 app.py
```
