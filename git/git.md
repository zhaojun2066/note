"# GIT"

### git 一些协作命令
     1、创建分支
     git branch 新分支
     在哪个分支下建立，默认是建立谁的分支
     建立一个开发分支
     git branch develop

     2、切换到新分支
     git checkout develop ，切换到开发分支

     3、创建和切换为一个命令
     git checkout -b develop ，创建并切换到develop分支
     git checkout -b new-f develop ，基于develop创建并切换到new-f分支

     4、切换分支之前，一定要先commit 否则会切换失败，单不要求push

     5、合并分支 
     当前在develop分支，需要合并某个功能分支
     git merge some-future

     6、查看本地分支列表
     git branch -a

     7、查询远程分支列表
     git branch -r

     8、提交本地分支到远程
     git push origin 本地分支

     9 删除远程分支
     git push origin :分支名称
     git push origin :develop

     10、 删除本地分支
     git branch 分支名称 -d
     git branch 分支 -D 强制删除

     11、更新分支信息
     git fetch -p
     
     12 tag
     git tag -d test_tag　　　　　　　　//本地删除tag
     git push origin :refs/tags/test_tag   删除远程tag

### gitflow 工作流
     历史分支：
     相对使用仅有的一个master分支，Gitflow工作流使用2个分支来记录项目的历史。master分支存储了正式发布的历史，
     而develop分支作为功能的集成分支。这样也方便master分支上的所有提交分配一个版本号
     master
     develop

     功能分支：
     每个新功能位于一个自己的分支，这样可以push到中央仓库以备份和协作。但功能分支不是从master分支上拉出新分支，
     而是使用develop分支作为父分支。当新功能完成时，合并回develop分支。新功能提交应该从不直接与master分支交互。
     也就是说有新的需求一定时是从develop 分支拉取开发，然后功能完善之后再合并到develop分支。
         如：git checkout -b some-feature develop
            中间进行很多的开发..............,然后进行提交
            git status
            git add
            git commit

     发布分支：
     一旦develop 分支的有很多的功能，需要进行发版测试了，此时需要从develop 拉取一个分支，之后这个分支就是用于测试，修复bug，一旦都测试修改完成，
     就需要合并到master分支并分配一个版本号tag ，另外该分支修复完bug 之后，需要重新合并到develop分支。
         如：合并到develop分支
         git pull origin develop
         git checkout develop
         git merge some-feature
         git push
         git branch -d some-feature
         准备发布
         git checkout -b release-0.1 develop
         release-0.1 这个分支是清理发布、执行所有测试、更新文档和其它为下个发布做准备操作的地方，像是一个专门用于改善发布的功能分支。
         测试完成
         合并到master 和 develop 分支，删除发布分支 release-0.1
         git checkout master
         git merge release-0.1
         git push
         git checkout develop
         git merge release-0.1
         git push
         git branch -d release-0.1
         发布分支是作为功能开发（develop分支）和对外发布（master分支）间的缓冲。只要有合并到master分支，就应该打好Tag以方便跟踪。
         git tag -a 0.1 -m "Initial public release" master
         git push --tags


     常见的分支约定：
     用于新建发布分支的分支： develop
     用于合并的分支： master
     分支命名： release-**

     维护分支：
     
     用于快速修改master的bug，它是为一个可以从master fork分支的，修改完成之后，应该马上合并回到master和develop分支，
     同时master分支应该用新的版本号打好tag
     







