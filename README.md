<h5>Directory</h5> 

<b>[Tech Portfolio Home](https://github.com/Jays1115/Jalen-Smith.git)</b>
<b>[AWS Projects](https://github.com/Jays1115/AWS-Projects.git)</b>

# Vertically-Scaling-an-EC2-Instance

<h2>Description</h2>
Scenario: A school server that runs a course scheduling solution needs more memory. 
<br><br>
Solution: Vertically scale an EC2 instance from t3.micro to m4.large to provide better application performance by increasing the instance's CPU, memory, and network capabilities, allowing it to handle a higher load, execute more processes simultaneously, and improve overall responsiveness for resource-intensive tasks. This scaling approach ensures the application can meet growing user demand without downtime or significant configuration changes.

<h2>Program walk-through:</h2>

<p align="center">
Navigated to the EC2 Section within AWS and reviewed the selected region, making sure its set to N. Virginia (us-east-1): <br/>
<img src="images/Screenshot 2024-09-16 at 6.21.58 PM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
</p>

<p align="center">
Navigate to "Instances" via the left side bar: <br/>
<img src="images/Screenshot 2024-09-16 at 6.24.55 PM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
</p>

<p align="center">
Selected the EC2 instance for the schools application & reviewed its details: <br/>
<img src="images/Screenshot 2024-09-16 at 6.25.52 PM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
</p>

<p align="center">
Navigated to "Instance Types". Searched for t3.large, c5.large, & r5.large instance types and selected them. Reviewed each instance type side by side, determining pros and cons, in the bottom panel: <br/>
<img src="images/Screenshot 2024-09-16 at 6.27.40 PM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<img src="images/Screenshot 2024-09-16 at 6.29.20 PM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
</p>

<p align="center">
Copied the IPv4 address of the EC2 instance & pasted it into a new browser tab: <br/>
<img src="images/Screenshot 2024-09-16 at 6.33.33 PM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<img src="images/Screenshot 2024-09-16 at 6.34.11 PM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
</p>

<p align="center">
Navigated back to the EC2 instance and clicked connect: <br/>
<img src="images/Screenshot 2024-09-16 at 6.36.52 PM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
</p>

<p align="center">
Connected to the EC2 instance via the session manager: <br/>
<img src="images/Screenshot 2024-09-16 at 6.40.13 PM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<img src="images/Screenshot 2024-09-16 at 6.40.22 PM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
</p>

<p align="center">
Followed these steps in the terminal:<br/>
1. Provided root privileges to the current session using the following command: <b>sudo -i</b><br/>
2. Moved into the sample_app directory using this command: <b>cd ../home/ec2-user/sample_app</b><br/>
3. Viewed the files in the sample_app directory, using this command: <b>ls</b><br/>
4. Checked the instance log, using this command: <b>tail -lf aws_compute_solutions.log</b>
<br/>
<img src="images/Screenshot 2024-09-16 at 6.44.20 PM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
</p>


<p align="center">
Navigated back through the instance section to review user data attached to this EC2 instance.
<br/>
<img src="images/Screenshot 2024-09-16 at 6.47.07 PM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<img src="images/Screenshot 2024-09-16 at 6.48.18 PM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
</p>

<p align="center">
Stopped the instance.
<br/>
<img src="images/Screenshot 2024-09-16 at 6.49.57 PM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<img src="images/Screenshot 2024-09-16 at 6.50.05 PM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<img src="images/Screenshot 2024-09-16 at 6.50.39 PM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
</p>

<p align="center">
Changed the instance type to m4.large to vertically scale this instance's capcity to perform its intended function.
<br/>
<img src="images/Screenshot 2024-09-16 at 6.54.23 PM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<img src="images/Screenshot 2024-09-16 at 6.54.49 PM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
</p>

<p align="center">
Restarted the EC2 instance.
<br/>
<img src="images/Screenshot 2024-09-16 at 6.56.12 PM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<img src="images/Screenshot 2024-09-16 at 6.56.43 PM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
</p>

<p align="center">
Now the school's student class scheduler should have enough capcity to continue running as intended!
<p/>
