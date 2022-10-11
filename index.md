[editor on GitHub](https://github.com/yangsu2022/yangsu0423.github.io/edit/gh-pages/index.md)

# Notebook of Su

## Intro to oneAPI

### Concepts

-SYCL

SYCL (pronounced ‘sickle’) represents an industry standardization effort that includes support for data-parallel programming for C++. It is summarized as “C++ Single-source Heterogeneous Programming for OpenCL.” The SYCL standard, like OpenCL, is managed by the __Khronos Group__.

SYCL is a cross-platform abstraction layer that builds on OpenCL. It enables code for heterogeneous processors to be written in a “single source” style using C++. This is not only useful to the programmers, but it also gives a compiler the ability to analyze and optimize across the entire program regardless of the device on which the code is to be run.

Unlike OpenCL, SYCL includes templates and lambda functions to enable higher-level application software to be cleanly coded with optimized acceleration of kernel code. Developers program at a higher level than OpenCL but always have access to lower-level code through seamless integration with OpenCL, as well as C/C++ libraries.

-DPC++

Data Parallel C++ (DPC++) is oneAPI's implementation of SYCL compiler. It takes advantage of modern C++ productivity benefits and familiar constructs, and incorporates the SYCL* standard for data parallelism and heterogeneous programming. DPC++ is a single source language where host code and heterogeneous accelerator kernels can be mixed in same source files. A DPC++ program is invoked on the host computer and offloads the computation to an accelerator. Programmers use familiar C++ and library constructs with added functionalities like a queue for work targeting, buffer for data management, and parallel_for for parallelism to direct which parts of the computation and data should be offloaded.

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










