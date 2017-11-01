WebIOPi-0.7.1 Patch for Raspberry B+, Pi2, and Pi3
=============================================

You have full access to all header pins (40 pins) on the Web interface.

## Usage

$ wget http://sourceforge.net/projects/webiopi/files/WebIOPi-0.7.1.tar.gz  
$ tar xvzf WebIOPi-0.7.1.tar.gz  
$ cd WebIOPi-0.7.1  
$ wget https://raw.githubusercontent.com/neuralassembly/raspi2/master/webiopi-pi2bplus.patch  
$ patch -p1 -i webiopi-pi2bplus.patch  
$ sudo ./setup.sh  
(Please answer with 'n' for the last question)  
$ wget https://raw.githubusercontent.com/neuralassembly/raspi2/master/webiopi.service  
$ sudo mv webiopi.service /etc/systemd/system/  

### How to Start WebIOPi

$ sudo service webiopi start  
$ sudo service webiopi stop  
