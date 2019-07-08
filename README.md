
## note: Host and Jenkins share docker

### 1.Beform docker-compose up(if you has installed docker-compose in host)
```
cp /usr/local/bin/docker-compose ./
```
### 2.Get password
```
docker exec -it jenkins bash
cat /var/jenkins_home/secrets/initialAdminPassword
```
### 3.Install plugins
1. click Manager Jenkins
2. click Manage Plugins 
3. download "github integration"

## Others(Unnessary)
#### You can update Jenkins port by the following steps
```
vi /etc/sysconfig/jenkins
sudo service jenkins restart
```
