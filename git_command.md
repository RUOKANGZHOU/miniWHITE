初始化命令：
1. git init                                           //完成文件夹初始化，产生.git的隐藏文件夹，为本地代码库
2. git config --global user.name "用户名"             //初始化设置用户名，仅需一次
3. git config --global user.email 邮箱地址            //初始化设置email


代码提交与存档命令：
1. git status                                        //查看仓库状态
2. git add .                                         //将文件夹内所有文件添加到缓冲区
3. git add + 文件名                                  //将单独的文件放入缓冲区
4. git commit -m "（添加说明）"                      //提交文件进入仓库，并添加说明
5. git commit --amend                               //追加提交，不增增加新的commit-id的情况下将新修改的代码追加到前一次的id当中
6. git log                                          //打印仓库日志
7. git branch                                       //创建分支（会初始化master（主分支）这个默认的分支）
8. git branch + name                                //给分支进行命名
9. git checkout + name                              //切换到所在分支
10.git checkout -b + name                          //命名+切换到所在分支
11.git merge + name                                //首先切换回master分支，再使用此命令合并两个分支
12.git branch -d + name                            //删除分支
13.git branch -D + name                            //强制删除分支
14.git tag + name                                  //贴标签
15.git checkout + name                             //切换到某标签


本地与远程仓库交互
1. ssh-keygen -t rsa                                //生成代码密钥
2. git clone + github上面复制的地址                  //完成对github上面文件的下载
3. git push origin master                           //把本地代码推到远程 master 分支
4. git pull origin master                           //把远程最新的代码更新到本地
我们需要区分 git clone 和 git pull，虽然它们都是从远程仓库到本地的更新，但前者在本地无仓库时使用，后者是本地已有仓库时使用。