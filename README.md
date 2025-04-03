#  NapCat-Mac-Installer

NapCat on macOS
##安装NapCat&连接trss崽
1、trss崽安装教程，请看云崽的安装说明，可安装miao崽后，在根目录运行下方指令切换
'''sh
node trss
'''

2、安装NTQQ；

3、在release下载NapCat的压缩包，解压后安装；

4、按照提示点击相应按钮，跳到对应路径备份qq配置文件，然后点击另一个按钮跳到NapCat配置文件的路径，复制文件到qq配置文件路径替换qq原配置文件；

5、按照NapCat到终端提示启动NTQQ
'''sh
#终端命令
/Applications/QQ.app/Contents/MacOS/QQ --no-sandbox
'''

6、启动完成后，在日志里找到
'''sh
WebUi Local Panel Url：http：//ip：port/webui？token=napcat
'''
ps:ip:是本地ip；端口号默认是：6099 （根据实际情况会有出入，被占用的会自动+1），token是登陆页面的密码，初始密码是napcat；

7、在浏览器打开上面的连接，会提示让你设置密码，初始密码是napcat，修改后重新登陆；
'''sh
http：//ip：port/webui？token=napcat
'''

8、进入页面，在网络配置添加Websocket客户端（公网的一定要加token），并启用
![image](https://github.com/user-attachments/assets/4b9aa11a-d49b-4c35-b01e-391a52c28cac)

9、启动trss崽，即可自动识别。
