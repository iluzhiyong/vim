使用说明
1. 在home文件夹下创建.vim .vim/bundle
sudo mkdir .vim
cd .vim
sudo mkdir bundle

2. 修改文件夹权限，保证vundle可以执行PluginInstall安装插件
sudo chmod 777 .vim -R

3. 配置文件
将.vimrc文件复制到home文件夹下

4. 更新，安装插件
安装插件,vim打开任意文件，执行以下命令
:PluginUpdate
:PluginInstall
