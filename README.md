# 电子科技大学电信宽带自动登录

源自 ![LambdaYH/UESTC-SRUN](https://github.com/LambdaYH/UESTC-SRUN)

主要改进：可以不需要python环境，导出为exe直接执行，更新webDriver为版本87

## 目录结构
- auto_login.py     python源代码
- config.ini        配置文件，用于修改用户名，密码等
- webdriver         Chrome的web驱动，执行过程中需要调用

## 使用方法
注意！在使用之前，需要更改config.ini来输入你对应的学号和密码，如果认证服务器地址有更新，也需要进行修改
### 使用可执行文件直接使用
请直接移步Release
![Windows x64](https://github.com/wmdscjhdpy/SRUN_AutoConnect_UESTC/releases/)
Linux 等待打包中

### python环境配置使用
需求的包：selenium,configparser,requests,   如果需要自己重新打包二进制文件需要pyinstaller
如果缺少对应的包可以使用```pip install PackYouNeed```来进行安装
可以直接执行auto_login.py
打包指令```pyinstaller -F .\auto_login.py```