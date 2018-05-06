# Linux-Tips

### R and Rstudio
sudo sh -c 'echo "deb http://cran.rstudio.com/bin/linux/ubuntu trusty/" >> /etc/apt/sources.list'  
gpg --keyserver keyserver.ubuntu.com --recv-key E084DAB9  
gpg -a --export E084DAB9 | sudo apt-key add -  
sudo apt-get update   
sudo apt-get upgrade  
sudo apt-get install r-base


sudo wget http://download1.rstudio.org/rstudio-1.1.447-amd64.deb  
sudo apt-get install gdebi-core  
sudo apt-get install libapparmor1  
sudo gdebi rstudio-1.1.447-amd64.deb  
rm *.deb

### Update the Ubuntu system from the version 14.04 to 16.04
[https://www.sysgeek.cn/upgrade-ubuntu-16-04-lts/](https://www.sysgeek.cn/upgrade-ubuntu-16-04-lts/)

### install cario
sudo apt-get install libcairo2-dev  
sudo apt-get install libxt-dev  

### install devtools
sudo apt-get install gfortran  
sudo apt-get install build-essential  
sudo apt-get install libxt-dev  
sudo apt-get install libcurl4-openssl-dev  
sudo apt-get install libxml++2.6-dev  
sudo apt-get install libssl-dev  
sudo apt-get install libfreetype6-dev  

R console: install.packages("devtools")


### Terminal
sudo apt-get install nautilus-open-terminal  


### Install Jabref
sudo add-apt-repository ppa:ari-tczew/jabref  
sudo apt-get update  
sudo apt-get install jabref  


