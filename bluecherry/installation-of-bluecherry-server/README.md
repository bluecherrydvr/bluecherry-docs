
title: Installation of Bluecherry server
createdAt: 2021-03-02T23:22:12.000Z
updatedAt: 2021-03-06T22:58:22.000Z
---

### Requirements



Version 3 (beta) supports Ubuntu LTS releases (Ubuntu 16.04 and Ubuntu 18.04), Debian 9 (Stretch) and Debian 10 (Buster). Support for CentOS has been removed.

##  Download instructions

###  Version 2 installation script

```curl
# Install Bluecherry on Ubuntu 18.04 LTS and Debian 9
 sudo bash -c "$(wget -O - https://dl.bluecherrydvr.com/scripts/install)"  
```
### Version 3 installation script

### 
Install Bluecherry on Ubuntu 18.04 LTS, 20.04 LTS, Debian 9 and Debian 10
Recommended for the ONVIF motion detection, sub streaming, H265 (beta) support **


```curl
# ** Bluecherry beta (3.x) **
  sudo bash -c "$(curl -s https://dl.bluecherrydvr.com/scripts/install-unstable)" 
```
### Version 3 docker image



Information and download instructions for the Version 3 docker image can be found on [GitHub](https://github.com/bluecherrydvr/bluecherry-docker)


We have a short YouTube video that shows the installation of the Bluecherry server

![](https://youtu.be/tcvlT-eGSkQ)


## mysql-server setup



Bluecherry uses mysql for storage of configuration and events.  It is highly recommended that you follow the defaults during this setup and to remember the password you set for the mysql-server.  You will need this password after the mysql-server setup and during the actually installation of the Bluecherry server

At this point the bluecherry server will be installed. If you plan to install the client on the same system, then please follow the client installation guide.



![](https://archbee-doc-uploads.s3.amazonaws.com/zEZ5kdtTvuIPeqGV--8aG/0KpVQl_yvBhcEuzhL8lV-_image.png)




![](https://bluecherry-apps.readthedocs.io/en/latest/_images/term-mysql-setup.png)
The instructions below assume you have received the [download instructions](https://app.archbee.io/docs/42ZCbo9vNLpw12_7zSpq4/yCamBxOsz-Q-B6FTClaqP#w2-installing-bluecherry-from-the-bluecherry-repository)

You will now be asked to configure Bluecherry. You must hit Yes, or the installation process will fail.

Enter the database administrative password that you set previously for the ‘root’ user.

Enter the password that you want to create for the bluecherry database. This can be the same password that you provided for the root MySQL account, but we recommend keeping the password unique. You will be asked to enter this password twice to verify the password matched.



![](https://archbee-doc-uploads.s3.amazonaws.com/zEZ5kdtTvuIPeqGV--8aG/1ipPnktSpHUI3MCp9KMGO_image.png)


