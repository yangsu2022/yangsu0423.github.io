## Welcome!

You can use the [editor on GitHub](https://github.com/yangsu2022/yangsu0423.github.io/edit/gh-pages/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [Basic writing and formatting syntax](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).

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

