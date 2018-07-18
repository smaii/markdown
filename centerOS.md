第一步 下载
cd opt
wget https://nodejs.org/dist/v7.5.0/node-v7.5.0-linux-x64.tar.xz
第二步 解压缩文件包
xz -d node-v7.5.0-linux-x64.tar.xz
tar -xvf node-v7.5.0-linux-x64.tar
第三部  NODE 环境配置
这样可以使得在任何目录下，都可以使用/opt/node-v7.5.0-linux-x64/bin 下得node命令，
步骤如下：
a、切换到 root 用户
b、vi /etc/profile
c、在最下面加入
# node （注释作用）
export NODE_HOME=/opt/node-v7.5.0-linux-x64
export PATH=$PATH:$NODE_HOME/bin  
export NODE_PATH=$NODE_HOME/lib/node_modules
d、:wq （保存并退出）
e、source /etc/profile （使配置文件生效）


第四步 大功告成
    你就可以用 node -v 看自己的成果了！ 