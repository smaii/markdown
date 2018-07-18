
//关于git 提交

// 首先要设置用户名和邮箱
git
1. git config --global user.name "youname"
2. git config --global user.email "youeamil@email.com"
最后可以通过 git config -l 这个命令查看已配置的用户名和邮箱信息

//拉取云端代码
 3. git clone '地址'

 	git branch '分支名'     						//创建分支
 	git branch   		 								//查看本地分支
 	git branch -a  									//查看远端分支
 	git branch '分支名' -d    			 		//删除本地gi分支
 	git push origin -d '分支名' 				//删除远程分支
 	git checkout  '分支名' (默认在master)  		//切换分支

4. 提交代码
git add .   //提交所有更新fetch
git add xxx  //提交某项更新
	//可通过git status  查看当前状态

5. 推送修改到本地git库中
git commit -m "修复XXbug"   

6.推送到远程分支
 git push origin test:master         // 提交本地test分支作为远程的master分支
 git push origin test:test              // 提交本地test分支作为远程的test分支
 git push origin :test              // 如果:左边的分支为空，那么将删除:右边的远程的分支。但是本地还会保存的
	git origin -v     //查看别名origin的具体地址


//与github建立连接并上传本地代码
>>ssh-keygen -t rsa -C "smapustyle@gmail.com"  //生成ssh秘钥

git add README.md
git commit -m "first commit"
git remote add origin git@github.com:smaii/angular5.git
git push -u origin master

#issue =>Everything up-to-date

//更新代码
git remote -v  //查看远程连接地址
	-没有连接地址 => add
		git remote add 'remote_name' 'remote_url'

	git fetch remote_name //拉取代码
	git merge remote_name/branch_name  //合并gi



	#代码加上tag标签  
	git tag [tag_name]

	#git 日志查看
	git log  显示提交记录，上下键浏览。q退出
	git log -–oneline   			--oneline参数可以将每条日志的输出为一行，
    git log --[length]  			 --[length]参数用于指定显示多少条日志
    git log –-skip=[skip]   		--skip=[skip]参数用来指定跳过前几条日志。
    git log -–pretty=raw		--pretty=
    git log    -p                      -p参数输出的信息会更多，用来显示提交的改动记录，相当于多次使用git show [commit_id]的结果。
    git log –-decorate         --decorate参数用来显示一些相关的信息，如HEAD、分支名、tag名等
    git log –-name-status    --name-status参数会带出每次提交对应的文件改动。
    git log --grep keywords  可以从提交的关键字中抓取匹配的commit项。


