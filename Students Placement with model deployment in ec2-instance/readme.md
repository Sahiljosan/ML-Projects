## Students_Placement model deployment in EC2 Instance 

![image](https://user-images.githubusercontent.com/106590141/209423899-288a11d4-708a-4a30-8290-a68a5faf9879.png)

### <img src="https://user-images.githubusercontent.com/106590141/209423660-f87be18d-f5d3-43e0-8005-8f661c0e23cb.png" alt="drawing" width="20"/> Steps ML Model Deployment


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

Reference Video-[campusX](https://youtu.be/_rwNTY5Mn40)<br>
[DATASET](https://github.com/Sahiljosan/ML-Projects/blob/main/Students%20Placement%20with%20model%20deployment%20in%20ec2-instance/students_placement.csv)

### :desktop_computer: Command to be written in putty

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
