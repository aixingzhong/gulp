1、注册github账号，新建库
2、下载安装Git，一路next，右键点击出现git bash here选项，单击进入git命名模式
3、创建ssh key，输入命令：
$ ssh-keygen -t rsa -C 1448954782@qq.com
输入后直接按回车。表示不设置密码

4、在c盘的用户名文件中找到生成的.ssh文件夹，打开id_rsa.pub并复制里面的内容粘贴到github网站
设置选项中的new SSh key中添加，输入命令：$ ssh --T git@github.com可以看到成功地验证的提示

5.添加用户,要设置username和email
$ git config --global user.name aixingzhong
$ git config --global user.email 1448954782@qq.com

6、在本地要创建的文件夹中右击进入git bash here命令模式，初始化git，输入：
$ git init
把项目更新下来，输入：
$ git pull git@github.com:aixingzhog/gulp.git

7.修改代码提交，进入要上传的项目文件夹，添加远程地址，右键git bash输入：
$ git remote add gulp git@github.com:aixingzhong/gulp.git

8、添加所有更改文件，添加上传注释,上传文件:
$ git add .
$ git commit -m "first commit"
$ git push origin master
