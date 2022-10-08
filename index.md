[editor on GitHub](https://github.com/yangsu2022/yangsu0423.github.io/edit/gh-pages/index.md)

# Notebook of Su

## Intro to oneAPI

### Download and installation of oneAPI
https://www.intel.com/content/www/us/en/developer/tools/oneapi/base-toolkit-download.html?operatingsystem=linux&distributions=webdownload&options=offline

![image](https://user-images.githubusercontent.com/102195992/194697699-26833eeb-ac70-4950-b87a-0c8ef848aa63.png)

Command Line Download
```markdown
wget https://registrationcenter-download.intel.com/akdlm/irc_nas/18852/l_BaseKit_p_2022.3.0.8767_offline.sh

sudo sh ./l_BaseKit_p_2022.3.0.8767_offline.sh
```
Installation Instructions
```markdown
Step 1: From the console, locate the downloaded install file.

Step 2: Use $ sudo sh ./<installer>.sh to launch the GUI Installer as the root.

Optionally, use $ sh ./<installer>.sh to launch the GUI Installer as the current user.

Step 3: Follow the instructions in the installer.

Step 4: Explore the Get Started Guide.
```
Add GPU access
https://dgpu-docs.intel.com/installation-guides/ubuntu/ubuntu-focal-legacy.html

### Intro to oneAPI DEMO with VS-Code Extensions 
![image](https://user-images.githubusercontent.com/102195992/192468653-d40d0509-e7bf-4716-bfbc-404b09f970db.png)

### vector-add Sample
![image](https://user-images.githubusercontent.com/102195992/192469092-58f4f804-d232-4c41-9056-eb1484f23766.png)


##   OpenVINO 2022.1 CentOS 7 Installation Guide

[centos7-install-guide bash script](https://github.com/sammysun0711/openvino/blob/centos7-install-guide/scripts/centos7_install_guide.sh)

Steps：
1.	CentOS 7.6 dependencies and anaconda installation
2.	download CMake 3.18.4
3.  GCC setup via devtoolset and python env setup via conda
4.	CMake build OpenVINO
5.	pip install python wheel
6.	benchmark_app testing and OV CLI

Usage

```markdown
$ git clone https://github.com/sammysun0711/openvino.git -b centos7-install-guide && cd openvino
$ ./scripts/centos_install_guide.sh -g 7 -p 8 -c ~ -m resnet-50-pytorch -b true
```

-Usage: [-g <7 or 8>] [-p <6, 7, 8 or 9>] [-c < Cmake Dir >] [-m < evaluation model >] [-b benchmark_app C++ < true or false >]

-The installation and test of OpenVINO 2022.1 under the eight combinations of centos7.6 has passed. GCC (7.3.1, 8.3.1), Python (3.6, 3.7, 3.8, 3.9)










