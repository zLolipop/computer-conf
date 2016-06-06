# My Linux Configure <font size=1>Mint 17.3</font>

- ## 安装稳定版的Wireshark
 添加源并安装 
 ```bash
 sudo add-apt-repository ppa:wireshark-dev/stable
 sudo apt-get update
 sudo apt-get install wireshark
 ```
 
- ## git 安装及配置
 安装: `sudo apt-get install git`

 配置：
 
 1. 设置用户名和邮箱：
 ```bash
 git config --global user.name "用户名"
 git config --global user.emai "邮箱"
 ```
 2. 设置编辑器为vim：
 `git config git config --global core.editor "vim"`