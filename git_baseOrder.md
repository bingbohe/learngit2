
## git 基本命令
* 链接origin11
   [教程地址](https://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000/001374385852170d9c7adf13c30429b9660d0eb689dd43a000)</br>
#### 基本使用
  * 创建版本库 `git init`
  * 把文件添加进入版本库</br>
  1.`git add 文件名`</br>
  2.`git commit -m "注释"`</br>
  * 把文件上传至远程库</br>
  1.`git pull origin -u master`</br>
  2.`git push -u origin master`</br>
  * 将远程库中的项目复制到本地</br>
  `https://github.com/用户名/远程库名.git`
  * 检查版本库状态 `git status`</br>
  * 检查修改内容 `git diff 文件名`
  * 检查历史版本 </br>
  1.详细显示`git log`</br>
  2.简略显示`git log --pretty=oneline`</br>
  3.指针移动日志 `git reflog`
  * 显示指针位置</br>
  1.显示当前位置`git reset --hard HEAD`</br>
  2.版本前移X位`git reset --hard HEAD~X`</br>
  3.移动到特定版本`git reset --hard 版本id`
  * 撤销修改和删除（只能撤销 未add的文件） `git checkout --文件名`
  * 撤销已add的文件 `git reset HEAD 文件名`
  * 删除文件 </br>
  1.`rm 文件`</br>
  2.`git add 被删除文件名`</br>
  3.`git commit -m "注释"`

#### 配置
  * 客户端与远程库建立链接</br>
  1.建立SSH `ssh-keygen -t rsa -C "你的绑定github的邮箱"`（id_rsa.pub记录公钥）</br>
  2.管理远程库 `git remote add origin  https://github.com/用户名/远程库名.git`</br>
  3.在本地备份远程库 `git pull origin -u master`</br>
  4.推送本地数据到远程库 `git push -u origin master (git push origi
  * 克隆远程库`git clone https://github.com/用户名/远程库名.git`
