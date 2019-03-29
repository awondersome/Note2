https://github.com/creationix/nvm

https://github.com/coreybutler/nvm-windows

安装前先卸载node，删除C:\Program Files\nodejs文件，删除C:\Users<user>\AppData\Roaming\npm
  
任何全局npm模块不会在各种版本间共享，不同的node版本需要重新安装module，如npm i -g @angular/cli

nvm-noinstall.zip 绿色版

nvm-setup.zip 安装版

注意，nvm安装的路径不能有中文和空格，nodejs是指定版本的生成路径

打开install.cmd，输入回车。生成settings.txt文件，root:为nvm的安装路径，path:为指定版本nodejs的路径

配置环境变量

用户变量： NVM_HOME=nvm的路径；NVM_SYMLINK=nodejs的路径

系统变量： path=%NVM_HOME%;%NVM_SYMLINK%

安装node，nvm install <version>
  
切换node，nvm use <version>
