## Lets install Jenkins and its dependencies in a new VM for controlling our first vm.

#### we need openjdk for this jenkins takes care of it.
```bash
sudo curl --fail --silent --show-error --location https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key --output /usr/share/keyrings/jenkins-keyring.asc
echo "deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc]" https://pkg.jenkins.io/debian-stable binary/ | sudo tee /etc/apt/sources.list.d/jenkins.list > /dev/null
sudo apt update 
sudo apt install fontconfig openjdk-17-jre -y
java -version

sudo apt install net-tools jenkins -y

sudo systemctl enable --now jenkins
sudo systemctl restart jenkins
sudo systemctl status jenkins

# check if jenkins is accessible from port 8080
sudo netstat -tulpn

```


![](img/jenkins001.png)
<hr>
 
![](img/jenkins002.png)
<hr>
 
![](img/jenkins003.png)
<hr>
 
![](img/jenkins004.png)
<hr>
 
![](img/jenkins005.png)
<hr>

#### Visit the Jenkins webpage from `vm_ip:8080` in a browser and configure the jenkins setup from this  
If asks for a password run in your vm 
`sudo cat /var/lib/jenkins/secrets/initialAdminPassword`

![](img/jenkins006.png)
<hr>
 
![](img/jenkins007.png)
<hr>

![](img/jenkins008.png)
<hr>
 
![](img/jenkins009.png)
<hr>
 
![](img/jenkins010.png)
<hr>
 
![](img/jenkins011.png)
<hr>
 
![](img/jenkins012.png)
<hr>
 
![](img/jenkins013.png)
<hr>
 
![](img/jenkins014.png)
<hr>
 
![](img/jenkins015.png)
<hr>
