安装nvm，nvm 路径默认一般为,user/xxx/Appdata/Roaming/nvm
下载node
```
nvm install 16.14.1	
nvm use 16.14.1
```
安装成功后，shell上输入`node -v` ,无法识别node指令。
解决方法：
修改nvm的环境变量。
在nvm安装下的根目录创建一个nodejs的文件夹.
打开系统环境变量
将`NVM_SYMLIK 的路径修改为你创建nodejs文件夹的位置

设置setting配置：
nvm setting默认配置为：
```
root: C:\Users\xxx\AppData\Roaming\nvm
arch: 64
proxy: none
originalpath: .
originalversion: 
node_mirror: none
npm_mirror:
```
修改为淘宝源配置后，为：
```
root: C:\Users\xxx\AppData\Roaming\nvm
arch: 64
proxy: none
originalpath: .
originalversion: 
node_mirror:npm.taobao.org/mirrors/node/
npm_mirror: 
```
当使用nvm下载node 报错指令为：
```
Could not retrieve https://nodejs.org/dist/latest/SHASUMS256.txt.
```
修改为淘宝源，（淘宝源错误同理，改为默认源)
