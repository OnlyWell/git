#### 1.创建SSH Key
>>>>> - ssh-keygen -t rsa -C "1206402998@qq.com"  //生成密钥对,一个是公钥,一个是私钥,一直回车即可.在用户主目录里找到.ssh目录,里面有id_rsa和id_rsa.pub两个文件,这两个就是SSH Key的密钥对,id_rsa是私钥,id_rsa.pub是公钥.
>>>>> - git remote add origin git@github.com:OnlyWell/git.git
连接到远程仓库(如果服务器是github),
如果git与github连接不上,使用git remote add origin https://github.com/OnlyWell/git.git
>>>>> - git push -u origin master //将本地库的所有内容推到远程库上
>>>>>> - 由于远程库是空的,第一次推送到master分支时,加上了-u参数.git不但会把本地的master分支内容推送到远程新的master分支,还会把本地的master分支和远程的master分支关联起来,在以后的推送或者拉取时可以简化命令.

#### 总结
>>>> - 1.关联一个远程仓库: git remote add origin https://github.com/OnlyWell/git.git
>>>> - 2.关联后,使用命令git push -u orign master第一次推送master分支的所有内容
>>>> - 3.之后如果有必要直接使用 git push origin master推送最新修改
#### ----------------------------------------------------------
#####1.从远程仓库克隆
>>>>> - git clone git@github.com/OnlyWell/git.git
>>>>> - git支持多种协议,包括https,如:git clone https://github.com/OnlyWell/git.git

