# DOCKERR INSTALLAION ON UBUNTU (LINUX):-----\



**Update the package index:**
```
sudo apt update

```


**Install necessary packages to allow apt to use a repository over HTTPS:**
```
sudo apt install apt-transport-https ca-certificates curl software-properties-common
```


**Add the Docker GPG key:**
```
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
```



**Add the Docker repository to APT sources:**
```
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"

```

**Update the package index again:**
```
sudo apt update
```


**Install Docker:**

```
sudo apt install docker-ce

```


**Verify that Docker is installed correctly by running the following command which will print Docker version:**
```
docker --version
```

**Optionally, you can also add your user to the docker group to run Docker commands without sudo (replace username with your username):**
```
sudo usermod -aG docker username
```

