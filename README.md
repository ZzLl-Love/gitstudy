
### git 实操问题
***
问题描述: 本地文件的内容修改了但是未提交直接拉取远程代码，pull拉取的时候失败  
根本原因：未提交的修改内容在工作区中没有被正式记录在提交历史中。而git只知道提交历史中文件的状态，无法通过对比历史来知道怎么合并
解决:  
 * 思路： 给本地修改文件提交使其拥有本地历史
 * 实操
   ```
         git add.
         git commit -m "保存本地更改"
         git pull origin master   
 
   ```

### 问题2： 不能切换到主分支
 * 描述
   ``` 
       cloudn‘t checkout master the fllowing untrached working tree  files  would be overwritten by checkout
       不能切换到主分支,在切换分支的时候以下未跟踪的工作树文件将被覆盖   
   ```
 * 思考
   目标分支 与 当前分支 哪个的文件覆盖哪个？  
   ```
      
   ```