## Welcome!

[editor on GitHub](https://github.com/yangsu2022/yangsu0423.github.io/edit/gh-pages/index.md)
## CentOS 7 编译 OpenVINO 2022.1
####脚本目录：
1.	配置CentOS 7.6的系统依赖和安装anaconda
2.	下载CMake 3.18.4
3.	devtoolset配置gcc和conda配置python环境
4.	CMake编译OpenVINO
5.	pip安装python wheel
6.	benchmark_app测试模型和提供OpenVINO的CLI
####脚本用法
#####举例

```markdown
$ git clone https://github.com/sammysun0711/openvino.git -b centos7-install-guide && cd openvino
$ ./scripts/centos_install_guide.sh -g 7 -p 8 -c ~ -m resnet-50-pytorch -b true
```

-Usage: [-g <7 or 8>] [-p <6, 7, 8 or 9>] [-c < Cmake Dir >] [-m < evaluation model >] [-b benchmark_app C++ < true or false >]

-在centos7.6这八种环境下的OpenVINO 2022.1的安装和使用测试已经通过。GCC (7.3.1, 8.3.1), Python (3.6, 3.7, 3.8, 3.9)

