
使用说明        
1. 在home文件夹下创建.vim .vim/bundle，修改权限

rick@ubuntu:~$sudo mkdir -p .vim/bundle
rick@ubuntu:~$ ls -al .vim
total 12
drwxr-xr-x  3 root root 4096 7月  29 16:41 .
drwxr-xr-x 22 rick rick 4096 7月  29 16:41 ..
drwxr-xr-x  2 root root 4096 7月  29 16:41 bundle

rick@ubuntu:~$ sudo chmod 777 .vim -R
rick@ubuntu:~$ ls -al .vim
total 12
drwxrwxrwx  3 root root 4096 7月  29 16:41 .
drwxr-xr-x 22 rick rick 4096 7月  29 16:41 ..
drwxrwxrwx  2 root root 4096 7月  29 16:41 bundle

2. vundle 会接管 .vim/ 下的所有原生目录，所以先清空该目录，再通过如下命令安装 vundle：
rick@ubuntu:~$ git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim

rick@ubuntu:~$ ls -al .vim/bundle/
total 12
drwxrwxrwx 3 root root 4096 7月  29 16:45 .
drwxrwxrwx 3 root root 4096 7月  29 16:41 ..
drwxrwxr-x 8 rick rick 4096 7月  29 16:45 Vundle.vim

3. 配置文件     
  将.vimrc文件复制到home文件夹下
  rick@ubuntu:~/work/vim$ cp .vimrc ../..

4. 更新，安装插件
安装插件,vim打开任意文件，执行以下命令
:PluginUpdate
:PluginInstall

相关git操作
git clone https://github.com/iluzhiyong/vim.git
git add .vimrc .vim -A
git commit -m "init"
git push -u origin master

