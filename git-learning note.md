1.注册账号并创建公开仓库
2.git clone:把远端仓库克隆到D盘
3.git status:查看各种各样的状态（修改了哪些文件；哪些文件还未加入暂存区之类的）
4.git add 文件名：添加单个文件到暂存区
  git add 文件1 文件2：添加多个文件到暂存区
  git add.(注意小数点)：当前所有文件均进入暂存区
5.git commit -m"写本次修改的说明文字":把暂存区文件打包存于本地 还没有上传github
  git log:查看历史记录（详细版本）    git log --oneline(简洁)
  按回车往下翻 按q退出
6.git checkout +git log查到的编号：临时查看旧版本
  查看完后 git checkout main(恢复到最新版本)
7.git reset --+编号：退回指定编号版本 直接便会旧版本 版本之后所有提交记录直接删除（慎用）
8.git revert+编号：没有删掉旧纪录 新建一条反向提交 抵消掉编号那一次commit新增文字（推荐使用 团队协作首选 即使push到github仓库也能使用）
9.git push:执行后可上传到github远端仓库
整体大概操作流程；修改文件→git status查看状态→git add加入暂存区→git commit存档到本地→git push上传至github