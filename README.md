# py-practise
## Python安装
官网下载安装Python 3.6.5，安装时选择同时安装pip

## 第三方库安装
### 自动获取安装包安装
 如果是无法访问互联网，要配置pip源地址（下面几个库优先使用这种方式安装）
 - pip install numpy
 - pip install pandas
 - pip install matplotlib
### 从内网获取
 配置C:\Users\XXX\pip\pip.ini 设置内网库地址，安装时使用：pip install numpy --trusted-host 内网地址
### 获取whl文件安装
 [[点击获取文件]](http://www.lfd.uci.edu/~gohlke/pythonlibs/)
 进入文件目录执行（下面两个库优先使用文件安装）:
 - pip install scipy-1.1.0-cp36-cp36m-win_amd64.whl
 - pip install scikit_learn-0.19.2-cp36-cp36m-win_amd64.whl 
 - 其他包 pandas‑0.23.4‑cp36‑cp36m‑win_amd64.whl numpy‑1.15.1+mkl‑cp36‑cp36m‑win_amd64.whl matplotlib‑3.0.0‑cp36‑cp36m‑win_amd64.whl
### 通过源码
  使用命令：python setup.py install
  
## Git安装配置
### 安装
 官网下载，安装过程中一路next

### 配置账户信息
 - git config --global user.name "rooftopcaller"         //GitHub用户名
 - git config --global user.email benmeimann@gmail.com   //GitHub注册邮箱

### 配置本地SSH
 ssh-keygen -t rsa -C "benmeimann@gmail.com" 一路回车，最终获取.ssh/id_rsa.pub文件中的内容
### 配置GitHub SSH
 登录GitHub，点击Settings——SSH and GPG keys——点击右侧Add SSH key，新建SSH key，将上面步骤获取内容黏贴进去，添加SSH Key

### 从GitHub下载工程
 如果无法访问互联网，要先设置代理：git config --global http.proxy http://[域账号]:[域密码]@[ProxyUrl]:[Port],若密码中带有特殊字符如"@"等，需要用"\"转义
 - 新建本地仓库：直接在文件夹上右击选择“Git Bash Here"
 - 初始化本地仓库：git init d/PythonB/Git
 - 下载GitHub工程：git clone https://github.com/rooftopcaller/py-practise.git
 
