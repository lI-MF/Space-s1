# SPACE-S1

# 个人博客项目

Git

1、拉取代码

|          命令          |            说明            |
| :--------------------: | :------------------------: |
| git clone 远程仓库地址 | 拉取代码 （第一次或第N次） |
|        git pull        |          更新代码          |
|        git init        |         初始化代码         |



2、上传代码的步骤

|                    命令                    |                             说明                             |
| :----------------------------------------: | :----------------------------------------------------------: |
|                  git pull                  |                           更新代码                           |
|                 git add .                  |                       提交代码到暂存区                       |
|   git commit -m "备注需要提交的代码内容"   |                        提交到本地仓库                        |
|                  git pull                  | 更新代码【 提交前需要更新（拉取）一次代码，防止覆盖或冲突 】 |
| git push 或  **git push -u origin master** |  把本地仓库内的代码提交到远程仓库  或 【提交到指定的分支】   |
|                 git status                 |   查看需要提交的代码有那些，在哪个步骤下都可以使用该条命令   |

3、切换到本地分支 [在该分支的代码已推送完毕后，再切换到自己想要切换的分支上]

|               命令                |     说明     |
| :-------------------------------: | :----------: |
| git switch main 或 git switch dev | 切换本地分支 |



4、合并分支

|                 命令                  |              说明              |
| :-----------------------------------: | :----------------------------: |
| git checkout main 或 git checkout dev |            切换分支            |
|     git pull main 或 git pull dev     | 要把代码pull下来到最新代码状态 |

4.1 把dev分支的代码merge到主分支 git merge 分支名（当前只合并到了本地）

4.2 将合并的代码git push推上去（这一步 推送到了远程）

5、错误解决：fatal: unable to access 'https://github.com/lI-MF/Space-s1.git/': OpenSSL SSL_read: Connection was reset, errno 10054

|                 命令                 |   说明   |
| :----------------------------------: | :------: |
| git config http.postBuffer 524288000 | 增加缓存 |
|  git config http.sslVerify "false"   |          |













