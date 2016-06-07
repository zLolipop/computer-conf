# My Linux Configure (Mint 17.3)

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
 
- ## Proxychains安装
编译安装：
```bash
git clone https://github.com/rofl0r/proxychains-ng.git
cd proxychains-ng
./configure
sudo make && sudo make install
sudo cp ./src/proxychains.conf /etc/proxychains.conf
```
编辑配置：

    vim /etc/proxychains.conf
    将socks4 127.0.0.1 9095改为
    socks5 127.0.0.1 1080

使用方法：在需要代理的命令前加上 proxychains4