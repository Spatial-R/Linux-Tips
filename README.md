# Linux-Tips

####source

(https://blog.csdn.net/xiangxianghehe/article/details/80112149)[https://blog.csdn.net/xiangxianghehe/article/details/80112149]


### R and Rstudio
sudo sh -c 'echo "deb https://mirrors.tuna.tsinghua.edu.cn/CRAN/bin/linux/ubuntu trusty/" >> /etc/apt/sources.list'  
gpg --keyserver keyserver.ubuntu.com --recv-key E084DAB9  
gpg -a --export E084DAB9 | sudo apt-key add -  
sudo apt-get update   
sudo apt-get upgrade  
sudo apt-get install r-base
[https://www.digitalocean.com/community/tutorials/how-to-install-r-on-ubuntu-18-04-quickstart](https://www.digitalocean.com/community/tutorials/how-to-install-r-on-ubuntu-18-04-quickstart)   

#### Install R package
[https://www.r-bloggers.com/installing-r-packages/](https://www.r-bloggers.com/installing-r-packages/)
[http://hoyoung.net/2015/12/06/R%E8%BD%AF%E4%BB%B6linux%E7%8E%AF%E5%A2%83%E4%B8%8B%E8%AE%BE%E7%BD%AEcran%E5%9B%BD%E5%86%85%E9%95%9C%E5%83%8F/](http://hoyoung.net/2015/12/06/R%E8%BD%AF%E4%BB%B6linux%E7%8E%AF%E5%A2%83%E4%B8%8B%E8%AE%BE%E7%BD%AEcran%E5%9B%BD%E5%86%85%E9%95%9C%E5%83%8F/)

sudo wget http://download1.rstudio.org/rstudio-1.1.447-amd64.deb  
sudo apt-get install gdebi-core  
sudo apt-get install libapparmor1  
sudo gdebi rstudio-1.1.447-amd64.deb  
rm *.deb   
[https://askubuntu.com/questions/864260/issue-with-dependency-of-r-studio-installation-in-ubuntu-16-10](https://askubuntu.com/questions/864260/issue-with-dependency-of-r-studio-installation-in-ubuntu-16-10)

sudo apt install r-base-core


### Update the Ubuntu system from the version 14.04 to 16.04
[https://www.sysgeek.cn/upgrade-ubuntu-16-04-lts/](https://www.sysgeek.cn/upgrade-ubuntu-16-04-lts/)  
[https://www.digitalocean.com/community/tutorials/how-to-upgrade-to-ubuntu-16-04-lts](https://www.digitalocean.com/community/tutorials/how-to-upgrade-to-ubuntu-16-04-lts)
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
sudo apt-get update  
sudo apt-get install nautilus  

### Sougou
[https://blog.csdn.net/qq_21792169/article/details/53152700]（https://blog.csdn.net/qq_21792169/article/details/53152700）

### cairo-dock
sudo apt-get install cairo-dock

### MPV
sudo add-apt-repository ppa:mc3man/mpv-tests  
sudo apt update && sudo apt install mpv

### POMP package
sudo apt-get install r-cran-nloptr 

### Install Jabref
sudo add-apt-repository ppa:ari-tczew/jabref  
sudo apt-get update  
sudo apt-get install jabref  

### Install WPS
sudo apt-get remove libreoffice

cd && wget -O wps-office.deb http://kdl1.cache.wps.com/ksodl/download/linux/a21//wps-office_10.1.0.5707~a21_amd64.deb  
sudo dpkg -i wps-office.deb  
sudo apt-get -f install && rm wps-office.deb  
wget -O web-office-fonts.deb http://kdl.cc.ksosoft.com/wps-community/download/fonts/wps-office-fonts_1.0_all.deb  
sudo dpkg -i web-office-fonts.deb  

## rJava

[https://askubuntu.com/questions/858961/install-rjava-on-ubuntu-failed](https://askubuntu.com/questions/858961/install-rjava-on-ubuntu-failed)

 sudo R CMD javareconf \ JAVA_HOME=${JAVA_HOME} \ JAVA=${JAVA_HOME}/bin/java \ JAVAC=${JAVA_HOME}/bin/javac \ JAVAH=${JAVA_HOME}/bin/javah \ JAR=${JAVA_HOME}/bin/jar \ JAVA_LD_LIBRARY_PATH=${JAVA_HOME}/jre/lib/amd64 \ JAVA_CPPFLAGS="-I${JAVA_HOME}/include -I${JAVA_HOME}/include/linux"

